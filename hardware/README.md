# Hardware

This hardware file contains the schematic and PCB design files needed to manufacture the OpenDosimeter board. Our design leverages a LYSO scintillation crystal and SiPM (silicon photomultiplier). 
## Components

### OpenDosimeter PCB
Follow these steps to order the OpenDosimeter board: 
1. **Download Files:** download the following files located in this folder
    - [openDosimeter_PCB_EasyEDA.json](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/hardware/OpenDosimeter_PCB_EasyEDA.json)
    - [openDosimeter_SCH_EasyEDA.json](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/hardware/OpenDosimeter_SCH_EasyEDA.json)
2. **Open in EasyEDA**
    - Go to easyeda.com
    - Log in or create an account
    - Click the "Design Online"
    - Click "Std Edition"
    - Click "New Project" and give it a title
    - Drag and drop both the PCB and SCH files into EasyEDA

               | PCB |<img width="800" alt="Image of PCB File" src="https://github.com/user-attachments/assets/ce661b25-9531-46c1-96a8-eccab1b3691f"> |
               |---------------------------------------------|--------------------------------------------------------------------------------------|
               | **Schematic** |<img width="800" alt="Image of Schematic File" src="https://github.com/user-attachments/assets/e582a008-7870-41ae-bcdd-088169dfb7a5">|

    - File --> Save or CMD + s to save both files to the project you created
    - On the PCB file, click Fabrication --> One Click Order PCB/SMT --> Yes, Check DCR --> One Click Order --> OK
3. **Open in JLCPCB**
    - Once redirected to JLCPCB, log in or create an account
    - Select quantity of PCB
    - Recomended: Select LeadFree HSL
    - Select PCB Assembly
    - Confirm --> Next --> Next -->
    - Select a product description from drop down
    - Add to cart and checkout

### 3D Printed Case 
We have designed 3D-printable cases for OpenDosimeter with different styles. Each case has two parts, a top and bottom. The .stl files can be found in the [case](https://github.com/OpenDosimeter/OpenDosimeter/tree/main/case) folder.
### Scintillator Crystals 
$\text{\color{red} Link to brand and location of LYSO crystals we recommend using}$

### 
### Optical Couplant

