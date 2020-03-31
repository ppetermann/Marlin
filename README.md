# Marlin 3D Printer Firmware for Monoprice Delta Mini

A fork of Marlin firmware (2.5.2) for the Monoprice MP Mini Delta 3d printer

<img alt="Monoprice Mini Delta" height="240" align="right"
 src="https://github.com/papabricole/Marlin/raw/malyan-m300/mpminidelta.png" />

## WARNINGS

You need to replace the 12V 5A power brick by a 12V 10A one. Otherwise the printer will be very instable and randomly crash.

## How to build

 - Fork this repo
 - Create a new branch malyan-m300-YourName based onto malyan-m300
 - Edit Marlin/Configuration.h and make your changes
 - Make a pull request
 - Go to this repro, click on the 'Actions' tab, identify your branch
 - When the Build Actions is finished, download the 'firmware.zip' artifact
 
## How to flash

M300 printers require flashing via SD card. Use the SD card that came with the printer if possible. The bootloader is very picky about SD cards.

 - Copy fcupdate.flg and firmware.bin to your SD card
 - Insert the SD card into your printer
 - Power-cycle the printer. The first flash may take longer. Don't be surprised if the .99 version number doesn't show up until after the UI has launched the default screen.
 - Remove the SD card and delete the files from the card to prevent an accidental re-flash.

## Credits

The current Marlin dev team consists of:

 - Scott Lahteine [[@thinkyhead](https://github.com/thinkyhead)] - USA &nbsp; [Donate](http://www.thinkyhead.com/donate-to-marlin) / Flattr: [![Flattr Scott](http://api.flattr.com/button/flattr-badge-small.png)](https://flattr.com/submit/auto?user_id=thinkyhead&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)
 - Roxanne Neufeld [[@Roxy-3D](https://github.com/Roxy-3D)] - USA
 - Chris Pepper [[@p3p](https://github.com/p3p)] - UK
 - Bob Kuhn [[@Bob-the-Kuhn](https://github.com/Bob-the-Kuhn)] - USA
 - João Brazio [[@jbrazio](https://github.com/jbrazio)] - Portugal
 - Erik van der Zalm [[@ErikZalm](https://github.com/ErikZalm)] - Netherlands &nbsp; [![Flattr Erik](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=ErikZalm&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)

## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
