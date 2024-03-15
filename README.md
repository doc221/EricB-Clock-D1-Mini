# EricB Clock ESP board
EricB has created a clock that uses MAX7219 dotmatrix and a lot of add-ons.
I have created a PCB (KiCad 8.0 format) that connects to the back of the matrix and has the possibilty to add the other components using simple pin headers.
Code is based on Arduine IDE and is also included.

For the EricB project, take a look at this [EricB Clock](https://www.hackster.io/ericBcreator/alarm-clock-with-web-interface-wake-up-light-temp-more-75dc6a)!
Code and my binary is also available here.

Enjoy and feedback is welcome.

## Pinout explanation
Here is what the pin assignment looks like.
#### Rotary
|Pinheader|Connection|To device|
|-|-|-|
|P1|GND|GND|
|P2|+5V|+5V|
|P3|D3|switch|
|P4|D2|pinB (data)|
|P5|D1|pinA (clock)|
#### MAX7219
|Pinheader|Connection|To device|
|-|-|-|
P1|+5V|+5V|
P2|GND|GND|
P3|D7|DIN (MOSI)|
P4|D8|CS|
P5|D5|CLK (SCK)|
#### Buzzer
|Pinheader|Connection|To device|
|-|-|-|
|P1|D4|First pin|
|P2|GND|Second pin|
#### PIR
|Pinheader|Connection|To device|
|-|-|-|
|P1|+5V|+5V|
|P2|GND|GND|
|P3|D0|sensor|
#### Neopixel
|Pinheader|Connection|To device|
|-|-|-|
|P1|+5V|+5V|
|P2|D6|DIN|
|P3|GND|GND|
#### Lightsensor GL5537
|Pinheader|Connection|
|-|-|
|P1|+5V|
|P2|A0 with resistor 120 Ohm to ground|

