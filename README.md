# arduino-esp8266

On https://github.com/igrr/Arduino/tree/ide-1.5.x-esp8266 there is a work-in-progress branch of the Arduino IDE targeting the ESP8266 platform. This means that you can run Arduino code on inexpensive modules like the ESP-01, without the need for an actual Arduino.

ESP-01 module
-------------

![module](https://cloud.githubusercontent.com/assets/2480569/5793940/15d3ec1e-9f59-11e4-8584-c4694501e420.jpg)

Solder VCC and CH_PD pin together (TODO: Check whether using a 1k pullup resistor changes the overall power consumption). Use a Prolific USB serial adapter to provide the 3.3V and GND, use another(!) serial adapter connected to the same USB hub (so that they share GND) to provide the RX and TX pins for the serial connection. This setup might not be the cleanest, but it is the quickest to get up and running. For programming, install a jumper between GND and GPIO0 as shown in the picture.
