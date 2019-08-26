# OpenMQTTGateway

## Overview

OpenMQTTGateway project goal is to concentrate in one gateway different technologies, decreasing by the way the number of proprietary gateways needed and hiding the different technologies singularity behind a simple & wide spread communication protocol; [MQTT](http://mqtt.org/).

OpenMQTTGateway support very mature technologies like basic 433mhz/315mhz protocols & infrared so as to make your old dumb devices "smart" and avoid you to throw then away. These devices have also the advantages of having a lower cost compared to Zwave or more sophisticated protocols.
And support also up to date technologies like Bluetooth Low Energy or LORA.

To have an overview of the supported PIR, door, water, smoke sensors, sirens, rings, beacons, switchs & weather stations you can take a look to the 
[compatible devices list](https://docs.google.com/spreadsheets/d/1_5fQjAixzRtepkykmL-3uN3G5bLfQ0zMajM9OBZ1bx0/edit#gid=2126158079)

MQTT enables you to connect easily a controller so as to monitor, control and automate scenarios.
The following controllers are compatible with MQTT:
* OpenHAB2
* Home Assistant
* Node Red
* FHEM
* Domoticz
* Jeedom

With OpenMQTTGateway and a controller you can for example:
* Monitor your garden with a Mi Flora sensor and control an irrigation valve depending on the soil moisture,
* Trigger a fan depending on the temperature and humidity thanks to a Mi Jia sensor,
* Alert yourself by a controller notification if the temperature of your fridge is too high,
* Detect your beacon/smartwatch so as to trigger a special scenario when you come home,
* Detect opened door or windows and alert yourself when leaving home
* Detect water leakage or smoke
* Actionate a siren if something is going wrong

The limit is your imagination 😀

!> **The material and information contained in this documentation is for general information purposes only. You should not rely upon the material or information on this documentation as a basis for making any business, legal or any other decisions. There is no warranty given on this documentation content. If you decide to follow the informations and materials given it is at your own risk.I will not be liable for any false, inaccurate, inappropriate or incomplete information presented on this blog.**

OpenMQTTGateway is not closed to one board or type of board, by using the power of the Arduino framework it let you many choice of hardware :
* Arduino UNO + W5100
* Arduino MEGA + W5100
* ESP8266: NodeMCU V1.0 NodeMCU V2.0, NodeMCU V3.0, ESP8266 12F and Wemos D1
* ESP32
* Sonoff RF bridge
* Sonoff Basic RFR3
You can take a look to the components sheet to have a view of [supported boards and components](https://docs.google.com/spreadsheets/d/1_5fQjAixzRtepkykmL-3uN3G5bLfQ0zMajM9OBZ1bx0/edit#gid=1323184277)

Moreover it supports also sensors; DHT, HC SR501, ADC, I2C bus, INA226, TSL2561
Or can actutate things.

Behind the scene you will find functionnalities dedicated to gateways like:
* Deduplication
* Simple and lite API
* Strong integrations with libraries used
* Signal forward/repeat
* First configuration with web portal
* Whitelist & Blacklist management

If you want to buy a coffee or other beverage so as to give me some support, here is a way to do it : 
<a href="https://www.buymeacoffee.com/1technophile" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
