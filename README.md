# OpenDosimeter

Our open-source hardware and software dosimeter offers an afordable solution for real-time, self-monitored radiation exposure. With a total component cost of roughly $90, this device provides an accessible option for radiation monitoring to promote broad access to radiation safety.
<div align=center>
<img width="650" alt="device-overview" src="https://github.com/user-attachments/assets/2c953f12-2e8e-4769-899f-a14eeb83f2f3">
</div>




## Key Features 
- **Open-Source Design:** The hardware and software are fully open-source, enabling customization and personalization to enhance and broaden the capabilities of the dosimeter
- **Compact Design:** 73mm x 42mm x 23mm
- **Easily Programmable:** Drag and drop firmware files
- **Buzzer:** Built in buzzer allows for optional audible warnings when radiation exposure exceeds predefined limit (default off)
- **Local Calibration:** Using Am-241 from an ionization household smoke detector, the device can be calibrated for accurate dose calculations
- **Real-time:** Instantly read out radiation exposure levels, eliminating the need for specialized read-out facilities, pre-existing infrastructure, and monthly subscription fees (e.g., for OSL or TLD badges)
- **Affordable:** With a price point around $90, the device is a low-cost option to democratize access to radiation safety
  <div align=center>
    <img width="463"  alt="Cost Breakdown" src="https://github.com/user-attachments/assets/65f5abfe-b1fb-4192-8f79-10c1414b636d">
    </br>
    Device cost with quantity of 15
  </div>

## How to Make One 
Check out the ``hardware`` for instructions to order the PCB, get the ``.stl`` files to 3D print the case, and find links to all other components. Additionally, you can find step by step instructions for assembling the device, programming and calibrating it, and a device overview over on our YouTube channel [@OpenDosimeter](https://www.youtube.com/channel/UCCUE-LeyRK8Y6H67ti1gdNA). 

## Working Principle 
$\text{\color{red} Flowchart coming soon}$

## Hardware 
Our hardware has been designed using EasyEDA. The ``hardware`` directory contains all the files needed and instructions for odering the board. Additionally, if you prefer to order directly from the PCB manufacturer, you can download the gerber file also located in the ``hardware`` directory. 
<br> 
## Software 
The ``software`` directory has everything you need to program your device, whether you are just looking to download the software with default settings or looking to modify the firmware and make changes to the sketch. 

## Troubleshooting and FAQ
$\text{\color{red} If we want this section, we should create a REFERENCE.md to answer questions}$

## Known Limitations 
1. The power switch is fragile and can easily be broken if pressed too hard. Future iterations of the hardware could feature a power button similar to the side button which would increase the durability and longevity of the device.

$\text{\color{red} 2. Other limitations}$

