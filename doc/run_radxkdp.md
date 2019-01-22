# RadxKdp
RadxKdp ingests polarimetric radar data and calculates KDP from PHIDP.

## Prerequesites
The following items are required:
- Polarimetric radar data (any Radx supported format, e.g., cfradial)
- Two parameter files to run RadxKdp and to set KDP.

## Overview
RadxKdp uses a couple different methods to calculate KDP from PHIDP. In general, KDP is calculated from the PHIDP slope between range gates (after smoothing and unfolding the PHIDP data). Filtering smears out KDP in range, so an additional field (KDP_SC) is constrained by KDP estimated theoretically from Z and ZDR.

## Parameter files
RadxKdp uses two separate parameter files. The first includes the basic parameters related to data location and field names, which is similar to the parameter files for the other applications. The second includes the parameters that set the filtering length, method, and relevant coefficients necessary to calculate KDP and estimate attenuation.

### 1) Main parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxKdp -print_params > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxKdp -params orig_param_file_name -print_params > new_param_file_name
```

#### Important parameters
```
Input params
- input_dir: directory containing radar data (if not specified on the command line and if mode = REALTIME)
- mode: determines if the program waits for new files or if files are specified in a directory

Input field information
- SNR_available: determines if SNR data is in the file or needs to be calculated from DBZ 
- VARIABLE_field_name: tells RadxKdp the polarimetric variable names in the ingested cfradial files 

Computing KDP
- KDP_params_file_path: path to the KDP-specific parameter file

Output format
- output_format: select the preferred file type (usually CFRADIAL)

Output directory
- output_dir: files will be written to this directory
```

### 2) KDP-specific parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxKdp -print_params_kdp > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxKdp -params_kdp orig_param_file_name -print_params_kdp > new_param_file_name
```

#### Important parameters
```
Unfolding and filtering
- KDP_fir_filter_len: Filter length applied to PHIDP

Handling phase shift on backscatter (PSOB)
- KDP_psob_method: Method to handle PSOB
```

## Running RadxKdp
To check all command line options for RadxPartRain, including debugging options and file paths, type the following command into a terminal.
```
lrose -- RadxKdp -h
```
Once your parameter file is complete, use a command similar to the following to run the application:
```
lrose -- RadxKdp -params param_file_name
```
The user can also specify the location of cfradial files in the following manner:
```
lrose -- RadxKdp -f /path/to/cfradial/files/ -params param_file_name
```
