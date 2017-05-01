# Altium_SLFF
Altium Schematic Library File Format (SLFF)

WARNING! The information exposed here is only with educational purposes, use at your own risk.

This repository contains information about the Schematic Library file format of the EDA Software Altium Designer 16.

The schematic library are saved as a file with extension .schlib like example.schlib

This file is in reallity a zipped file. If we have a single component and we decompress that library we obtain this files:

- FileHeader
- Storage
- Component_1 : a folder 'Component_n' for each component.
   - Data
   - Other files ...
   
One of the more important files of the library is on 'Data' file. This file has 'records' in both ASCII format and binary values, you can see that in this picture:

![Altiumm Schematic Library File Format ScreenShoot](https://github.com/braincodec/Altium_SLFF/raw/master/AltiumSLFF_001.png)


