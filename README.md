# JJRC-X9 firmwares

Repo for JJRC's X9 firmwares, as APM / QGC may flash your drone with a not compatible one.
depending on wich mainboard you have, choose your firmware, and burn !
Don't try another fw version, as hardware are a lot different, it won't boot.

## Tools used ##

 * STlink v2 emulator (USB) : https://www.amazon.com/Aideepen-ST-Link-Programming-Emulator-Downloader/dp/B01J7N3RE6
 * stlink / stflash (linux) : https://github.com/texane/stlink

## Backup/Flash firmware (linux) ##

 * backup : `st-flash --format binary read mydump.bin 0x08000000 0x100`
 * flash : `st-flash write firmware.bin 0x8000000`

or use stlink-gui : (available on all distrib's repo).

## Thanks ##

 * sidri from kopterforum.at
