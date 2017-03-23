# Adafruit Featherwing OLED Demo

This repository contains files used for the Adafruit Featherwing OLED Demo that is [here](https://learn.adafruit.com/digital-display-badge?embeds=allow) .


## Manual Arduino BSP Setup

The preferred method of installing the WICED Feather BSP is to use the Adafruit WICED package from the Arduino Board Manager, but if you wish to maintain the git repo to contribute pull requests you can manually install this BSP with the following setup procedure:

- Create a **hardware/adafruit** folder in `~/Documents/Arduino` (OS X) or
  `My Documents\Arduino` (Windows) if it doesn't already exist
- Clone this repo to the root of the `hardware/adafruit` folder, or download as a .zip and
  unzip it into `hardware/adafruit/wiced`

	```
	git clone https://github.com/adafruit/Adafruit_WICED_Arduino.git
	```
	
- You should end up with a folder structure like this:

	```
        .
        └── Arduino
            ├── hardware
            │   └── adafruit
            │       └── wiced
            │           ├── README.md
            │           ├── boards.txt
            │           ├── bootloader
            │           ├── changelog.md
            │           ├── cores
            │           ├── drivers
            │           ├── featherlib
            │           ├── keywords.txt
            │           ├── libraries
            │           ├── platform.txt
            │           ├── programmers.txt
            │           ├── tools
            │           └── variants
	```
	
- Install the necessary GCC toolchain for ARM: Tools->Board->Board Manager --> Download **Arduino SAM Boards (32-bits ARM Cortex-M3)**
- Restart the Arduino IDE
ew Windows binary will need to be generated.  Follow the steps below
on a Windows machine with the **32-bit version** of Python (for maximum compatibility
with all Windows versions, since 32-bit executables can run on 64-bit Windows too).

First you need to install the dependencies of the script.  This is only done
once (unless the dependencies change).  From inside the `tools/source/feather_dfu`
folder run:
```
pip install -r requirements.txt --pre
```
