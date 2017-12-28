# RadxQpe
This document describes RadxQpe, which takes the three-dimensional output from RadxPartRain and determines the precipitation rate closest to the surface that satisfies the necessary thresholds in terms of blockage by terrain, .

## Prerequesites
The following items are required:
- RadxPartRain output (cfradial)
- RadxBeamBlock output (cfradial)

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
#### Input params
- input_dir: directory containing radar data (if not specified on the command line and if mode = REALTIME)
- mode: determines if the program waits for new files or if files are specified in a directory

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
