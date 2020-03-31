# Marlin 3D Printer Firmware for Monoprice Delta Mini

A fork of Marlin firmware (2.5.2) for the Monoprice MP Mini Delta 3d printer

<img alt="Monoprice Mini Delta" height="240" align="right"
 src="https://github.com/papabricole/Marlin/raw/malyan-m300/mpminidelta.png" />

## WARNINGS

You need to replace the 12V 5A power brick by a 12V 10A one. Otherwise the printer will be very instable and randomly crash.

## How to build

This repo use github actions to build the firmware for you.

 1. Fork this repo
 2. On your forked repo, go to the 'Actions' tab and activate your workflows by clicking 'I understand my workflows, go ahead and run them'
 3. Edit Marlin/Configuration.h directly from github and make your changes
 4. Create a pull request
 5. Go back to the 'Actions' tab: a build action has been triggered
 6. When the Build Action is finished, download the 'firmware.zip' artifact
 7. Every time you update your pull request, a new build will be triggered

## How to flash

M300 printers require flashing via SD card. Use the SD card that came with the printer if possible. The bootloader is very picky about SD cards.

 - Copy fcupdate.flg and firmware.bin to your SD card
 - Insert the SD card into your printer
 - Power-cycle the printer. The first flash may take longer. Don't be surprised if the .99 version number doesn't show up until after the UI has launched the default screen.
 - Remove the SD card and delete the files from the card to prevent an accidental re-flash.

