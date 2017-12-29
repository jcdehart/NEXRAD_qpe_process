# RadxQpe
This document describes RadxQpe, which takes the three-dimensional output from RadxPartRain and determines the precipitation rate closest to the surface that satisfies the necessary thresholds in terms of blockage by terrain, .

## Prerequesites
The following items are required:
- RadxPartRain output files (cfradial)
- RadxBeamBlock output files (cfradial)

## Parameter file
The parameter file will need to be updated accordingly.

### Ensure parameter file is up to date
To obtain the default parameter file, use the following command:
```
/path/to/Radx/apps/RadxQpe -print_params > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
/path/to/Radx/apps/RadxQpe -params orig_param_file_name -print_params > new_param_file_name
```

### Specific parameters to edit
Caution: this is not a complete list. We urge each user to read through the entire parameter file carefully.
#### Algorithm parameters
- azimuthal_resolution_degrees: sets the azimuthal resolution of the output files
- min_snr: if the SNR lies below this threshold for a gate, a higher elevation angle is used
- max_beam_block_percent: beam blockage percentage must be below this threshold or else a higher elevation angle will be used
- max_beam_height_km_msl: the beam must not be above this height, otherwise the precipitation will be set to 0
- min_valid_precip_rate: any precipitation rates less than this threshold will be set to 0
#### Inputs/outputs
- data_url: directory containing the output from RadxPartRain
- snr_field: name of the SNR field in the RadxPartRain files (empty if no field)
- pid_field: name of the PID field in the RadxPartRain files 
- beam_block_path: path to the RadxBeamBlock file
- beam_block_field: field name of the maximum beam blockage percentage (accumulated)
- rainrate_fields: sets the precipitation rates that are saved to the final files; the user can choose their preferred rate from the four options
- output_fields: additional fields the user would like to see in the final files
#### Polar output format
- output_format: select the preferred file type
- netcdf_style: if output_format is CFRADIAL, specify the netCDF format
#### Polar output directory and filename
- output_dir: file will be written to this directory (set to empty if the user does not want polar output)
#### Cartesian grid projection and XY details, and output specification
- output_cartesian_dir: file will be written to this directory (set to empty if the user does not want cartesian output)
- grid_projection: map projection for the cartesian grid
- grid_xy_geom: sets the lower left corner of the cartesian grid, grid size, and grid spacing
- center_grid_on_radar: centers the grid on the radar and not a (lat, lon) location
- min_nvalid_for_interp: the number of points required for interpolation to occur
- set_discrete_fields: option to use discrete values for certain fields instead of interpolation
- discrete_fields: list of fields that should use nearest neighbor instead of interpolation (e.g., PID)

## Running RadxQpe
To check all command line options for RadxQpe, including debugging options and file paths, type the following command into a terminal.
```
/path/to/Radx/apps/RadxQpe -h
```
Once your parameter file is complete, use a command similar to the following to run the application:
```
/path/to/Radx/apps/RadxQpe -params param_file_name
```
The user can also specify the location of cfradial files in the following manner:
```
/path/to/Radx/apps/RadxQpe -f /path/to/cfradial/files/ -params param_file_name
```
