# Parameter File Guidance

This document highlights the critical changes one should make before using the default parameter files that come with each Radx application. While we attempt to include all parameters that are important to properly run each application, we encourage a thorough read through of each parameter file.

## Obtaining Up-To-Date parameter files

To ensure that your parameter file is capatible with the most recent code, run the following command to generate a new parameter file given your original settings. This will add parameters that are missing and remove parameters deemed unnecessary. Original settings for unchanged parameters carry through to the new file.

```
[Radx App] -params [original param file] -print_params > [new param file]
```

Note: if using emacs, param files use syntax highlighting of c++ file. Type "M-x c++-mode" to enable highlighting. 
M = alt key or option key, depending upon your OS.

## General notes
- debug sets the amount of messages printed to the terminal.
- output_dir sets the location where files will be saved.

## Applications (sorted alphabetically)
### RadxBeamBlock

### RadxConvert
- output_format: choose between several formats, where dorade is suggested if you will be editing files in soloii and cfradial for most usage by other Radx applications.

### RadxPartRain

### RadxQpe

### Radx2Grid
