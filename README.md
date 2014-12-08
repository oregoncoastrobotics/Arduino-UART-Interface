Arduino-UART-Interface
======================

Arduino UART Interface


This repository holds the code and info for the UART interface between our OS running processors and an arduino

The API works as outlined below, but is subject to change as we see fit:

all commands are ascii encoded comma seperated strings

- To change servo positions, send an "s" and then the position value for each servo in order.  Servos are connected to the digital pins of the arduino.  The connection for which pins connect to which servos happen in the arduino code itself (should we move this configuration up to the OS level?).

s,0,0,0,0,0,0,0,0
