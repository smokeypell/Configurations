# TronXY XY-3 Pro v2 Configurations for Marlin Firmware

This configuration is for Tronxy machines with CXY-V6-191121 / CXY-446-V10-220413 boards.
There are options to compile with and without USB flash drive support.

Build Environments:
TRONXY_CXY_446_V10 - Without USB flash drive support
TRONXY_CXY_446_V10_usb_flash_drive - With USB flash drive support

### Compiled firmware file information

- Once successfully compiled, the firmware files will be placed into a folder named `update` in the root of the Marlin project folder.
- Firmware compiles as, both .bin and .hex. TronXY recommends compiling as .hex.
  See the following issue - https://github.com/tronxy3d/F4xx-SIM480x320/issues/6
- Unmount and unplug your Micro-SD card.

### Prepare the SD Card

- Format a Micro-SD card, selecting FAT32 for the file system and 4096 bytes sector size. These parameters are required for the procedure to work.
- Create a folder named `update` on the root of the Micro-SD card.
- Place either 'fmw_tronxy.bin', or 'fmw_tronxy.bin' in the update folder.

### Flash the touchscreen

- Turn off and unplug your printer (both power and USB).
- You will need to access the Micro-SD slot on the printer.
- Insert the Micro-SD card into the printer SD slot.
- Plug the printer's power cable back in (but not the USB cable) and turn on the printer.
- Once powered on, the firmware flash will begin. _Do not cut power to the printer while the procedure is running!_
- The firmware is now up-to-date.