# Thermal-feedback-display-with-Peltier-Elements-on-Arduino
A temperature feedback device with PID controller

This program is for a thermal feedback module built on Arduino.
In this design, two 5V TEC peltier modules (https://www.adafruit.com/product/1331) are placed back to back to achieve heating and cooling on the same surface. 
A heatsink is attached (using thermal tape) to the other end of the cooler element. Two N-MOSFETs are required to power these through the Arduino.
The desired temperature is received via serial input.
A TMP36 temperature sensor is used to regulate temperature by feeding back to a PID controller. 
The PID controller has two sets of coeffcicents for the heater and the cooler because the cooling element is further away from the target surface. The controller direction is also reversed for cooling.
The TMP36 circuit should be grounded separately from the peltier elements to avoid interference.

An image of the module is attached here. A schematic of the circuit will be uploaded later.
