# atmega32u4_devboard
Custom microcontroller with atmega 32u4 w/USB - C @ 2.0 speeds. Made to be compatible with arduino bootloader, and 0805 components for easy hand soldering

This project was one of my first pcb / embedded project, using refrence designs from sparkfun and arduino.cc I wanted a fast, easy to integrate us -  C microcontroller for quick sensor and electronic IC evaluation and testing. The atmega 32u4 was a primary canadite given its popularity in terms of documenation as the IC on the arduino leonardo and micro. And the ingrated USB 2.0 capabilities made layout and schematic work easier then for a atmega 328p (the IC on the arduino uno and nano - whcih requires a additional IC for usb -> serial communications)

Design Features:
  - USB - C receptacle
  - Analog and Digital IO
  - Arduino IDE / bootloader compatible
  - ICSP header pins for bootloader or non - arduino programming
  - 0805 components for easy hand-soldering

Design Issues:
  - No ground pours on either top or bottom layers, made routing more difficult then if GND plane was poured on the bottom layer
  - USB D+/D- was **not** routed differentially, caused usb connectivity isses
  - USB - C D+/D- pin were not connected on the pcb making receptacle only funciton when plugged into one side (This couldve been mitigated by using a "Dummy" usb C port with only 2.0, CC, D+/D- pins
  - Silkscreen intervened with vias due to size constraints with 0805 components

While not the best or most robust design, this project served as an oppurtunity to give an intro to pcb design fundamentals and embedded hardware

Schematic:
