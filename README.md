# Arduino LDR Smart Lighting System

An environmental light-sensing project utilizing a Photoresistor (LDR) to create a dual-function automated lighting system.

About : This project demonstrates how to read analog sensor data and use it for both logical thresholds and dynamic output scaling. A photoresistor is connected to analog pin A0 using a voltage divider circuit. The Arduino reads the ambient light luminosity (0-1023) and controls two LEDs. LED 1 (Pin 10) acts as a strict night light, turning ON digitally only when the light level drops below a defined threshold (330). LED 2 (Pin 11) acts as an adaptive smart light, utilizing Pulse Width Modulation (PWM) to continuously adjust its brightness inversely proportional to the ambient light—getting brighter as the environment gets darker.

Components :
* Arduino Uno
* 1 Photoresistor (LDR)
* 2 LEDs
* 1 Resistor (1kΩ) - For the LDR voltage divider
* 2 Resistors (220Ω) - For LED current limiting
* Breadboard
* Jumper wires

Wiring Connections :
**Photoresistor (LDR) Circuit:**
* **LDR Leg 1** to 5V on breadboard
* **LDR Leg 2** to Analog Pin A0 on Arduino board **AND** to GND via a 1kΩ resistor (Creates the voltage divider for analog reading)

**LEDs Circuit:**
* **LED 1 Anode (+)** to digital pin 10 on Arduino
* **LED 1 Cathode (-)** to GND via a 220Ω resistor
* **LED 2 Anode (+)** to digital pin 11 (PWM-capable pin) on Arduino
* **LED 2 Cathode (-)** to GND via a 220Ω resistor

Tools :
* Arduino IDE
* C/C++
* Tinkercad Circuits

A-QITAZ Mechatronics Engineering Student :)
