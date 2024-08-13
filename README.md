# OpenDosimeter

Our open-source hardware and software dosimeter offers an afordable solution for real-time, self-monitored radiation exposure. With a total component cost of roughly $90, this device provides an accessible option for radiation monitoring to promote broad access to radiation safety.
<div align=center>
<img width="500" alt="Complete cased device" src="https://github.com/user-attachments/assets/2c953f12-2e8e-4769-899f-a14eeb83f2f3">
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
    Device cost (quantity of 15)
  </div>

## How to Make One 
**This repository has everything you need to create your own OpenDosimeter, below is an explanation of the repository structure:** 

**[Case](https://github.com/OpenDosimeter/OpenDosimeter/tree/main/case):** Use this directory to 3D print the case. It contains two sets of ``.stl`` files that can be downloaded to print top and bottom components for a case with and without a belt clip. 

**[Docs](https://github.com/OpenDosimeter/OpenDosimeter/tree/main/docs):** This is where you can find the reference images used throughout this repository. 

**[Software](https://github.com/OpenDosimeter/OpenDosimeter/tree/main/software):** The software directory has everything you need to program your device, whether you are just looking to download the software with default settings or looking to modify the firmware and make changes to the sketch.  After programming your device, you will be guided through local calibration of your device and an overview of how to use it. 

**[Hardware](https://github.com/OpenDosimeter/OpenDosimeter/tree/main/hardware):** Check out the hardware directory to see the OpenDosimeter board layout in EasyEDA and instructions for ordering it using JLCPCB. This directory contains a breakdown of each component required to assemble the hardware with prices and links to order parts. Furthermore, this is where you can find instructions to assemble your device. 
Additionally, if you prefer to order directly from the PCB manufacturer, you can download the gerber file also located in the ``hardware`` directory. 


**[@OpenDosimeter](https://www.youtube.com/channel/UCCUE-LeyRK8Y6H67ti1gdNA):** Finally, head over to our YouTube channel for instructional manuals on ordering the PCB, assembling, programming, and calibrating the device.

## Working Principle 
$\text{\color{red} Flowchart of device principle coming soon}$

 <div align=center>
    <img width="463"  alt="Flowchart of device principle" src="https://github.com/OpenDosimeter/OpenDosimeter/blob/main/docs/Flowchart.svg">
    </br>
  </div>



## Troubleshooting and FAQ
Refer to [REFERENCE.md](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/REFERENCE.md) for troubleshooting support and guidance in debugging.
- submitting to issues

## Future Improvements
1. The power switch is fragile and can easily be broken if pressed too hard. Future iterations of the hardware could feature a power button similar to the side button which would increase the durability and longevity of the device.
2. In order to make an even more integrated and compact design, the RP2040 chip from the Raspberry Pi Pico could be incorporated in the OpenDosimeter board. 

## Project Team

## Contributing to OpenDosimeter
- interested in contributing to future development and support for new features openDosimeter
- need to add section on contacting developers opendosimeter@gmail.com

## Acknowledgements
Our device is inspired by the [Open Gamma Detector](https://github.com/OpenGammaProject/Open-Gamma-Detector/tree/main)

