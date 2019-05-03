# RadxRate
RadxRate ingests polarimetric radar data and produces three-dimensional fields of the NCAR particle identification (PID) and various precipitation rates.

## Prerequesites
The following items are required:
- Polarimetric radar data (any Radx supported format, e.g., cfradial)
- PID fuzzy logic thresholds file
- Sounding data (either from observations or a numerical model)
- Precipitation rate coefficients (e.g., those found in R(Z) or R(Z,ZDR) equations)
- Parameter files for KDP, PID, and Rate.

## Overview
Overall, RadxRate builds upon the capabilities of RadxKdp and RadxPid by calculating hourly rain rates at each radar gate depending on the local PID category and polarimetric values. It shares parameters files with those two applications. RadxRate will calculate the rain rates with either raw or attenuated-corrected data; the user can choose the option they prefer. The three-dimensional rain rates produced by RadxRate can be then used in RadxQpe to estimate the rain rate closest to the surface, after accounting for beam blockage, noise, and clutter.

## PID thresholds file
These thresholds describe the membership functions for each combination of the PID category and polarimetric field as well as the variable weights for each particle type. The file also contains a place to enter a single sounding, if the data cover a narrow time period; otherwise, the sounding will be overwritten by data provided by the user, which is explained below. The particle types are most sensitive to temperature, Zh, Zdr, and the standard deviations of Zdr and PhiDP. 

Set this to a file suitable for the radar transmit mode and wavelength:

| Wavelength                | Transmit mode | thresholds_file_example |
| -------------             | ------------- | ----------------------- |
| S-band                    | Simultaneous  | [pid_thresholds.sband.shv](./pid_thresholds.sband.shv.md) |
| S-band                    | Alternating   | [pid_thresholds.sband.alt](./pid_thresholds.sband.alt.md) |
| C-band                    | Simultaneous  | [pid_thresholds.cband.shv](./pid_thresholds.cband.shv.md) |
| X-band                    | Simultaneous  | [pid_thresholds.xband.shv](./pid_thresholds.xband.shv.md) |

## Sounding data
If sounding data varies in time, sounding data in a non-gridded data format (SPDB) will need to be ingested. SPDB data can come from either observations or numerical simulations (e.g., RAP or HRRR). For additional information regarding this data format, please see the documentation here (**insert link when written**).

## Precipitation rate coefficients and thresholds
RadxRate has the capability to calculate four different precipitation rates relying on a combination of the PID category and formulas dependent upon polarimetric values. Each algorithm requires user-defined polarimetric variable thresholds (typically Zh, Zdr, and KDP) and precipitation rate coefficients/exponents to determine the appropriate precipitation rate formula. The user should choose values appropriate for the specific radar and precipitation type (e.g., tropical vs continental, stratiform vs convective). These values can be set manually within the parameter file below, but users may find it easier to create a separate bash file that sets environment variables using the Unix 'source' command.

## Parameter files
RadxRate uses four separate parameter files. The first includes the basic parameters related to data location and field names, which is similar to the parameter files for the other Radx applications. The second includes the parameters that set the filtering length, method, and relevant coefficients necessary to calculate KDP and estimate attenuation. The third specifies filter parameters and relevant information related to the soundings used by the PID. The fourth includes all the filters and coefficients necessary to calculate a variety of polarimetric-based rain rates.

### 1) Main parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxRate -print_params > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxRate -params orig_param_file_name -print_params > new_param_file_name
```

#### Important parameters
```
Input params
- input_dir: directory containing radar data (if not specified on the command line and if mode = REALTIME)
- mode: determines if the program waits for new files (REALTIME),
    moves through start and end times specified on the command line (ARCHIVE),
    or moves through list of files specified on the command line (FILELIST)

Input field information
- SNR_available: determines if SNR data is in the file or needs to be calculated from DBZ 
- VARIABLE_field_name: tells RadxRate the polarimetric variable names in the ingested cfradial files 
- LDR_available: determines if LDR data is in the file

Computing KDP
- KDP_params_file_path: path to the KDP-specific parameter file

Computing PID
- PID_params_file_path: path to the PID-specific parameter file
- PID_use_attenuation_corrected_fields: determines whether PID uses Z and ZDR fields that are corrected for attenuation

Computing Rate
- RATE_params_file_path: path to the RATE-specific parameter file
- RATE_use_attenuation_corrected_fields: determines whether RATE equations use Z and ZDR fields that are corrected for attenuation

Writing the output files
- output_dir: files will be written to this directory
- output_format: select the preferred file type (usually CFRADIAL)
```

### 2) KDP-specific parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxRate -print_params_kdp > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxRate -params_kdp orig_param_file_name -print_params_kdp > new_param_file_name
```

#### Important parameters
```
Unfolding and filtering
- KDP_fir_filter_len: Filter length applied to PHIDP

Handling phase shift on backscatter (PSOB)
- KDP_psob_method: Method to handle PSOB
```

### 3) PID-specific parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxRate -print_params_pid > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxRate -params_pid orig_param_file_name -print_params_pid > new_param_file_name
```

#### Important parameters
```
NCAR PID Method
- pid_thresholds_file_path: file path for the PID thresholds file

Sounding input for PID temperatures
- use_soundings_from_spdb: tells RadxRate whether to override the sounding in the pid thresholds file with SPDB data
- PID_sounding_spdb_url: path to SPDB sounding data
```

### 4) Rate-specific parameter file
#### Ensure file is up to date
To obtain the default parameter file, use the following command:
```
lrose -- RadxRate -print_params_rate > param_file_name
```
If you already have a parameter file and simply want to check for (and add) updated parameters while retaining current parameters, use the following command:
```
lrose -- RadxRate -params_rate orig_param_file_name -print_params_rate > new_param_file_name
```

#### Important parameters
All the parameters in this file are important as it contains all the coefficients for each available rain rate relationship. It is important to carefully read this entire file.

## Running RadxRate
To check all command line options for RadxRate, including debugging options and file paths, type the following command into a terminal.
```
lrose -- RadxRate -h
```
Once your parameter file is complete, use a command similar to the following to run the application:
```
lrose -- RadxRate -params param_file_name
```
The user can also specify the location of cfradial files in the following manner:
```
lrose -- RadxRate -f /path/to/cfradial/files/ -params param_file_name
```

## Other relevant items

### Additional parameters to edit
Caution: this is not an exhaustive list. We urge each user to read through the entire parameter file carefully.
#### Main parameter file
```
Specifying copy-through fields
- copy_selected_input_fields_to_output: determines whether original fields are copied to the output file
```
#### KDP-specific parameter file
```
Precip-induced attenuation correction for DBZ and ZDR
- KDP_specify_coefficients_for_attenuation_correction: the user can either set the coefficients 
    or use the default coefficients based on the radar wavelength
```
#### PID-specific parameter file
```
Computing PID
- PID_snr_threshold: mininmum SNR required for the PID to be calculated
- PID_min_valid_interest: mininimum interest value required in order for a PID category to be accepted
- PID_apply_median_filter_to_VARIABLE: sets whether RadxRate applies a filter to specific polarimetric variables
    before running the PID
- PID_ngates_for_sdev: sets the number of gates used to calculate the standard deviations of ZDR and PHIDP

Sounding input for PID temperatures
- sounding_search_time_margin_secs: the maximum allowable time difference between the radar files and sounding data
- sounding_location_name: directs RadxRate to the appropriate sounding
- sounding_required_pressure_range_hpa: sets the minimum pressure range required for a valid sounding
- sounding_required_height_range_m: sets the minimum altitude range required for a valid sounding
```
