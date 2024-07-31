# Troubleshooting and FAQ 

## Troubleshooting 

#### Calibration/Device Settings are Not Saved 
This is likely due to not allocating any memory for the file system. When you flash the Pico, be sure that you have selected the following setting: ``Boards`` --> ``Flash Size: 2MB (Sketch: 1MB, FS: 1MB)`` so the Pico has memory allocated for the file system. 


## FAQ 

#### Can I Modify the Program? 
Yes! Check out Step 1, Option 2 in the software [README.md](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/software/README.md) for detailed instructions to modify the code and flash the Pico using ArduinoIDE.
