# OpenDosimeter

Our open-source hardware and software dosimeter offers an afordable solution for real-time, self-monitored X-ray radiation exposure. With a total component cost of roughly $90, this device provides an accessible option for radiation monitoring to promote broad access to radiation safety. This project is based on the [Open Gamma Detector](https://github.com/OpenGammaProject/Open-Gamma-Detector), with the main new feature being the effective dose calculations (in Sv) from the detected spectrum.

<p float="center">
  <img src="https://github.com/OpenDosimeter/OpenDosimeter/blob/main/docs/OpenDosimeter%20logo.png" width="35%" /> 
  <img src="https://github.com/user-attachments/assets/2c953f12-2e8e-4769-899f-a14eeb83f2f3" width="35%" />
</p>

## Key Features 
- **Open-Source Design:** The hardware and software are fully open-source, enabling customization and personalization to enhance and broaden the capabilities of the dosimeter
- **Compact Design:** 73mm x 42mm x 23mm
- **Easily Programmable:** Drag and drop firmware files
- **Buzzer:** Built in buzzer allows for optional audible warnings when radiation exposure exceeds predefined limit (default off)
- **Local Calibration:** Using Am-241 from an ionization household smoke detector, the device can be calibrated for accurate dose calculations
- **Real-time:** Instantly read out radiation exposure levels, eliminating the need for specialized read-out facilities, pre-existing infrastructure, and monthly subscription fees (e.g., for OSL or TLD badges)
- **Affordable:** With a price point around $90, the device is a low-cost option to democratize access to radiation safety
- **Data Logging:** Storage of dose rates and accumulated dose for the last 10 hours on the device (1 s sampling).
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
The flow chart below illustrates the operation, using grey boxes to represent hardware components and orange boxes to indicate software functionality (inspired by the [Open Gamma Detector flowchart](https://github.com/OpenGammaProject/Open-Gamma-Detector/tree/main?tab=readme-ov-file#working-principle), demonstrating the similarity of the underlying design). The current software version (1.0) implements photon-counting capabilities (excellent for low to medium dose rates). A parallel energy-integrating component (for medium to high dose rates)is under development for the upcoming software version 1.1.
 <div align=left>
    <img width="600"  alt="Flowchart of device principle" src="https://github.com/OpenDosimeter/OpenDosimeter/blob/main/docs/Flowchart.png">
    </br>
</div>

## Troubleshooting and FAQ
Refer to [REFERENCE.md](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/REFERENCE.md) for troubleshooting support and guidance in debugging.


## Future Improvements
1. The current power switch on the OpenDosimeter board is fragile and sometimes breaks. Future iterations of the hardware should replace for a more durable model.
2. In order to make an even more integrated and compact design, the RP2040 chip from the Raspberry Pi Pico could be incorporated into the OpenDosimeter board. 

## Project Team
Many people have contributed to the realization of this project so far:
- Kian Shaker (Stanford University) **[Project lead]**
- Alice Ku (Stanford University)
- Jasmyn Lopez (Stanford University)
- Enoch Anyenda (University of Nairobi)
- Norah Ger (Mama Lucy Kibaki Hospital, Nairobi)
- Grace Ateka (Kenya Bureau of Standards)
- Jia Wang (Stanford University)
- Robert Bennett (Stanford University)
- Adam Wang (Stanford University)
- Matthias Rosezky (https://nuclearphoenix.xyz/)

## Contributing to OpenDosimeter
The OpenDosimeter is a living project and we invite people to submit issues, suggest improvements, and contribute to future development!

Want to contribute? Reach out to Kian Shaker (kians@stanford.edu / opendosimeter@gmail.com)

## Acknowledgements
_Inspiration:_ The basis for our hardware and software is the fantastic [Open Gamma Detector](https://github.com/OpenGammaProject/Open-Gamma-Detector/tree/main) project, check it out! Much of its detailed documentation is relevant to the OpenDosimeter as well (SiPM behavior, X-ray counting concept etc.)

_Funding support:_ King Center on Global Development at Stanford University, Knut and Alice Wallenberg Foundation
