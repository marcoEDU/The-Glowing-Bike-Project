# The Glowing Bike Project

Upgrade your bike with LEDs, raibows and turn signals.

Want to support the development financially? Donations are always welcomed! 
[Click here to donate on Liberapay](https://liberapay.com/marcoEDU)

[<img src="http://img.shields.io/liberapay/receives/marcoEDU.svg?logo=liberapay">](https://liberapay.com/marcoEDU)

## Features

- Turn left & right animation
- Rainbow animation
- Safe driving animation


## Requirements

### Hardware

- your bike
- 1x ESP8266 or ESP32 (for example NodeMCU)
- 3x WS2812B LED strips with waterproof protection
- 3x USB to MicroUSB cables with switch to turn on/off power
- 2x Toggle switches
- 1x external battery with 3 or more USB ports
- a bunch of longer cable ties
- tape
- soldering iron, solder
- cables, to connect LED strips, Toggle switches, USB power cables and ESP
- fur fabric


### Software

- Python 3
- this repo
- latest MicroPython for your [ESP8266](http://micropython.org/download/esp8266/) or [ESP32](http://micropython.org/download/esp32/) (.bin file)


## How to upgrade your bike

### Software

-  Install MicroPython [on your ESP8266](https://docs.micropython.org/en/latest/esp8266/tutorial/intro.html) or [your ESP32](https://docs.micropython.org/en/latest/esp32/tutorial/intro.html#esp32-intro)
- copy latest [neopixel_plus.py](https://github.com/marcoEDU/NeoPixelPlus/blob/master/neopixel_plus/neopixel_plus.py) to the main directory of your ESP using the WebREPL.
- create 'functions' folder on ESP, with all files from the ['functions' folder of The Glowing Bike Project](https://github.com/marcoEDU/The-Glowing-Bike-Project/tree/master/functions)
- copy 'main.py' and 'bike.py' to main directory


### Hardware

- tape one LED strip to the back of your bike, one to the center part and one at the front of your bike
- for each LED strip solder the LED strip power and ground to the power and ground of one of the USB cables with a switch in the middle (on Micro USB side) - and connect the power and ground of the ESP to the USB cable with the least amount of LEDs connected
- solder the data cables of the LED strips to the ESP (GPIO 13 for the front LEDs, GPIO 12 for the center LEDs and GPIO 14 for the back LEDs)
- connect the USB cables with the external battery and fix the battery on the back of your bike
- fix the toggle switches to your bike handlebar at the front (using tape and cable ties) and solder it to the ESP (use GPIO 3 for the data pin of theleft switch, GPIO 1 for the right switch)
- once you connected all the electronics, cut out pieces of fabric to cover the cables connecting the front LED strip and switches, cover the bike with your fabric and make sure the LEDs aren't covered with the fabric
- fix the fabric, LED strips and wires using cable ties

Done! Turn on all three switches and you are ready to drive:)