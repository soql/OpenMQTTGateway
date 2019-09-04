# Compatible Modules for the RF Gateway:

|Module|Purpose|Where to Buy|
|-|-|-|
|SRX882|433Mhz Receiver|[compatible parts list](https://docs.google.com/spreadsheets/d/1_5fQjAixzRtepkykmL-3uN3G5bLfQ0zMajM9OBZ1bx0/edit#gid=1323184277)|
|STX882|433Mhz Transmitter|[compatible parts list](https://docs.google.com/spreadsheets/d/1_5fQjAixzRtepkykmL-3uN3G5bLfQ0zMajM9OBZ1bx0/edit#gid=1323184277)|
* or alternative XD RF 5V& FS1000A 

# Pinout
|Board| Receiver Pin| Emitter Pin|
|-|:-:|:-:|
|Arduino UNO|D3|D4|
|ESP8266|D2/D3/D1/D8|RX/D2|
|ESP32|27/26|12|
|RF BRIDGE|-|-|
|RF BRIDGE [DIRECT HACK](https://github.com/xoseperez/espurna/wiki/Hardware-Itead-Sonoff-RF-Bridge---Direct-Hack)|4|5|
|SONOFF RFR3|4|-|

# Arduino Hardware setup:
For NodeMCU pins are D4 (GPIO2) for receive and RX (GPIO3) for send.

Vcc pin of the Arduino, the RF Emitter and RF Receiver to a 5V supply source
Ground pins of the Arduino, the RF Receiver and RF Receiver to the ground of the supply source.

![RF](https://github.com/1technophile/OpenMQTTGateway/blob/master/img/OpenMQTTgateway_Arduino_Addon_RF.png)

# ESP8266 Hardware setup:

**If the gateway works only when serial monitor is connected don't use D3 use D2 instead (gpio 4) and modify config_RF.h accordingly.**

**With SRX882 some users reported that D3 is not working use D1 instead in this case and modify config_RF.h accordingly.**

Vcc pin of the ESP8266, the RF Emitter and RF Receiver to a 5V supply source
Ground pins of the ESP8266, the RF Emitter and RF Receiver to the ground of the supply source.

![Addon_RF](https://github.com/1technophile/OpenMQTTGateway/blob/master/img/OpenMQTTgateway_ESP8266_Addon_RF.png)

# ESP32 Hardware setup:

Vcc pin of the ESP32, the RF Emitter and RF Receiver to a 5V supply source
Ground pins of the ESP32, the RF Emitter and RF Receiver to the ground of the supply source.

![Addon_RF](https://github.com/1technophile/OpenMQTTGateway/blob/master/img/OpenMQTTgateway_ESP32_Addon_RF.png)

# SONOFF RF Bridge Hardware setup:
Per default there is no need on modifying the RF Bridge hardware, unless you don't want to use the provided RF controller (EFM8BB1). Indeed if you want to extend the protocols supported by the bridge you can [bypass this controller](https://github.com/xoseperez/espurna/wiki/Hardware-Itead-Sonoff-RF-Bridge---Direct-Hack) and use the ESP8255 capacities to decode RF Signal.
The processing can be achieved after the modification by either RF, RF2 or Pilight gateways.

# SONOFF RFR3 Hardware setup:
[Connect GPIO4 of the ESP8255 to the pin D0 of SYN470](https://1technophile.blogspot.com/2019/08/new-sonoff-rfr3-as-433tomqtt-gateway.html)
