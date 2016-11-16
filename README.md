# esp301
python module to control Newport esp 301 stepper motion controller

Requirements
-------------
 - USB or Serial connection to ESP301.
 - PySerial module

Usage
-----
import esp
controller = esp.esp("/dev/ttyUSB0",19200,1) # newport controller device, baud rate, default axis 
controller.setpos(20.0,1)  # position, axis
controller.getpos(1) # axis

