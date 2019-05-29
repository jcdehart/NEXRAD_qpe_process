# RadxQpe
RadxQpe ingests three-dimensional output from RadxRate and determines the precipitation rate closest to the surface that satisfies beam blockage and data quality requirements.

## Prerequesites
The following items are required:

- Three-dimensional file of rain rates created by RadxRate (cfradial)
- Beamblock file created by RadxBeamBlock (cfradial)
- Parameter file for running RadxQpe

## Overview
RadxQpe synthesizes the files created by RadxRate and RadxBeamBlock to determine the best estimate of surface rainfall. RadxBeamBlock data is used to determine the data closest to the surface with minimal blocking by terrain. For irregularly-spaced elevation angles, RadxQpe finds the elevation angle in BeamBlock closest to the elevation angle in the files from RadxRate. Additional constraints based on the signal to noise ratio, beam height, and minimum precipitation rate can be set to constrain where data is reported.

## Parameter files
RadxQpe uses one parameter file that includes the basic parameters related to data location and field names, which is similar to the parameter files for the other Radx applications, and other parameters that specify when precipitation rates will be written to the output file. 

### 1) Main parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxQpe -print_params > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxQpe -params orig_param_file_name -print_params > new_param_file_name
```

#### Important parameters

Inputs/outputs

- data_url: directory containing the output from RadxRate
- snr_field: name of the SNR field in the RadxRate files (empty if no field)
- pid_field: name of the PID field in the RadxRate files 
- beam_block_path: path to the RadxBeamBlock file
- beam_block_field: field name of the maximum beam blockage percentage (accumulated)

Polar output format

- output_format: select the preferred file type

Polar output directory and filename

- output_dir: file will be written to this directory (set to empty if the user does not want polar output)

Cartesian grid projection and XY details, and output specification

- output_cartesian_dir: file will be written to this directory (set to empty if the user does not want cartesian output)


## Running RadxQpe
To check all command line options for RadxQpe, including debugging options and file paths, type the following command into a terminal.
```
lrose -- RadxQpe -h
```
Once your parameter file is complete, use a command similar to the following to run the application:
```
lrose -- RadxQpe -params param_file_name
```
The user can also specify the location of cfradial files in the following manner:
```
lrose -- RadxQpe -f /path/to/cfradial/files/ -params param_file_name
```

## Other relevant items

### Additional parameters to edit
Caution: this is not an exhaustive list. We urge each user to read through the entire parameter file carefully.
#### Main parameter file

Algorithm parameters

- azimuthal_resolution_degrees: sets the azimuthal resolution of the output files
- min_snr: if the SNR lies below this threshold for a gate, a higher elevation angle is used
- max_beam_block_percent: beam blockage percentage must be below this threshold or else a higher elevation angle will be used
- max_beam_height_km_msl: the beam must not be above this height, otherwise the precipitation will be set to 0
- min_valid_precip_rate: any precipitation rates less than this threshold will be set to 0

Inputs/outputs

- rainrate_fields: sets the precipitation rates that are saved to the final files; the user can choose their preferred rate from the four options
- output_fields: additional fields the user would like to see in the final files

Cartesian grid projection and XY details, and output specification

- grid_projection: map projection for the cartesian grid
- grid_xy_geom: sets the lower left corner of the cartesian grid, grid size, and grid spacing
- center_grid_on_radar: centers the grid on the radar and not a (lat, lon) location
- min_nvalid_for_interp: the number of points required for interpolation to occur
- set_discrete_fields: option to use discrete values for certain fields instead of interpolation
- discrete_fields: list of fields that should use nearest neighbor instead of interpolation (e.g., PID)

