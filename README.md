# eggbot_extensions
This repository contains original EggBot Inkscape extension with slight changes to support arduino-based firmware [Eggduino](https://github.com/cocktailyogi/EggDuino)

Changes:
* autodetection of CH340G-based arduinos (`/dev/ttyUSBx` instead of `/dev/ttyACMx`)
* modified serial routine to support arduino bootloader (no need to disable autoreset)

Have fun :)
