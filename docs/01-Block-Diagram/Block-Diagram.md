## Overview
1) Input power is taken in through the 9V barrel jack. 
2) 9V input is converted to 5V using an LM7805T regulator.
   - This is done to appropriately power the Curiosity Nano board and water pressure sensor.
4) An analog pressure sensor is powered from this 5 V and take continous readings on the water pressure flowing the attached pipe.
5) The analog reading from the pressure sensor is fed into the Curiosity Nano's Analog to digital converter. 
6) The program coded onto the Curiosity Nano will determine the appropriate "bin" to categorize the sensor reading based on predetermined pressure levels.
   - These "bins" will categorize a safe or dangerous water pressure level.
7) Depending on the bin the system will digitally output 0 or 1 if the pressure is safe or dangerous.
   - A high setting of 1 indicates an irregularity and will prompt the alarm to turn on.
8) This cycle repeats while plugged in. 

## Pressure Sensor Block Diagram

![Example of Indivial Block diagram ](PressureSensorBlockDiagram.png)
