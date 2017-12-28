# RadxPartRain
This document describes the application that ingests polarimetric radar data and produces three-dimensional fields of the particle identification (PID) and precipitation rates.

## Prerequesites
The following items are required:
- Polarimetric radar data (any Radx supported format, e.g., cfradial)
- PID fuzzy logic thresholds file
- Sounding data (either observed or simulated)
- Precipitation rate coefficients (e.g., R(Z), R(Z,ZDR))

## PID thresholds file
The specific thresholds will need to be tuned to the specific radar. NCAR has some example files that have been tuned for [S-BAND in fast alternating mode (FHV)](https://ral.ucar.edu/projects/titan/docs/radial_formats/pid_thresholds.sband.alt.txt) and [C-BAND in simultaneous-transmit (SHV) mode](https://ral.ucar.edu/projects/titan/docs/radial_formats/pid_thresholds.cband.shv.txt).

## Parameter file
Once the elevation data and radar parameters are collected, the parameter file will need to be updated accordingly.

### Ensure parameter file is up to date
To obtain the default parameter file, use the following command:
```
/path/to/Radx/apps/RadxPartRain -print_params > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
/path/to/Radx/apps/RadxPartRain -params orig_param_file_name -print_params > new_param_file_name
```

### Specific parameters to edit
Caution: this is not a complete list, simply the most important for running the code. Read through the entire parameter file.
#### Input params
- input_dem_path: directory containing elevation data
- input_data_format: choose elevation data format from list

### Running RadxPartRain
