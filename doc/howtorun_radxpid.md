# RadxPid
RadxPid produces three-dimensional fields of the NCAR particle identification (PID).

## Prerequesites
The following items are required:

- Polarimetric radar data (any Radx supported format, e.g., cfradial)
- PID fuzzy logic thresholds file
- Sounding data (either from observations or a numerical model)
- Three parameter files to run RadxPid, calculate KDP, and PID.

## Overview
RadxPid ingests polarimetric data to estimate the dominant hydrometeor type using NCAR's Particle Identification algorithm. First, KDP is calculated from PHIDP using the same KDP-specific parameter file as RadxKdp. Next, the polarimetric radar data and calculated KDP are combined with sounding data to determine the most likely dominant hydrometeor. The user decides whether or not the algorithm will use the raw Zh and Zdr data from the radar or correct for attenuation. Finally, the resulting three-dimensional PID categories are sent to an output file.

## PID thresholds file
These thresholds describe the membership functions for each combination of the PID category and polarimetric field as well as the variable weights for each particle type. The file also contains a place to enter a sounding, if the radar files cover a narrow time period; otherwise, the sounding will be overwritten by data provided by the user, which is explained below. The particle types are most sensitive to temperature, Zh, Zdr, and the standard deviations of Zdr and PhiDP. 

Set this to a file suitable for the radar transmit mode and wavelength:

| Wavelength                | Transmit mode | thresholds_file_example |
| -------------             | ------------- | ----------------------- |
| S-band                    | Simultaneous  | [pid_thresholds.sband.shv](pid_thresholds.sband.shv.md) |
| S-band                    | Alternating   | [pid_thresholds.sband.alt](pid_thresholds.sband.alt.md) |
| C-band                    | Simultaneous  | [pid_thresholds.cband.shv](pid_thresholds.cband.shv.md) |
| X-band                    | Simultaneous  | [pid_thresholds.xband.shv](pid_thresholds.xband.shv.md) |

## Sounding data
If sounding data varies in time, sounding data in a non-gridded data format (SPDB) will need to be ingested. SPDB data can come from either observations or numerical simulations (e.g., RAP or HRRR). For additional information regarding this data format, please see the documentation here (**insert link when written**).

## Parameter files
RadxPid uses three separate parameter files. The first includes the basic parameters related to data location and field names, which is similar to the parameter files for the other applications. The second includes the parameters that set the filtering length, method, and relevant coefficients necessary to calculate KDP and estimate attenuation. The third specifies filter parameters and relevant information related to the soundings used by the PID.

### 1) Main parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxPid -print_params > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxPid -params orig_param_file_name -print_params > new_param_file_name
```

#### Important parameters

Input params

- input_dir: directory containing radar data (if not specified on the command line and if mode = REALTIME)
- mode: determines if the program waits for new files (REALTIME),
    moves through start and end times specified on the command line (ARCHIVE),
    or moves through list of files specified on the command line (FILELIST)
    
Input field information

- SNR_available: determines if SNR data is in the file or needs to be calculated from DBZ 
- VARIABLE_field_name: tells RadxPid the polarimetric variable names in the ingested cfradial files 
- LDR_available: determines if LDR data is in the file

Computing KDP

- KDP_params_file_path: path to the KDP-specific parameter file

Computing PID

- PID_params_file_path: file path for the PID-specific parameter file
- PID_use_attenuation_corrected_fields: determines whether PID uses Z and ZDR fields that are corrected for attenuation

Writing the output files

- output_dir: files will be written to this directory
- output_format: select the preferred file type (usually CFRADIAL)


### 2) KDP-specific parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxPid -print_params_kdp > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxPid -params_kdp orig_param_file_name -print_params_kdp > new_param_file_name
```

#### Important parameters

Unfolding and filtering

- KDP_fir_filter_len: Filter length applied to PHIDP

Handling phase shift on backscatter (PSOB)

- KDP_psob_method: Method to handle PSOB


### 3) PID-specific parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxPid -print_params_pid > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxPid -params_pid orig_param_file_name -print_params_pid > new_param_file_name
```

#### Important parameters

NCAR PID Method

- pid_thresholds_file_path: file path for the PID thresholds file

Sounding input for PID temperatures

- use_soundings_from_spdb: tells RadxPid whether to override the sounding in the pid thresholds file with SPDB data
- PID_sounding_spdb_url: path to SPDB sounding data


## Running RadxPid
To check all command line options for RadxPid, including debugging options and file paths, type the following command into a terminal.
```
lrose -- RadxPid -h
```
Once your parameter file is complete, use a command similar to the following to run the application:
```
lrose -- RadxPid -params param_file_name
```
The user can also specify the location of cfradial files in the following manner:
```
lrose -- RadxPid -f /path/to/cfradial/files/ -params param_file_name
```

## Other relevant items

### Additional parameters to edit
Caution: this is not an exhaustive list. We urge each user to read through the entire parameter file carefully.
#### Main parameter file

Specifying copy-through fields

- copy_selected_input_fields_to_output: determines whether original fields are copied to the output file

#### KDP-specific parameter file

Precip-induced attenuation correction for DBZ and ZDR

- KDP_specify_coefficients_for_attenuation_correction: the user can either set the coefficients themselves or use the default coefficients based on the radar wavelength

#### PID-specific parameter file

Computing PID

- PID_snr_threshold: mininmum SNR required for the PID to be calculated
- PID_min_valid_interest: mininimum interest value required in order for a PID category to be accepted
- PID_apply_median_filter_to_VARIABLE: determines whether RadxPid applies a filter to specific polarimetric variables
    before running the PID
- PID_ngates_for_sdev: sets the number of gates used to calculate the standard deviations of ZDR and PHIDP

Sounding input for PID temperatures

- sounding_search_time_margin_secs: the maximum allowable time difference between the radar files and sounding data
- sounding_location_name: directs RadxPid to the appropriate sounding
- sounding_required_pressure_range_hpa: sets the minimum pressure range required for a valid sounding
- sounding_required_height_range_m: sets the minimum altitude range required for a valid sounding

