# Instructions for using this circuit board (the "GBG-PCB") to build a go baby go car

questions? post [here](https://github.com/gobabygocarswithjoysticks/gbg-pcb/discussions/categories/questions-and-troubleshooting) or email gobabygocarswithjoysticks@gmail.com 

# Parts needed
* a car
* materials for frame and backrest (usually pvc pipe)
* joystick (recommended part: Radiolink joystick replacement for RC controllers AT9 and AT10 (get the “back to middle” type that springs back on both axes) )
* four wire cable - for joystick
* [3D printed joystick holder parts](https://github.com/gobabygocarswithjoysticks/index?tab=readme-ov-file#cad)
* an assembled [joystickpcb](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/joystickpcb)
* an assembled GBG-PCB
1. make one using [these files](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/PCB_production),
2. email gobabygocarswithjoysticks@gmail.com. I might have assembled boards to sell or donate to you. The components cost approximately $50 but it depends on quantity and shipping.
3. use [this PCBWay link]() to order fully assembled boards

# Tools needed
* flathead screwdriver (3mm)
* wire strippers/cutters
* micro USB cable

# Circuit diagram
![circuit diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/diagrams/circuit_diagram.drawio.png)

## [PCB Schematic](https://github.com/gobabygocarswithjoysticks/gbg-pcb/blob/main/schematic.pdf)
## [PCB List Of Components](https://github.com/gobabygocarswithjoysticks/gbg-pcb/blob/main/PCB_production/BOM.csv)

---

# Choose a Car
## 12 volts
It won't run on 6 volts, the motor driver ICs need over 8 volts.

It hasn't been tested above 12 Volts.

The PCB was only designed for 12 Volt ride on cars. Feel free to email if you are interested in trying it at other voltages. The motor drivers can easily handle 24 volts, but the 5V regulator and some of the resistors would need to be changed.

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

If you see a fuse (usually a small black box with two wires coming out of it), please leave it in the circuit between the battery and the GBG-PCB. It's a really good idea to have a fuse between the battery and the PCB; if you need to get a fuse, a 20 Amp auto resetting fuse is a reasonable choice.

Connect the positive battery wire (usually red) to the positive BATTERY terminal on the GBG-PCB (labeled "+"). 

Connect the negative battery wire (usually black) to the negative BATTERY terminal on the GBG-PCB (labeled "-"). 

The GBG-PCB has reverse voltage protection, so it won't be damaged if you accidentally connect the battery backwards. It just won't turn on.

### The PCB can be left connected to the battery. It does not need a switch between itself and the battery. The PCB has MOSFETs that stop electricity from flowing when the on/off switch is off. When the PCB is off it draws practically zero current (2 nanoAmps) so it will not make the battery discharge.

# Wire the PCB to the on/off switch
## Choose or add a switch to use as the main power on/off switch.
### Low currents (about 4 mA) will flow through this circuit, so any wires and switches will work.
## Connect the switch to the screw terminal labeled on/off.
### Current can flow either way through a switch so either wire from the switch can go to either terminal.
It doesn't matter for a switch (and I recommend just using a regular switch), but in case you're interested, the terminal closer to the battery is connected to the positive wire of the battery and the terminal closer to the left motor should be pulled to 12 Volts to turn the board on. The MOSFETs interrupt the connection to the negative wire of the battery.
### An electrical connection between the two terminals of the on/off screw terminal block will turn the PCB on.

# Wire the Joystick
![joystick photo](https://github.com/gobabygocarswithjoysticks/gbg-pcb/raw/main/photos/joystick.jpg)
The wires between the joystickpcb and the GBG-PCB would be a longer 4 wire cable when installed in a car.
# (optional) Wire Buttons and/or Speed Knob
TODO 
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
### if the blue light blinks quickly that means the joystick needs to be left centered for a few seconds before trying to move and that the joystick may need to be recalibrated

# Troubleshooting
# The car doesn't drive in the direction the joystick is pointing in
#### follow these steps to reprogram the car if it drives in the wrong direction:
### 0. Connect the programmer website and calibrate the joystick
### 1. If moving the joystick forwards makes the car spin, use the website to reverse the motor that the car turned towards (show all the settings then press the reverse motor button next to the "motor fast" setting)
### 2. If moving the joystick forwards makes the car drive backwards, use the website to reverse both motors
### 3. If the car spins the opposite direction from the direction that the joystick is points, use the website to swap the motors, then repeat the 3 steps starting at step 1
# The car doesn't drive
## if the blue light blinks quickly
#### that means the joystick needs to be left centered for a few seconds before trying to move and that the joystick may need to be recalibrated
## if none of the green lights on the PCB turn on,
#### the battery might have been connected backwards (the PCB is not damaged)
#### the on/off switch might not be making a connection
