# My Keyboard

```bash
util/docker_build.sh massdrop/alt:sunggun_mac_md
```

Download `mdloader` for mac from <https://github.com/Massdrop/mdloader>

```bash
chmod +x mdloader_mac
```

Download `applet-mdflash.bin` files

```bash
wget https://raw.githubusercontent.com/Massdrop/mdloader/master/applet-mdflash.bin
```

Run firmware upgrade

```bash
./mdloader_mac --first --download massdrop_alt_sunggun_mac_md.bin --restart
```

then press fn + b for 1 sec and release. the keyboard led will turned off and firware update will be proceed

```txt
Massdrop Loader 1.05

Massdrop Loader  Copyright (C) 2018-2020 Massdrop Inc.
This program is Free Software and has ABSOLUTELY NO WARRANTY

Scanning for device for 60 seconds
.........
Device port: /dev/cu.usbmodem1A122201 (SAMD51J18A)

Opening port '/dev/cu.usbmodem1A122201'... Success!
Found MCU: SAMD51J18A
Bootloader version: v2.18Sep  4 2018 16:48:28
Applet file: applet-mdflash.bin
Applet Version: 1
Writing firmware... Complete!
Booting device... Success!
Closing port... Success!
```
