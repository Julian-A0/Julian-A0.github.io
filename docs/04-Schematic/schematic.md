---
Pressure Sensor Subsystem
---

## Overview

This subsytem is design to support the JECK water leak detection system. Power is adapted using a barrel jack switch that is connected to a wall outlet. Voltage levels are then regulated to 5V and sent to the water pressure sensor. The water pressure sensor is utiilized to take in analog input, amplify the signal and feed it into the Curiosity Nano Board. A debugging LED and reset push button are included to aid in tracking issues in code and circuitry. If the pressure is categorized by the board's program as a leak a high settingo of 1 will be digitally outputted to trigger the alarm. 

## Subsystem Schematic Overview
![schematic](PressureSensorSubsystemSchematic.png)



