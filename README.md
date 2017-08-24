Freetronics LibreSat Payload Processor Module
=============================================
Copyright 2013-2017 Freetronics Pty Ltd  
Freetronics site:  www.freetronics.com  
Freetronics email: info@freetronics.com  

A CubeSat payload board that incorporates 16 processor nodes for
running experiments, and a supervisor processor node to control
the experiment nodes.

A previous version of this board flew in space on ArduSat-X and
ArduSat-1.

Features:

 * 16 x processor nodes, each with an ATmega328P MCU
 * Each processor node runs the Arduino bootloader
 * 1 x supervisor node with an ATmega2561
 * Micro SD card slot connected to supervisor
 * All MCUs and sensors on a shared I2C bus
 * All I2C devices use bidirectional isolation circuits to allow continued operation of the system with failed devices
 * Processor node UARTs connected via multiplexers to the supervisor's first UART
 * 5V serial debug console with standard FTDI-style pinout on supervisor's second UART
 * Each processor node can be powered down independently by the supervisor
 * Each processor node can be reset using an I2C latch by the supervisor
 * Each MCU has an independent crystal for maximum reliability
 * TX, RX, and D13 LEDs on every processor node
 * Top and bottom temperature sensors on I2C bus with "disable" option to prevent address collisions
 * Requires external 5V and 3.3V supply
 * Current consumption monitoring of both power rails by the supervisor
 * Stackable CubeSat bus connectors
 * Conforms to CubeSat mechanical standards for dimensions and mounting
 * Selectable power bus connections
 * Optional I2C satellite bus pull-ups
 * I2C headers for spectrometer, Geiger counter, and bottom plate sensor assembly
 * GPS header with UART connections to node 11 via 3.3V level shifters
 * Switchable power supply to GPS header controlled by supervisor
 * Stackable CubeSat Bus connectors

Specifications:

 * Dimensions: 95.45mm x 90.3mm
 * PCB material: FR4 fibreglass (requires out-gassing before vacuum use)
 * PCB finish: ENIG (electroless nickel immersion gold) recommended
 * Module mass: 37 grams
 * Connector mass (pair): 15 grams
 * Total assembled mass including solder: 54 grams

More information is available at:

  http://www.freetronics.com.au/lsppm


INSTALLATION
------------
The design is saved as an EAGLE project. EAGLE PCB design software is
available from www.cadsoftusa.com free for non-commercial use. To use
this project download it and place the directory containing these files
into the "eagle" directory on your computer. Then open EAGLE and
navigate to the project. 


DISTRIBUTION
------------
The specific terms of distribution of this project are governed by the
license referenced below.


LICENSE
-------
Licensed under the TAPR Open Hardware License (www.tapr.org/OHL).
The "license" folder within this repository also contains a copy of
this license in plain text format.
