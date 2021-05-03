# TOSLink Transceiver (Tool and Control Box)

## Overview

This repository contains the Autodesk Eagle schematic and layout for the TOSLink transceivers on the control box and the tools used by the MIT Bioinstrumentation Lab rover. 

For sending and receiving data to and from the tools over the TOSLink optic fiber cables, the TTL interface on a TinkerForge RS232 bricklet was used to communicate with an off-the-shelf TOSLink transceiver. This transceiver and the required external components were mounted on a custom PCB that easily meshed with the TTL breakout pins without needing any external wires and matched the RS232 bricklet footprint. In other words, this PCB could be mounted on top of the RS232 bricklet with only a couple of screws and male-female 12 mm long standoffs. The RS232 bricklet sends and receives data over the TTL/TOSLink interface at a serial baudrate of 115200 Baud.

The same TOSLink transceiver in the control box is mounted on a custom-made PCB board for the universal tool interface. It receives commands from the control box and returns data to be analyzed. The associated signal communication protocol is UART/USART/TTL, so the four output pins on the PCB correspond to power, ground, transmitter (TX), and receiver (RX). These pins can be accessed with most available four-pin connector housings. 

The `TOSLink Tool V2` and `TOSLink Transceiver V3` directories contain the layout and schematics for the transceiver mounted to the tool interface and the control box RS232 bricklet, respectively. 

## Contributors

#### Primary Contributors
Ryan Poon from the [MIT Bioinstrumentation Lab](https://bioinstrumentation.mit.edu/) is the primary contributor of this project.

#### Other Contributors
Professor Ian Hunter served as the main advisor.