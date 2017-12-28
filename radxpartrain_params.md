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
These thresholds describe the membership functions for each PID category and polarimetric field combination and the variable weights for each particle type. The file also contains a place to enter a sounding, if the radar files cover a narrow time period; otherwise, the sounding will be overwritten by provided data, which is explained below. The particle types are most sensitive to temperature, Zh, Zdr, and the standard deviations of Zdr and PhiDP. 

## Sounding data
If sounding data varies in time, sounding data in a non-gridded data format (SPDB) will need to be ingested. SPDB data can come from either observations or numerical simulations (e.g., RAP or HRRR). For additional information regarding this data format, please see the documentation here (**insert link**).

## Precipitation rate coefficients and thresholds
RadxPartRain has the capability to calculate four different precipitation rates using techniques dependent upon a mixture of the PID category and formulas dependent upon polarimetric values. Each algorithm requires user-defined polarimetric variable thresholds (typically Zh, Zdr, and KDP) and precipitation rate coefficients and exponents to determine the appropriate precipitation rate formula. The user should choose values appropriate for the specific radar and precipitation type (e.g., tropical vs continental, stratiform vs convective). These values can be set manually within the parameter file below, but  users may find it easier to create a separate bash file that can set variables using the Unix 'source' command.

## Parameter file
Once the data, thresholds, and coefficients have been collected, the parameter file will need to be updated accordingly.

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
Caution: this is not a complete list. We urge each user to read through the entire parameter file carefully.
#### Input params
- input_dir: directory containing radar data (if not specified on the command line and if mode = REALTIME)
- mode: determines if the program waits for new files or if files are specified in a directory
#### Input field information
- SNR_available: determines if SNR data is in the file or needs to be calculated from DBZ 
- VARIABLE_field_name: tells RadxPartRain the polarimetric variable names in the ingested cfradial files 
- KDP_available: determines if KDP data is in the file or needs to be calculated from PHIDP
- LDR_available: determines if LDR data is in the file
#### Computing KDP
- KDP_fir_filter_len: sets the filter length applied in smoothing PHIDP
(include the numerous other choices?)
#### Precip-induced attenuation correction for DBZ and ZDR
- apply_precip_attenuation_correction: determines whether application with produce extra fields that estimate and correct for attenuation in DBZ and ZDR
- specify_coefficients_for_attenuation_correction: the user can either set the coefficients themselves or have the application determine default coefficients for the radar wavelength
#### Computing PID
- pid_thresholds_file_path: file path for the PID thresholds file
- PID_snr_threshold: mininmum SNR required for the PID to be calculated
- PID_min_valid_interest: mininimum interest value required for a PID category to be accepted
- PID_apply_median_filter_to_VARIABLE: determines whether RadxPartRain applies a filter to polarimetric radar data before running the PID
- PID_ngates_for_sdev: sets the number of gates used to calculate the standard deviations of ZDR and PHIDP
#### Sounding input for PID temperatures
- use_soundings_from_spdb: tells RadxPartRain whether to use the sounding from the pid thresholds file or from SPDB files
- sounding_spdb_url: directory where SPDB files are located
- sounding_search_time_margin_secs: sets the maximum allowable time difference between the radar files and sounding data
- sounding_location_name: tells RadxPartRain the name of the radar so that the appropriate soundings can be used
- sounding_required_pressure_range_hpa: sets the minimum pressure range required for a sounding to be valid
- sounding_required_height_range_m: sets the minimum altitude range required for a sounding to be valid
#### Computing precipitation rate
- PRECIP_snr_threshold: minimum SNR required for precipitation rate to be returned
- PRECIP_apply_median_filter_to_VARIABLE: determines whether RadxPartRain applies a filter to polarimetric radar data before calculating the precipitation rate
- PRECIP_min_valid_rate: precipitation rates below this value will be set to 0.
- PRECIP_max_valid_rate: precipitation rates above this value will be set to this hourly rate.
- PRECIP_max_valid_dbz: DBZ exceeding this value will be set to this maximum before the precipitation rate is calculated, to mitigate the influence of hail.
- PRECIP_brightband_dbz_correction: in the brightband, the reflectivity is reduced by this value before calculating the precipitation rate.
#### Precip coefficients
Parameters in this section determine the specific thresholds, coefficients, and exponents that set the polarimetric precipitation rate formulas that were discussed in a previous section.
#### Specifying copy-through fields
- copy_input_fields_to_output: determines whether fields from the original cfradial files are copied to the final file (e.g., Zh, ZDR)
#### Output format
- output_format: select the preferred file type
- netcdf_style: if output_format is CFRADIAL, specify the netCDF format
#### Output directory
- output_dir: files will be written to this directory

## Running RadxPartRain
To check all command line options for RadxPartRain, including debugging options and file paths, type the following command into a terminal.
```
/path/to/Radx/apps/RadxPartRain -h
```
Once your parameter file is complete, use a command similar to the following to run the application:
```
/path/to/Radx/apps/RadxBeamBlock -params param_file_name
```
The user can also specify the location of cfradial files in the following manner:
```
/path/to/Radx/apps/RadxBeamBlock -f /path/to/cfradial/files/ -params param_file_name
```
