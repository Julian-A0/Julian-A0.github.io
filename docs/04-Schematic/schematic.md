---
Pressure Sensor Subsystem
---

## Overview

The pressure subsystem serves to detect any rapid drops or unusual changes in pessure within a water system. By taking an analog input, amplifying the signal and sending it to the Curiosity Nano Board JECK is able to determine the severity of the situation and output a digital alarm code to the speaker system. The schematic is broken down into four sections: A power supply and regulator combination, the current divider subsection, an amplification and analog pressure sensor subsection as well as a microcontroller processing unit. 

## Power Supply and Voltage Regulation

Within this subsection of the schematic a 9V AC-DC wall outlet adapter is used to bring in power to the Pressure subsystem. From this supply a MIC5211-LXYM6-TR dual voltage regulator converts the input voltage into 3.3V and 5V outputs. Decoupling capacitors are utilized to minimize the noise of the voltage input. The final result is a circuit subsection that can power the amplifier, Curiosity Nano Board and sensor.
![schematic](PSVR.png)

## Current Divider 

The output of the dual voltage regulator is 80 mA, however the input for the pressure sensor is 2mA. A current divider is necessary to redirect the difference in current out to ground while diverting 2 mA to the pressure sensor net. Given the input and output currents of the eletrical components the values of the resistors can be calculated using a simple current divider formula. An additional decoupling capacitor is included. 
![schematic](Currdiv.png)




