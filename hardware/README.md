# Hardware
<div align=center>
<img width="600" alt="board-overview" src="https://github.com/user-attachments/assets/4594c9e4-8149-4a25-a02a-83c2b1c2eb5e">
</div>
This hardware folder contains the schematic and PCB design files needed to manufacture the OpenDosimeter board. Our design leverages a LYSO scintillation crystal and SiPM (silicon photomultiplier). 
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

      | PCB |<img width="700" alt="Image of PCB File" src="https://github.com/user-attachments/assets/ce661b25-9531-46c1-96a8-eccab1b3691f"> |
      |---------------------------------------------|--------------------------------------------------------------------------------------|
      | **Schematic** |<img width="700" alt="Image of Schematic File" src="https://github.com/user-attachments/assets/e582a008-7870-41ae-bcdd-088169dfb7a5">|

    - File --> Save or CMD + s to save both files to the project you created
    - On the PCB file, click Fabrication --> One Click Order PCB/SMT --> Yes, Check DCR --> One Click Order --> OK
3. **Open in JLCPCB**
    - Once redirected to JLCPCB, log in or create an account
    - Select quantity of PCB
    - Recomended: Select LeadFree HSL
    - Select PCB Assembly
    - Confirm --> Next --> Next --> OK
    - Select a product description from drop down
    - Add to cart and checkout

### 3D Printed Case 
We have designed 3D-printable cases for OpenDosimeter with different styles. Each case has two parts, a top and bottom. The .stl files can be found in the [case](https://github.com/OpenDosimeter/OpenDosimeter/tree/main/case) folder.
### Scintillator Crystals 
$\text{\color{red} Link to brand and location of LYSO crystals we recommend using}$

### SiPM (Silicon Photomultipier)
$\text{\color{red} Fill this in}$

### Optical Couplant
Applying optical couplant between the scintilattor crystal and SiPM will allow efficient photon detection and reduce reflections. Many options will work, we recommend the following 

| Component            | Purpose  | Specification| Cost (USD) | Where to buy (example) |
|------------------------|--------|------------------|------------|---------|
|OpenDosimeter custom PCB| Main Board  |  | $20 |Directly from PCB manufacturer |
|Battery  | Power |LiPo protected battery, ideally >1200 mAh, size around 34mm L x 62mm W x 5mm H | $10 |[1200 mAh Lipo battery](https://www.digikey.com/en/products/detail/adafruit-industries-llc/258/5054544) |
|Display| Displaying dose values to user |128x64 pixels, I2C, SSD1306 | $5 | [Amazon, 128x64 pixels, I2C, SSD1306](https://www.amazon.com/Teyleten-Robot-Display-SSD1306-Raspberry/dp/B0CN373JF4/ref=sr_1_4?crid=2FMQS7B2IFQAD&dib=eyJ2IjoiMSJ9.l-FK2pxw8wWhZ_wtkFb4O1fyrXLIhGQ52dk_-yA7h6FWtEW-CW5RA7_9w5hhpIE9lSkkBIurGV3JAYvQS695jjQR0VVPaO92fd4QVHkD4CTCp4bQsF8CrU8NM0aMPuOZ8RjYMbesVbpG_UDMbMGqyALbXdphIb0nHzBxKLcVF0Pm0UNgyMb1CITVfuh6bqspsPWljCJVLda51Ct931b4NpiFFhTkOtDTzaaWjYwOTCTaZgTjvpziUI1kPpnvJCXBBrgzoC6xlvPtjO4YGGF54xkeJpWnkoouL7rm1iE_GsA.JpSEJVJP5Itir15xcqstihVBHkHDpMhWXXJUSeBi6w4&dib_tag=se&keywords=i2c+128x64+oled+display&qid=1717603122&s=electronics&sprefix=i2c+128x64+oled+sipl%2Celectronics%2C134&sr=1-4) |
|Raspberry Pi Pico| Microcontroller for programming |Regular version with no headers | $4 | [Raspberry Pico](https://www.digikey.com/en/products/detail/raspberry-pi/SC0915/13684020) |
|SiPM| Visible light sensor |6 mm model (MICROFC-60035-SMT-TR) | $33 | [MICROFC-60035-SMT-TR onsemi](https://www.digikey.com/en/products/detail/onsemi/MICROFC-60035-SMT-TR/9742618) |

|Plastic tweezer| Handling LYSO and SiPM without scratching it | | $5 | [Amazon, Electronic Repair Plastic Tweezers](https://www.amazon.com/Auniwaig-Anti-static-Tweezers-Precision-Electronics/dp/B08V4BF99K/ref=sr_1_12?crid=2P40DUMKMZHT0&dib=eyJ2IjoiMSJ9.5iYaL1v0I09-iIDQSI0il9h9dCchGEMT1_R94GDH6QmGBH9JFVbAaTAhQZnx0XBo4cjV3EEqDrwTKModIGqUoZWvEqlQyNpFlKvh4ELaqovPHcoU8QCtQ_gAPJ3ZQqBBykfEOf3ee_Jy_4Cu1DA4cSwaO0_pREw9jqP76LslU0dONBOJbGBz6dSRFpDfedrx9rXWLsOMbWLiBONTW1WC0Ly0xX2P2gjgEt74SLqEWsFbY5vmGJeui-m0vcTuJ7wPjrXGSxMzvf9YKbVLzJ0jwkunz39TJtpU8bXlPIO1iSg.wfmLhkznWWSroapnGolqC6t9x1-rZ5mUHo_qM8KZED4&dib_tag=se&keywords=plastic+tweezer+1+pc&qid=1722446225&refinements=p_36%3A-600&rnid=1243644011&sprefix=plastic+tweezer+1+pc%2Caps%2C127&sr=8-12) |
|Optical Couplant | Improving light coupling and adhesion between LYSO crystal and the SiPM  |  | ~$33 | [Amazon, MOLYKOTE 4 Electrical Insulating Compound](https://www.amazon.com/Dow-Corning-Electrical-Insulating-Compound/dp/B0195UWAHG/ref=sr_1_1?crid=1FDS4YSQBHPVO&dib=eyJ2IjoiMSJ9.gfqP0gv9GKU1J2V8zgA0DIDlFhblCyriWhmx9rixKP4DlPxaEkgcBvgK9pTtv9ylH2qXpEG7Q0Jr_dqlBQAYybvFcqWoDgZY5-vvUUvg9PZ8B5LmGmroxZlqPYVmTveAXmyWjn8t2abIkMnV_ef1-QQflucTbNi13fpyZnEI9CO0lSYM9HJYMK2EkayUmpfo-NmrVb7GUy98wMPoeMR1yX3z4wpON1PGkZhy6cWraXs.iPNCpVDAOINZHw5AYk9FiJiEVbZVzLLVk0iQbdBasXg&dib_tag=se&keywords=molykote+4+electrical+insulating+compound&qid=1722446595&sprefix=molykote+in%2Caps%2C131&sr=8-1) |


$\text{\color{red} Add more rows to the table of recomendations}$



