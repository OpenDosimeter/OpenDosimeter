# Software 
This software folder contains a precompiled file for simplest set up, and the arduino sketch to make changes to the software. Below are instructions for how to program your OpenDosimeter. 

## Programming the Raspberry Pi Pico
### Default Settings
**If you don't want to change the code and just want to program the pico with default settings follow these steps!**
1. Download the [OpenDosimeter.uf2](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/software/OpenDosimeter.uf2) file in the software file
2. Use the micro-USB connection to plug the Raspberry Pi Pico into a computer
3. When the file manager window pops up, drag the ``OpenDosimeter.uf2`` file into the directory. Your device should restart and is now ready for callibration.

### Modifying the Code in ArduinoIDE
**Here's how you can modify the provided code**
1. Download ArduinoIDE
2. Download Arduino-Pico so your computer recognizes the Raspberry Pi Pico
3. Download the folder [OpenDosimeter_ino](https://github.com/OpenDosimeter/OpenDosimeter/tree/main/software/OpenDosimeter_ino)
4. Open the file ``OpenDosimeter_ino.ino`` to open the code in ArduinoIDE
5. Use the Library Manager (tools --> library manager) to download the following dependency packages
    - TaskScheduler
    - SimpleShellEnhanced
    - ArduinoJson
    - Adafruit_SSD1306
    - Adafruit_SH110X
    - RunningMedian
6. Modify the code as desired
7. Flash the Pico
    - Tools --> Board --> Raspberry Pi RP2040 Boards --> Flash Size: 2MB (Sketch: 1MB, FS: 1MB)
    - Keep remaining settings at default values
    - Press the ``Upload`` button

### Programmed Device Overview
**A complete overview of the device is on our YouTube channel**

<div align="center">
<a href="https://www.youtube.com/watch?v=nXH3Gc72z8Y" target="_blank">
    <img  src="https://github.com/user-attachments/assets/b8d9e2cf-32de-4e3b-ae07-3a61a8f6a33e" alt="OpenDosimeter Device Overview" width="540" style="border:none;">
</a>
</div>
</br>
Once your device is programmed, you should see the OpenDosimeter home screen and firmware version. There are 
<img width="800" alt="software states" src="https://github.com/user-attachments/assets/c6200f90-329b-47db-9c23-d41645b06a1c">
$\text{\color{red} is this a good section to add? not in OGD}$

### Calibrating the Device
$\text{\color{red} is this a good section to add? not in OGD}$
### Data Log
$\text{\color{red} Add link to data log once website live}$







