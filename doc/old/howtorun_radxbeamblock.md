# RadxBeamBlock
RadxBeamBlock takes elevation data near a radar to estimate the amount of beam blockage that will occur.

## Prerequesites
The following items are required:
- Elevation model data
- Radar location (lat, lon, alt)
- Specific radar parameters (wavelength, horizontal and vertical beamwidths, gates, azimuth angles, elevation angles)

## Elevation model data
Two digital elevation models are supported: Esri grid data on a spheroid and high-resolution topographic data collected by NASA's Shuttle Radar Topography Mission (SRTM) in 2000.

To download SRTM data for the entire globe (~15 GB compressed), use the following command:
```
wget -r https://dds.cr.usgs.gov/srtm/version2_1/SRTM3/
```
Alternatively, subregions of the globe can be downloaded from subdirectories found at the aforementioned link. All files need to be unzipped.

## Parameter file
Once the elevation data and radar parameters are collected, the parameter file needs to be updated.

### Ensure parameter file is up to date
To obtain the default parameter file, use the following command:
```
/path/to/Radx/apps/RadxBeamBlock -print_params > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
/path/to/Radx/apps/RadxBeamBlock -params orig_param_file_name -print_params > new_param_file_name
```

### Specific parameters to edit
Caution: this is not a complete list, simply a list of important parameters to run RadxBeamBlock. We urge the user to read through the entire parameter file.
#### Input params
- input_dem_path: directory where the elevation data resides
- input_data_format: choose elevation data format from list
#### Radar parameters
- time: specific time not important as it will be used for all timesteps 
- radar_location: lat (degrees), lon (degrees), elevation (km)
- radar_wavelength_cm: radar wavelength
- horiz_beam_width_deg/vert_beam_width_deg: beamwidths for both polarizations
- gates: specify the initial gate distance, gate spacing (both in km), and number of gates in each beam
- azimuths: specify the initial angle, spacing, and number of azimuths
#### Output format
- output_format: select the preferred file type (usually CFRADIAL)
- netcdf_style: if output_format is CFRADIAL, specify the netCDF format
#### Output directory
- output_dir: file will be written to this directory

## Running RadxBeamBlock
To check all command line options for RadxBeamBlock, including debugging options, type the following command into a terminal.
```
/path/to/Radx/apps/RadxBeamBlock -h
```
Once your parameter file is complete, use a command like the following to run the application:
```
/path/to/Radx/apps/RadxBeamBlock -params param_file_name
```
Depending on the number of azimuths, elevations, and gates, this code can take 15-30 minutes to run. 
