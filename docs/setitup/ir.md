# Compatible parts for the IR Gateway:
* IR Gateway: an infrared diode for emitting
* IR Gateway: a transistor 2N2222
* IR Gateway: a 330 ohms resistor (connecting to Pin 9)
* IR Gateway: a 220 ohms resistor (limit current to LED)
* IR Gateway: an infrared receiver

The IR setup can work with bc547 and a 4x3 LED-Matrix.

# Pinout
|Board| Receiver Pin| Emitter Pin|
|-|:-:|:-:|
|Arduino UNO|D2|D9|
|ESP8266|D4|D0|
|ESP32|27|14|

# Arduino Hardware setup
Vcc pin of the Arduino, the IR Emitter and IR Receiver to a 5V supply source
Ground pins of the Arduino, the Transistor and IR Receiver to the ground of the supply source.

![IR](https://github.com/1technophile/OpenMQTTGateway/blob/master/img/OpenMQTTgateway_Arduino_Addon_IR.png)

# ESP8266 Hardware setup
![IR](https://github.com/1technophile/OpenMQTTGateway/blob/master/img/OpenMQTTgateway_ESP8266_Addon_IR.png)
