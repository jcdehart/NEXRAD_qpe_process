# Quantitative Precipitation Estimation (QPE) for NEXRAD radar data

This document details the required steps to apply a QPE algorithm to NEXRAD radar data. The steps discussed include data format conversion, removal of inadequate data, determination of precipitation type, calculation of precipitation rate, and selection of the highest quality QPE value closest to the surface.

## Prerequisites

The following data and programs will be required.
- NEXRAD data
- RadxConvert
- Soloii (for radar editing)
- RadxPartRain
- RadxBeamBlock
- RadxQpe

## Where to find data

NEXRAD data can be found at NCAR's motherlode website.

## Editing and Programs

### Convert data to sweep format for editing

Soloii will allow editing of wind data and other variables to clean up data.

### Convert edited data to cfradial format
  * [CfRadial documentation](https://github.com/NCAR/CfRadial/tree/master/docs)

Convert data from sweep format to cfradial for use within other Radx programs.

### Run NCAR PID algorithm and calculate rain rate

RadxPartRain first calculates the most likely hydrometeor type for each data point. Based on the particle type and polarimetric data, different R(Z), R(Z, Zdr), and R(Kdp) relationships are used to calculate the rain rate at each gate/azimuth/elevation combination.

### Calculate percentage of beam blockage

RadxBeamBlock will calculates fraction of beam blockage at each point. Uses digital elevation data from NASA space shuttle STS-99 Mission (Dixon et al. 2015).

### Determine highest quality "surface" measurement

RadxQpe synthesizes the results of RadxPartRain and RadxBeamBlock to determine the best estimate of the surface precipitation. To be considered good data, there must be less than 25% beam blocking, the signal to noise ratio must be strong enough, and the radar volume must lie below an appropriate altitude. RadxQpe generates a 2-D horizontal grid of the radar volumes closest to the surface that satisfy the aforementioned conditions. The precipitation rate determined by RadxPartRain is then accepted as the "surface" precipitation rate and is returned.
