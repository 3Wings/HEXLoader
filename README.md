# HEXLoader
Arduino Flash and Backup tool.

NOTES!! Things to do, error handling when flashing if comport is not selected

Test Flash and backup for: Mega 1280, Nano 328 & 168 & Uno


Usage backup::

1) Connect Arduino board to computer
2) Open app select com port
3) Select Device, if needed change baud
4) Press backup, you will have a backup file named ex. backup_2018_02_23.hex (backup_(Date).hex
5) Press flash.
6) If you dont like new firmware just reflash your backup_(Date).hex


Usage flash::

1) Connect Arduino board to computer
2) Open app select com port
3) Select Device, if needed change baud
4) Browse new firmware hex file
5) Press flash.

Adding new device is simple!

1) Open devices.txt
2) A device is a row in the file ex: Mega(ATMEGA2560);atmega2560;stk500v2;115200;
3)
Short name = Mega
Real device = (ATMEGA2560)
avrude.exe Partno = atmega2560
avrude.exe Programmer = stk500v2
avrude.exe Baudrate = 115200


Changes:

Changes 0.2 to 0.3
Fixed error handling, for flash and backup if not selecting com port and file to flash.

Changes 0.1 to 0.2
Testing functions, flash should work
Backup should work but you need to set all settings like device, com and baud to prevent app to crash
--
Changes 0.1
Building app
