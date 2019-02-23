# Flight controller comparison

## Summary
||Pixhawk 2.1 Cube|Pixhawk 4|Pixhack v5|
|-|-|-|-|
|OSHW|Fully OSHW (altium design files incl)|schematics only|schematics only|
|JST-GH connectors|yes|yes|yes|
|price| $238 with GPS | $211 with GPS | $ 300 w/o GPS|
|case|plastic|plastic or aluminum| aluminum|
|modular MCU separate from IO board| yes|no|yes

## I/O allignment
Pixhack v5 has I/O on the sides rather than on top of the case which seems to be slightly more convenient for wiring.

![](https://docs.px4.io/assets/flight_controller/pixhack_v5/pixhack_v5.jpg)

![](https://docs.px4.io/assets/flight_controller/pixhawk4/pixhawk4_logo_view.jpg)

## Modular "cube" design
Pixhawk 2.1 and Pixhack v5 have modular design (similarly to Nvidia Jetson), allowing to incorporate the FCU on a custom IO motherboard at a later time.

## Open source 
Manufacturers of all boards claim to follow OSHW license, but only Pixhawk 2.1 actually released modifiable Altium schematics & board files. Pixhawk 4 and Pixhack released pdf schematics only

Pixhawk 2.1 design files

https://github.com/proficnc/The-Cube

https://github.com/3drobotics/Pixhawk_OS_Hardware


## MCU
Pixhawk 2.1 uses a 168MHz Cortex-M4 MCU whereas Pixhawk 4 and Pixhack v5 use faster Cortex-M7 MCUs. The speed is not a big concern - all of the MCUs allow running control loop @ 400Hz maximum.

