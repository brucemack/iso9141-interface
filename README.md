Overview
========
This is a KiCad project for a simple ISO-9141 interface board.  This allows a microcontroller to be interfaced to car's ISO-9141 (OBD2) port.

Please see related firmward projects.

Interfaces
==========

J1 is the connection to the vehicle
* Pin 1 - 12V battery power
* Pin 2 - KLINE
* Pin 3 - Ground

J2 is the connector to the microcontroller
* Pin 1 - Data receive (data from vehicle to controller)
* Pin 2 - Data transmit (data from controller to vehicle)
* Pin 3 - Control line which allow the KLINE to be pulled low for the purposes of signalling
* Pin 4 - 12V battery power
* Pin 5 - Ground

"# iso9141-interface" 
