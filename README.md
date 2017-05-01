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

As you can see this file has records like RECORD=41, RECORD=34, RECORD=41 and the first one RECORD=1 which are plain text in ASCII

Each of these records has different format and has many parameters or fields and you can see also a lot of rare characters which are a little special. This "special characters are in binary format and are used to store things like the 'symbols', 'electrical type' of the pins, graphical parameters like location X, color or lenght, etc.

This binary data was the more difficult part to obtain and you can find more detailed information in the ASLFF_DataFile.txt file, here in the repository.

I am using all the information exposed here for my own use and for a tool I am developing.

Thanks for read and enjoy!
