Overview
========
This is a KiCad project for a simple ISO-9141 interface board.  This allows a microcontroller to be interfaced to car's ISO-9141 (OBD2) port.

Please see related firmware projects:

* [The OBDII Reader](https://github.com/brucemack/hello-obd2)
* [The ECU Simulator](https://github.com/brucemack/ecu-sim)

[Here is the official ISO standard document](https://cdn.standards.iteh.ai/samples/16737/e6b719fd44c345a792656f6d19e6cee4/ISO-9141-1989.pdf) that explains all of the details of this interface. What makes this interesting is that the transmit/receive to/from the vehicle all happens on a single wire.

Send any questions to bruce at mackinnon dot com.

Interfaces (V2)
===============

J1 is the connection to the vehicle:
* Pin 1 - 12V battery power
* Pin 2 - KLINE
* Pin 3 - Ground

J2 is the connector to the microcontroller:
* Pin 1 - Data transmit (data from controller to vehicle)
* Pin 2 - Data receive (data from vehicle to controller)
* Pin 3 - Control line which allow the KLINE to be pulled low for the purposes of signalling
* Pin 4 - An indicator LED that can be used by the controller
* Pin 5 - +5V regulated power for controller
* Pin 6 - Ground

Hardware
========

The V2 PCB:

![](images/v2pcb.jpg)

Here's what it looks like in real life (V1):

![](images/IMG_1681.jpg)

