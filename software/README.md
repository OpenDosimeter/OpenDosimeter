# Software 
This software folder contains a precompiled file for simplest set up, and the arduino sketch to make changes to the software. Below are instructions for how to program your OpenDosimeter. 

## Step 1: Programming the Raspberry Pi Pico
### Option 1: Default Settings
**If you don't want to change the code and just want to program the pico with default settings follow these steps!**
1. Download the [OpenDosimeter.uf2](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/software/OpenDosimeter.uf2) file in the software file
2. Use the micro-USB connection to plug the Raspberry Pi Pico into a computer
3. When the file manager window pops up, drag the ``OpenDosimeter.uf2`` file into the directory. Your device should restart and is now ready for callibration.
   
$\text{\color{red} Programming Video Coming Soon!}$

### Option 2: Modifying the Code in ArduinoIDE
**Here's how you can modify the provided code**
1. Download ArduinoIDE
2. Download Arduino-Pico so your computer recognizes the Raspberry Pi Pico
3. Download the folder [OpenDosimeter_ino](https://github.com/OpenDosimeter/OpenDosimeter/tree/main/software/OpenDosimeter_ino)
4. Open the file ``OpenDosimeter_ino.ino`` to open the code in ArduinoIDE
5. Use the Library Manager (``tools`` --> ``library manager)`` to download the following dependency packages
    - ``TaskScheduler``
    - ``SimpleShellEnhanced``
    - ``ArduinoJson``
    - ``Adafruit_SSD1306``
    - ``Adafruit_SH110X``
    - ``RunningMedian``
6. Modify the code as desired
7. Flash the Pico
    - ``Tools`` --> ``Board`` --> ``Raspberry Pi RP2040 Boards`` --> ``Flash Size: 2MB (Sketch: 1MB, FS: 1MB)``
    - Keep remaining settings at default values
    - Press the ``Upload`` button

### Step 2: Calibrating the Device
**A step-by-step guide to calibrating the device is on our YouTube channel**
<div align="center">
<a href="https://www.youtube.com/watch?v=btqXVTFHygs" target="_blank">
    <img  src="https://github.com/user-attachments/assets/e5be1f51-4546-4f0d-8dd3-b335cabdabfa" alt="OpenDosimeter Calibration" width="540" target="_blank" style="border:none; ">
</a>
</div>

1. Extract Am-241 from household ionization smoke detector
2. Turn ``ON`` your assembled and programmed device
3. ``Long Press`` side button to open Reset/Calibration menu
4. ``Long Press`` again to begin calibration
5. Align Am-241 with the circle on the back of the case
    - You should see two peaks forming
    - Keep Am-241 in place until calibration is complete (~1 minute)
6. Your device should say ``Calibrating...Done``

**For troubleshooting, checkout the [REFERENCE.md](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/REFERENCE.md)**



### Step 3: Programmed Device Overview
**A complete overview of the device is on our YouTube channel**

<div align="center">
<a href="https://www.youtube.com/watch?v=nXH3Gc72z8Y" target="_blank">
    <img  src="https://github.com/user-attachments/assets/b8d9e2cf-32de-4e3b-ae07-3a61a8f6a33e" alt="OpenDosimeter Device Overview" width="540" target="_blank" style="border:none;">
</a>
</div>e

Once your device is programmed, you should see the OpenDosimeter home screen and firmware version. Below is a flowchart that shows how you can use the side button to navigate between the different programmed states. 
<div align="center">
<img width="700" alt="software states" src="https://github.com/user-attachments/assets/c6200f90-329b-47db-9c23-d41645b06a1c">
</div>


### Data Log
$\text{\color{red} Link to Data Log Coming Soon!}$







