# instructions for using this circuit board (the "GBG-PCB") to build a go baby go car

questions? post [here](https://github.com/gobabygocarswithjoysticks/gbg-pcb/discussions/categories/questions-and-troubleshooting) or email gobabygocarswithjoysticks@gmail.com 

# Parts needed
* a car
* materials for frame and backrest (usually pvc pipe)
* joystick (recommended part: Radiolink joystick replacement for RC controllers AT9 and AT10 (get the “back to middle” type that springs back on both axes) )
* four wire cable - for joystick
* [3D printed joystick holder parts](https://github.com/gobabygocarswithjoysticks/index?tab=readme-ov-file#cad)
* an assembled GBG-PCB - make one using [these files](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/PCB_production), or email gobabygocarswithjoysticks@gmail.com I might have assembled boards to sell or donate to you. The components cost approximately $50 but it depends on quantity and shipping.
* an assembled [joystickpcb](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/joystickpcb)

# Tools needed
* flathead screwdrivers (large and small)
* wire cutters
* wire strippers
* micro USB cable (and USB hub if needed for your computer)

# Circuit diagram
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

## Fits a frame and has a way to connect a joystick
### Go Baby Go cars usually get a PVC pipe frame with a backrest
It's easier to fit a frame to a blockier car with more right angles
### The joystick can be connected to the frame, or it can be put on the end of an "adjustable photo arm"
[Here](https://github.com/gobabygocarswithjoysticks/index?tab=readme-ov-file#cad) are some 3D printed parts that could be used to hold the joystick

---

# Disconnect the battery
### If possible, disconnect one wire from the battery to keep the circuit off while you are working on it. Some cars have a spade terminal that has to be connected to the battery of a new car.

# Wire the PCB to the motors
## Find the motors
### The motors are usually under the seat of the car
## Prepare the motor wires
### Cut the wires to the motors
### Strip the insulation off the ends of the wires
## Connect the motors to the PCB
### The motors can be reversed or swapped left/right in software later.

# Wire the PCB to the battery

If there is a plug that comes from the battery and goes to a circuit board that is already in the car, you can probably cut that plug off and use those wires to power the GBG-PCB. 

If you see a fuse (usually a small black box with two wires coming out of it), please leave it in the circuit between the battery and the GBG-PCB.

Connect the positive battery wire (usually red) to the positive BATTERY terminal on the GBG-PCB (labeled "+"). 

Connect the negative battery wire (usually black) to the negative BATTERY terminal on the GBG-PCB (labeled "-"). 

The GBG-PCB has reverse voltage protection, so it won't be damaged if you accidentally connect the battery backwards, it just won't turn on.

### The PCB can be left connected to the battery. It does not need a switch between itself and the battery. The PCB has MOSFETs that stop electricity from flowing when the on/off switch is off. When the PCB is off it draws practically zero current (2 nanoAmps) so it will not make the battery discharge.

# Wire the PCB to the on/off switch
## Choose or add a switch to use as the main power on/off switch.
### Low currents (about 4 mA) will flow through this circuit, so any wires and switches will work.
## Connect the switch to the screw terminal labeled on/off.
### Current can flow either way through a switch so either wire from the switch can go to either terminal.
It doesn't matter for a switch (and I recommend just using a regular switch), but in case you're interested, the terminal closer to the battery is connected to the positive wire of the battery and the terminal closer to the left motor should be pulled to 12 Volts to turn the board on.
### An electrical connection between the two terminals of the on/off screw terminal block will turn the PCB on.

# Wire the Joystick

# (optional) Wire Buttons and/or Speed Knob

# Program the Pico
## Flash the firmware to the Pico
### This step is only needed if your GBG-PCB wasn't programmed when it was assembled and tested.

Go to [the go baby go programmer website](https://gobabygocarswithjoysticks.github.io/programmer/#new) and follow the instructions to upload code to a new car.

Select the PCB_gbg_program. If you don't see the PCB program, click on Advanced settings and check the box to get car code from the main branch.

## Connect
### Connect the GBG-PCB to your computer with a micro USB cable
### Go to [the go baby go programmer website](https://gobabygocarswithjoysticks.github.io/programmer/#configure)
### Follow the instructions pointed to with the magenta arrow to connect to the car
## Calibrate the joystick and adjust settings
### Click the "calibrate the joystick the easy way" button and follow the instructions on the screen
### You can also adjust the speed and acceleration settings for the car.

# Reconnect the battery
### If you disconnected a wire from the battery (or the car comes with a wire disconnected for shipping), reconnect it now.

# Test the car
## disconnect the car from the computer
## turn on the car using the on/off switch
### the three green lights on the PCB should turn on
### you should hear a short beep from the motors
## the car should drive when you move the joystick
### the blue light on the PCB should turn on when the car is moving and turn off when the joystick is centered

# Troubleshooting
