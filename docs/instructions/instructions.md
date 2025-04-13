# instructions for using this PCB to build a go baby go car

questions? post [here](https://github.com/gobabygocarswithjoysticks/gbg-pcb/discussions/categories/questions-and-troubleshooting) or email gobabygocarswithjoysticks@gmail.com 

# parts needed
* a car
* materials for frame and backrest (usually pvc pipe)
* joystick (recommended part: Radiolink joystick replacement for RC controllers AT9 and AT10 (get the “back to middle” type that springs back on both axes) )
* [3D printed joystick holder parts](https://github.com/gobabygocarswithjoysticks/index?tab=readme-ov-file#cad)
* an assembled GBG-PCB
* a joystickpcb

# circuit diagram
![circuit diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/diagrams/circuit_diagram.drawio.png)

---

# Choose a Car
## 12 volts
### The PCB will only work with 12 volt cars. It won't run on 6 volts.

The motor driver chips specify 8-40 volts [P_4.2.1](https://mm.digikey.com/Volume0/opasdata/d220001/medias/docus/781/IFX007T_Rev1.0_2018-02-21.pdf#G5.557706)

The voltage regulator for the Pico is rated for 9-18 volts [D78B05T-1.0](https://diwellshop.cafe24.com/web/DATASHEET/01_subtitle/4_POWER/2_DC-DC/D78B05T-1.0/D78B-1.0.pdf)

## Two motors
### The car will be steered by controlling the two back wheels separately, so the car needs to have a motor for each wheel.

Cars with two speeds often have two motors in them.

Some cars are sold with one motor but have space in the frame to add a second motor. 

## Able to (be modified to) spin in place
### Some models already can spin in place ("bumper cars")
### For most cars, you'll need to remove the front wheels and add swivelling caster wheels.

## fits a frame and has a way to connect a joystick
### Go Baby Go cars usually get a PVC pipe frame with a backrest
It's easier to fit a frame to a blockier car with more right angles
### The joystick can be connected to the frame, or it can be put on the end of an "adjustable photo arm"
[Here](https://github.com/gobabygocarswithjoysticks/index?tab=readme-ov-file#cad) are some 3D printed parts that could be used to hold the joystick

---
