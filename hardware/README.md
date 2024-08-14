# Hardware
Our design leverages a cusom OpenDosimeter board, LYSO scintillation crystal and SiPM (silicon photomultiplier). The figure below outlines key features of the OpenDosimeter board that is essential to the hardware design. 
<div align=center>
<img width="600" alt="board-overview" src="https://github.com/user-attachments/assets/4594c9e4-8149-4a25-a02a-83c2b1c2eb5e">
</div>

## Components

### OpenDosimeter PCB
Follow these steps to order the OpenDosimeter board: 
1. **Download Files:** download the following files located in this folder
    - [openDosimeter_PCB_EasyEDA.json](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/hardware/OpenDosimeter_PCB_EasyEDA.json)
    - [openDosimeter_SCH_EasyEDA.json](https://github.com/OpenDosimeter/OpenDosimeter/blob/main/hardware/OpenDosimeter_SCH_EasyEDA.json)
2. **Open in EasyEDA**
    - Go to easyeda.com
    - Log in or create an account
    - Click ``Design Online``
    - Click ``Std Edition``
    - Click ``New Project`` and give it a title
    - Drag and drop both the ``PCB`` and ``SCH`` files into EasyEDA

      | Schematic |<img width="700" alt="Image of Schematic File" src="https://github.com/user-attachments/assets/e582a008-7870-41ae-bcdd-088169dfb7a5">|
      |---------------------------------------------|--------------------------------------------------------------------------------------|
      | **PCB** |<img width="700" alt="Image of PCB File" src="https://github.com/user-attachments/assets/ce661b25-9531-46c1-96a8-eccab1b3691f"> |

    - ``File`` --> ``Save`` or ``CMD + s`` to save both files to the project you created
    - On the PCB file, click ``Fabrication`` --> ``One Click Order PCB/SMT`` --> ``Yes, Check DCR`` --> ``One Click Order`` --> ``OK``
3. **Open in JLCPCB**
    - Once redirected to JLCPCB, log in or create an account
    - Choose quantity of PCB
    - Recomended: ``Select LeadFree HSL``
    - Select ``PCB Assembly``
    - ``Confirm`` --> ``Next`` --> ``Next`` --> ``OK``
    - Select a product description from drop down
    - Add to cart and checkout
  
**A complete tutorial for ordering the OpenDosimeter Board is on our YouTube**
<div align="center">
<a href="https://youtu.be/UWabvXynp9I" target="_blank">
    <img  src="https://github.com/OpenDosimeter/OpenDosimeter/blob/main/docs/Thumnail%201.png" alt="Ordering OpenDosimeter Board Thumbnail" width="540" target="_blank" style="border:none;">
</a>
</div>
</br>



### 3D Printed Case 
We have designed 3D-printable cases for OpenDosimeter with different styles. Each case has two parts, a top and bottom. The ``.stl`` files can be found in the [case](https://github.com/OpenDosimeter/OpenDosimeter/tree/main/case) folder.

### Table of Materials
Here are all of the required components and tools for assembly. Also included is the purpose, specification details, cost, and links to purchase each component. 
| Component            | Purpose  | Specification| Cost (USD) | Where to buy (example) |
|------------------------|--------|------------------|------------|---------|
|OpenDosimeter PCB| Main Board  |Custom PCB, see instructions above | $20 |Directly from PCB manufacturer |
|Battery  | Power |LiPo protected battery, ideally >1200 mAh, size around 34mm L x 62mm W x 5mm H | $10 |[1200 mAh Lipo battery](https://www.digikey.com/en/products/detail/adafruit-industries-llc/258/5054544) |
|Display| Displaying dose values to user |128x64 pixels, I2C, SSD1306 | $5 | [Amazon, 128x64 pixels, I2C, SSD1306](https://www.amazon.com/Teyleten-Robot-Display-SSD1306-Raspberry/dp/B0CN373JF4/ref=sr_1_4?crid=2FMQS7B2IFQAD&dib=eyJ2IjoiMSJ9.l-FK2pxw8wWhZ_wtkFb4O1fyrXLIhGQ52dk_-yA7h6FWtEW-CW5RA7_9w5hhpIE9lSkkBIurGV3JAYvQS695jjQR0VVPaO92fd4QVHkD4CTCp4bQsF8CrU8NM0aMPuOZ8RjYMbesVbpG_UDMbMGqyALbXdphIb0nHzBxKLcVF0Pm0UNgyMb1CITVfuh6bqspsPWljCJVLda51Ct931b4NpiFFhTkOtDTzaaWjYwOTCTaZgTjvpziUI1kPpnvJCXBBrgzoC6xlvPtjO4YGGF54xkeJpWnkoouL7rm1iE_GsA.JpSEJVJP5Itir15xcqstihVBHkHDpMhWXXJUSeBi6w4&dib_tag=se&keywords=i2c+128x64+oled+display&qid=1717603122&s=electronics&sprefix=i2c+128x64+oled+sipl%2Celectronics%2C134&sr=1-4) |
|Raspberry Pi Pico| Microcontroller for programming |Regular version with no headers | $4 | [Raspberry Pico](https://www.digikey.com/en/products/detail/raspberry-pi/SC0915/13684020) |
|SiPM| Visible light sensor |6 mm model (MICROFC-60035-SMT-TR) | $33 | [MICROFC-60035-SMT-TR onsemi](https://www.digikey.com/en/products/detail/onsemi/MICROFC-60035-SMT-TR/9742618) |
|Plastic tweezer| Handling LYSO and SiPM without scratching it | Any plastic is fine| $5 |[Amazon, Electronic Repair Plastic Tweezers](https://www.amazon.com/Auniwaig-Anti-static-Tweezers-Precision-Electronics/dp/B08V4BF99K/ref=sr_1_12?crid=2P40DUMKMZHT0&dib=eyJ2IjoiMSJ9.5iYaL1v0I09-iIDQSI0il9h9dCchGEMT1_R94GDH6QmGBH9JFVbAaTAhQZnx0XBo4cjV3EEqDrwTKModIGqUoZWvEqlQyNpFlKvh4ELaqovPHcoU8QCtQ_gAPJ3ZQqBBykfEOf3ee_Jy_4Cu1DA4cSwaO0_pREw9jqP76LslU0dONBOJbGBz6dSRFpDfedrx9rXWLsOMbWLiBONTW1WC0Ly0xX2P2gjgEt74SLqEWsFbY5vmGJeui-m0vcTuJ7wPjrXGSxMzvf9YKbVLzJ0jwkunz39TJtpU8bXlPIO1iSg.wfmLhkznWWSroapnGolqC6t9x1-rZ5mUHo_qM8KZED4&dib_tag=se&keywords=plastic+tweezer+1+pc&qid=1722446225&refinements=p_36%3A-600&rnid=1243644011&sprefix=plastic+tweezer+1+pc%2Caps%2C127&sr=8-12) |
|Electrical Tape| Light sealing of X-ray sensor assembly (SiPM + LYSO) |Black color to efficiently absorb light| $5 |[Amazon, 3/4 Inch Black Electrical Tape ](https://www.amazon.com/Scotch-Super-33-Electrical-carton/dp/B0000AZ9HG/ref=sr_1_3?crid=379MWXWL4Y0R4&dib=eyJ2IjoiMSJ9.XvYh8n8zmezRYWLAeSMp20zS9aMZ_OkZg9vVBnTuU9GBnum6MaLk_FPOJdiiIQndOT6PMejF4weVSVKhDYIE3xq4anvIYIb2bUix0Xf1IJWaM_yuLf7KJLssxgNuyph5Qr31Q8kyOHiXkHE_QoVhGvJzU42l153y9bNqDpVcdg1LXhe9vM8SUbilLvBktT7x3NhoBBvg5GYRCd9G_OwcpAwru3oxciV83fxZaOs_FNA.jo3fPo-i_RRH7EV2clOFCC7W_iUatKs2lCPoXZ7GGuU&dib_tag=se&keywords=electrical+tape+black+3M&qid=1722446293&sprefix=electrical+tape+black+3m%2Caps%2C133&sr=8-3) |
|Aluminum Tape| Light sealing of X-ray sensor assembly (SiPM + LYSO) | Up to 0.1mm thickness to avoid absorbing X-rays | $19 |[Amazon, Aluminum Foil Tape(3M)](https://www.amazon.com/3M-Foil-Tape-3381-Silver/dp/B00A7I5L86/ref=sr_1_4?crid=3FZZ6HXVJFKJW&dib=eyJ2IjoiMSJ9.8g7E604QbHpwyZvpiHS3KOL4D3rbTgkJXTTxyiqD9h9b-tUnIXUthRJ0kzFq5Y0kKPXasQMRFyWgzRdT74c3A0QlN1IbgHV3P2SP6Lm4cNlWMsj0mbBnfrKRNlUb_2VNj8dCcybmoFVXx98mwtjPjzYzJFfLs8Ut27cfT1oYEoi0NeQUm26s7w9ase0wYRub1rl0tQPrTFYCIdzNUsw3XmRI0fHvdR4uIouX2Y2r9mk.iRudZFUJZVLtJbsEUs6dUpkbcNRu_nmlgzl6Sg9rv3g&dib_tag=se&keywords=aluminum+tape+3m&qid=1722446481&sprefix=aluminum+tape+3m%2Caps%2C134&sr=8-4) |
|Optical Couplant | Improving light coupling and adhesion between LYSO crystal and the SiPM  | Should be viscous enough to apply easily, but any will do | $33 | [Amazon, MOLYKOTE 4 Electrical Insulating Compound](https://www.amazon.com/Dow-Corning-Electrical-Insulating-Compound/dp/B0195UWAHG/ref=sr_1_1?crid=1FDS4YSQBHPVO&dib=eyJ2IjoiMSJ9.gfqP0gv9GKU1J2V8zgA0DIDlFhblCyriWhmx9rixKP4DlPxaEkgcBvgK9pTtv9ylH2qXpEG7Q0Jr_dqlBQAYybvFcqWoDgZY5-vvUUvg9PZ8B5LmGmroxZlqPYVmTveAXmyWjn8t2abIkMnV_ef1-QQflucTbNi13fpyZnEI9CO0lSYM9HJYMK2EkayUmpfo-NmrVb7GUy98wMPoeMR1yX3z4wpON1PGkZhy6cWraXs.iPNCpVDAOINZHw5AYk9FiJiEVbZVzLLVk0iQbdBasXg&dib_tag=se&keywords=molykote+4+electrical+insulating+compound&qid=1722446595&sprefix=molykote+in%2Caps%2C131&sr=8-1) |

**Note on Cost**
- Price on OpenDosimeter board decreases substantially the larger quantity you order
- Device assembly only requires small amounts of Electrical Tape, Aluminum Tape, and Optical Couplant, thus the total cost is inflated by their initial purchase.







