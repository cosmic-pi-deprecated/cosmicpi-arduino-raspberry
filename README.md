# cosmicpi-arduino-raspberry
NB. this is the firmware for V1 units, using the old output format. Not recommended for use.
Here is where we keep the binary files for Raspberry Pi because we can't compile using ARM cpu's (yet)
It can be uploaded using bossac as follows:
assuming you have bossac installed (Arduino comes with it, it's in /.arduino15/packages/arduino/tools/bossac/1.6.1-arduino for a typical installation. I'm using /dev/ttyACM0 which is a fairly standard default in Ubuntu. the file is the .bin.
```
sudo stty -F /dev/ttyACM0 1200; sudo stty stop /dev/ttyACM0;sudo ./bossac -i -d --port=ttyACM0 -U false -e -w -v -b cosmicpi-arduino.ino.arduino_due_x.bin -R
```

