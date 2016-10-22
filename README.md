# October 2016 Electronics for Inventors ESP8266 class

These instructions reside on github: https://github.com/hydronics2/ESP8266---Oct-2016-PCC-Class

We'll be programming the ESP8266 wifi chip.  It is packaged on the sparkfun dev board: https://www.sparkfun.com/products/13711

Your boards are pre-programmed as wifi hot spots. Try connecting to your board with your phone and trying these pages:
http://192.168.4.1/index.html  this controls the blue onboard LED

http://192.168.4.1/smoothie.html  this page is not yet connected to your arduino but hopefully will be soon.

Install Arduino 1.6.11 from here: https://www.arduino.cc/en/Main/OldSoftwareReleases#previous

Follow the directions by sparkfun to add the json board files from the Arduino Board Manager menu: https://learn.sparkfun.com/tutorials/esp8266-thing-development-board-hookup-guide/setting-up-arduino

Create a directory in your My Documnets called Arduino.  Add the esp8266fs.jar file to the directory Arduino/tools/ESP8266FS/tool/esp8266fs.jar
This file allows you to upload html and js data files to your Arduino. There are no folders though. The file is here:https://github.com/esp8266/arduino-esp8266fs-plugin/releases/tag/0.2.0


The 192.168.4.1/index.html file contains buttons that trigger XMLHttpRequest() to the ESP8266 Arduino code and adjust LED button speed. 

The 192/168.4.1/soothie.html file contains a small javascript library for graphing: http://smoothiecharts.org/

Small is important as there are memory constraints. Here is a description of how the memory is allocated for FS file systems: https://github.com/esp8266/Arduino/blob/master/doc/filesystem.md

There is a list of micro javascript libraries here: http://microjs.com/#

Here are some Arduino Learning resources: http://www.pcc.edu/staff/index.cfm/1514,13821,30,html 
