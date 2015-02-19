# eggbot_extensions
This repository contains original EggBot Inkscape extension with slight changes to support arduino-based firmware [EggDuino](https://github.com/bartebor/EggDuino) forked from [CocktailYogi's version](https://github.com/cocktailyogi/EggDuino)

Changes:
* autodetection of CH340G-based arduinos (`/dev/ttyUSBx` instead of `/dev/ttyACMx`)
* modified serial routine to support arduino bootloader (no need to disable autoreset - new option available on Options page)

Have fun :)
