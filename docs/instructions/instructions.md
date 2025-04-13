# circuit diagram
![circuit diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/diagrams/circuit_diagram.drawio.png)

# Choose a Car
## 12 volts

The PCB will only work with 12 volt cars. It won't run on 6 volts.

The motor driver chips specify 8-40 volts [P_4.2.1](https://mm.digikey.com/Volume0/opasdata/d220001/medias/docus/781/IFX007T_Rev1.0_2018-02-21.pdf#G5.557706)

The voltage regulator for the Pico is rated for 9-18 volts [D78B05T-1.0](https://diwellshop.cafe24.com/web/DATASHEET/01_subtitle/4_POWER/2_DC-DC/D78B05T-1.0/D78B-1.0.pdf)

## Two motors

The car will be steered by controlling the two back wheels separately, so the car needs to have a motor for each wheel.

Cars with two speeds often have two motors in them.

Some cars are sold with one motor but have space in the frame to add a second motor. 
