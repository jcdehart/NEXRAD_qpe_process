# RadxBeamBlock
RadxBeamBlock estimates the amount of beam blockage due to terrain near a radar.

## Prerequesites
The following items are required:

- Digital elevation model data
- Radar antenna location
- Radar characteristics
- Parameter files for RadxBeamBlock.

## Overview
Overall, RadxBeamBlock takes elevation data, the radar location, and radar characteristics to estimate how much blockage occurs due to terrain.

## Digital elevation model data
The supported digital elevation models include Shuttle Radar Topography Mission and ESRI grid data (spheroid). SRTM data can be found online [here](http://dds.cr.usgs.gov/srtm/version2_1/SRTM3).

## Radar location and characteristics
The radar location requires the latitude, longitude, and elevation of the antenna (ground level + radar height). In addition, characteristics including the wavelength, beamwidth, gate spacing, azimuths, and elevation angles are required. 

## Parameter files
RadxBeamBlock uses one parameter file. Compared to other Radx applications, the RadxBeamBlock parameter file requires just a few edits in order to run. Most of the parameters that need to be changed relate to the radar characteristics.

### 1) Main parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxBeamBlock -print_params > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxBeamBlock -params orig_param_file_name -print_params > new_param_file_name
```

#### Important parameters

Input params

- input_dem_parth: directory containing the elevation data
- input_data_format: specifies the format of the elevation data (examples provided in the parameter file)

Radar parameters

- radar_location: latitude, longitude, and elevation (ground elevation + radar height in km) of the radar antenna 
- radar_wavelength_cm: radar wavelength (cm)
- horiz_beam_width_deg: horizontal beamwidth (degrees)
- vert_beam_width_deg: horizontal beamwidth (degrees)
- gates: starting distance, gate spacing (km), and number of gates
- azimuths: starting azimuth, azimuth spacing (degrees), and number of azimuths
- elevations: starting elevation angle, angle spacing (degrees), and number of elevation angles

Output directory and file name

- output_dir: files will be written to this directory
- output_format: select the preferred file type (usually CFRADIAL)


## Running RadxBeamBlock
To check all command line options for RadxRate, including debugging options and file paths, type the following command into a terminal.
```
lrose -- RadxBeamBlock -h
```
Once your parameter file is complete, use a command similar to the following to run the application:
```
lrose -- RadxBeamBlock -params param_file_name
```
