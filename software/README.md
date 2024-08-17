# Software 
This software folder contains a precompiled file for simplest set up, and the arduino sketch to make changes to the software. The software was based on the [Open Gamma Detector](https://github.com/OpenGammaProject/Open-Gamma-Detector) (FW. 4.2.1). Below are instructions for how to program your OpenDosimeter once you have assembled it:

## Step 1: Programming the Raspberry Pi Pico
### Option 1: Default Settings
**If you don't want to change the code and just want to program the pico with default settings follow these steps!**
1. Download the [OpenDosimeter.uf2](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/software/OpenDosimeter.uf2) file in the software folder
2. Connect the OpenDosimeter to the computer using the micro-USB port of the Raspberry Pico
3. When it is your first time programming the Pico, it should appear as an external drive. When the  file manager window pops up, drag the ``OpenDosimeter.uf2`` file onto the drive. Your device should then automatically restart and is now ready to be calibrated (go to Step 2).
   
**Check out our YouTube video showing the steps above**
<div align="center">
<a href="https://youtu.be/HLWoSg5BW90" target="_blank">
    <img  src="https://github.com/OpenDosimeter/OpenDosimeter/blob/main/docs/Thumbnail%203.png" alt="Programming Thumbnail" width="540" target="_blank" style="border:none; ">
</a>
</div>

### Option 2: Uploading using ArduinoIDE
**Useful if you'd like to see how the code works for potentially modifying it**

_Set up the programming environment_
1. Install ArduinoIDE
2. Install Raspberry Pi Pico Board in the ArduinoIDE
   - Open Arduino --> ``Settings/Preferences`` --> ``Additional Board Managers URL``
   - Add this link: https://github.com/earlephilhower/arduino-pico/releases/download/global/package_rp2040_index.json
   - Press ``OK``
   - Go to ``Board Manager``
   - Search for "Raspberry Pico" and install ``Raspberry Pi Pico/RP2040 by Earle F. Phillhower, III``
3. Use the Library Manager (``tools`` --> ``library manager)`` to install the following dependency packages
    - ``TaskScheduler``
    - ``SimpleShellEnhanced``
    - ``ArduinoJson``
    - ``Adafruit_SSD1306``
    - ``Adafruit_SH110X``
    - ``RunningMedian``

_Download the OpenDosimeter software_

4. Download the folder [OpenDosimeter_ino](https://github.com/OpenDosimeter/OpenDosimeter/tree/main/software/OpenDosimeter_ino)
5. Open the file ``OpenDosimeter_ino.ino`` to open the code in ArduinoIDE
6. Here you can inspect and modify the code to add new desired features
   
_Program the Device_

8. Flash the Pico
    - Connect Pico over USB
    - Choose the following settings:
       - **Board:** ``Tools`` --> ``Board`` --> ``Raspberry Pi RP2040 Boards``
       - **Port:** ``Tools`` --> ``Port`` Select associated port 
       - **Flash Size:** ``Tools`` --> ``Flash Size: 2MB (Sketch: 1MB, FS: 1MB)``
    - Keep remaining settings at default values
    - Press the ``Upload`` button

## Step 2: Calibrating the Device
**A step-by-step guide for calibrating the device is on our YouTube channel**
<div align="center">
<a href="https://youtu.be/eI6PJFmvRmY" target="_blank">
    <img  src="https://github.com/OpenDosimeter/OpenDosimeter/blob/main/docs/Thumbnail%204.png" alt="Calibrating Thumbnail" width="540" target="_blank" style="border:none; ">
</a>
</div>
</br>

1. Extract Am-241 from any household ionization smoke detector
    - See this [video](https://www.youtube.com/watch?v=lOWNI6bC5EM) for disassembling instructions
2. Turn ``ON`` your assembled and programmed device (using the power switch)
3. ``Long Press`` side button to open Reset/Calibration menu
4. ``Long Press`` again to begin calibration
5. Align Am-241 with the circle on the back of the case
    - You should see two peaks forming
    - Keep Am-241 in place until calibration is complete (up to 1 minute recording)
6. Your device should say ``Calibrating...Done``

**For troubleshooting, checkout the [REFERENCE.md](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/REFERENCE.md)**

## Step 3: Programmed Device Overview
**A complete overview of the device is on our YouTube channel**
<div align="center">
<a href="https://youtu.be/77HooAmk0_8" target="_blank">
    <img  src="https://github.com/OpenDosimeter/OpenDosimeter/blob/main/docs/Thumbnail%205.png" alt="Device Overview Thumbnail" width="540" target="_blank" style="border:none; ">
</a>
</div>
</br>

Once your device is programmed, you should see the OpenDosimeter home screen and firmware version. Below is a flowchart that shows how you can use the side button to navigate between the different programmed states. 
<div align="center">
<img width="700" alt="software states" src="https://github.com/user-attachments/assets/c6200f90-329b-47db-9c23-d41645b06a1c">
</div>


## Data Log
$\text{\color{red} Link to Data Log Coming Soon!}$







