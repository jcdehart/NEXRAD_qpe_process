# Calculate Quantitative Precipitation Estimate (QPE) for NEXRAD radar

This document details the required steps to calculate the QPE for a NEXRAD radar. The steps discussed include data format conversion, removal of inadequate data, determination of precipitation type, calculation of precipitation rate, and selection of the highest quality QPE value closest to the surface.

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

### Convert data to sweep format for radar editing

Soloii will allow editing of wind data and other variables to clean up data.

### Convert edited data to cfradial format

Convert data from sweep format to cfradial for use within other Radx programs.

### Run NCAR PID algorithm and calculate rain rate

RadxPartRain calculates the most likely particle type for each data point. Based on the particle type and dual-pol observations, different R(Z), R(Z, Zdr), and R(Kdp) relationships are used.

### Calculate percentage of beam blockage

RadxBeamBlock will calculates fraction of beam blockage at each point. Uses digital elevation data from NASA space shuttle STS-99 Mission (Dixon et al. 2015).

### Determine highest quality "surface" measurement

RadxQpe synthesizes the results of RadxPartRain and RadxBeamBlock to determine the lowest radar beams with less than 25% beam blocking and below an appropriate altitude. The precipitation rate determined by RadxParRain is then accepted as the "surface" precipitation rate and the surface rain is returned.
