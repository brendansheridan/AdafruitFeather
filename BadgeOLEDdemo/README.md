# Adafruit Featherwing OLED Demo

A great project for getting started in the world of Arduino and the Adafruit Featherwing. This project is based on the [Adabox 003](https://www.adafruit.com/adabox003) which came with a Feather HUZZAH with ESP8266 WiFi board and a Featherwing OLED - 128x32 screen. The aim of this project is for beginner's like myself to learn data API's, data feeds, and Arduino. 

What's cooler than a computer smaller than a box of matches with a screen?

This repository contains files used for the Adafruit Featherwing OLED Demo that is [here](https://learn.adafruit.com/digital-display-badge?embeds=allow) .

## Pre-install Checklist
- Install all libraries necessary for the [Feather HUZZAH](https://learn.adafruit.com/adafruit-feather-huzzah-esp8266) board
- Add the following libraries within Arduino IDE. The [Adafruit MQTT](https://github.com/adafruit/Adafruit_MQTT_Library) library and  [Adafruit SSD1306](https://github.com/adafruit/Adafruit_SSD1306). These will be referenced in the code.

## Code modification
Within the code on the Adafruit site there is frequent mention of **PROGMEM**. Through a [troubleshooting session](https://forums.adafruit.com/viewtopic.php?f=57&t=114134&p=570426) it was made aware that PROGMEM is now an obsolete command. Simply remove this from the code from Adafruit or simply use the code I have available in this repository.

- Assuming you are using the provided code from this repository, you will only need to modify the following lines of code to fit your environment

	```
    //Wifi information
    const char* ssid     = "XXX";
    const char* password = "XXX";
 
    // Adafruit IO aka the data feed info
    #define AIO_SERVER      "io.adafruit.com"
    #define AIO_SERVERPORT  1883
    #define AIO_USERNAME    "XXX"
    #define AIO_KEY         "XXXX"
        
	```
	
When all is said and done, you should have a wearable badge that will hook into a data feed. Awesome!