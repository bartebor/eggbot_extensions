# eggbot_extensions
This repository contains original EggBot Inkscape extension with changes to support arduino-based firmware [EggDuino](https://github.com/bartebor/EggDuino) forked from [CocktailYogi's version](https://github.com/cocktailyogi/EggDuino)

Changes:
* autodetection of CH340G-based arduinos (`/dev/ttyUSBx` instead of `/dev/ttyACMx`)
* modified serial routine to support arduino bootloader (no need to disable autoreset - new option available on Options page)
* new smooth movement mode (option on Options page) available only with my modified EggDuino firmware). This mode sends special buffering-friendly SMQB command instead of SM/QB pairs.
* autodisabling motors after plotting without layers. In layered mode motors stay on to allow pen change without repositioning.

Note it is still **better to disable autoreset** (I'm using 10uF capacitor connected between RESET and +5V).
Autoreset is annoying especially in manual mode, because:
- commands initiated from extension are delayed until arduino resets (about 2s)
- there are movements of the motors and/or pen during reset
- your board may be not autodetected at all
 
Have fun :)
