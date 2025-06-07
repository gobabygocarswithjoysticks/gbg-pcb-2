aosom jeep
box cutter for opening box
wire cutter
wire stripper
clamps
screw driver with phillips head
pvc glue


# Parts needed
* an Aosom jeep (Aosom SKU: 370-038)
* materials for frame and backrest (usually pvc pipe) //TODO: ADD DETAILS
* Radiolink joystick replacement for RC controllers AT9 and AT10 (get the “back to middle” type that springs back on both axes)
* four wire cable - for joystick
* //TODO
* [3D printed parts](https://github.com/gobabygocarswithjoysticks/index?tab=readme-ov-file#cad) (handles, joystick holder)
* an assembled [joystickpcb](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/joystickpcb)
* an assembled GBG-PCB
{% include how-to-get-boards.md %}
# Tools needed //TODO
* flathead screwdriver (3mm)
* wire strippers/cutters
* micro USB cable

# Circuit diagram
![circuit diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/diagrams/circuit_diagram.drawio.png)

## [PCB Schematic](https://github.com/gobabygocarswithjoysticks/gbg-pcb/blob/main/schematic.pdf)
## [PCB List Of Components](https://github.com/gobabygocarswithjoysticks/gbg-pcb/blob/main/PCB_production/BOM.csv)

---

#### note: some photos are of a white Jeep, some are of a green Jeep. Please just ignore the color changes, the two cars are otherwise identical.

# Unpack the Jeep (Parts to Keep)

### 201: Back wheels

### 202: Back axle (attached to steering mechanism)

### 203: Front bar (attached to steering mechanism) 

### 204: Grey reinforcement pieces 

### 205: Seat 

### 206: Little plastic wrenches 

### 207: Bags of nuts, bolts, and screws 

### 208: Back motors 

### 209: Motor covers 

### 210: Charger 

### 211: Driving lights 

### 212: Toolbox 

### 213: Auxiliary cord for music 

### 214: Manual

![Jeep parts photo.jpg](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/jeep parts.jpg)

Parts of the Jeep not shown in the image can be discarded.

# Frame and Wheel Modifications
## Back wheels
Remove all nuts and washers from the back axle (202).

Slide the back axle into place as shown below.

![back axle photo](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/back axle photo.jpg)

Install back motors (208), back wheels (201), spacers (207), nuts (207) (tighten the nuts on the two ends of the axle, 202, simultaneously), and hubcaps (207) as shown in the manual (214, image below). Use the provided plastic wrenches. Make sure to check the labels on the motors that say L or R and put the L motor on the side of the car that will be on the left side when the car is upright from the perspective of the driver, and put the R motor on the right side of the car. If the motors are on the wrong sides the car will drive backwards.

![back axle diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/back wheels.jpg)


## Front Caster Wheels
The front steering motor will not be used. The motor is on the underside of the car. Unplug the wires to the motor. Unscrew the motor, remove and discard.

![front steering motor](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/front steering motor.jpg)

Unscrew the locknuts from the metal steering mechanism to remove the front bar (203) and use a clamp to securely hold the front bar for cutting the welds on it, in the next step.

Remove the round tubes on the front bar by using the dremel and a cutting wheel to cut through the welds that hold the tubes in place. (Try to maintain the structural integrity of the square bar while cutting; the round tubes will be disposed of, so damaging them while cutting is acceptable.) After the welds are cut, use a hammer to tap the tubes out if necessary (making sure to hammer from the side of the tube OPPOSITE the weld).

Place the casters (1) into the holes in the bar (where the tubes were), with washers (2) on both sides of the hole. Bolt the casters to the bar using ½-13 lock nuts (3), using a large channel lock pliers to keep the caster from spinning while turning the nut with a ¾” wrench. Make sure that the casters are not installed upside-down; mounting tabs on the bar should be on the wheel side.

Use screws (207) found in the Jeep parts to screw the front bar to the Jeep.


## PVC Frame
Cut the 10 foot length of 3/4 inch PVC pipe to the following lengths, as also shown in the diagram below:
* 2x 26.5" pieces
* 1x 14.5" piece
* 2x 13" pieces
* 2x 7.5" pieces
* 1x 5" piece
* 2x 3" pieces

![pvc frame diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/pvc frame.png)

Join the two parts of each 3D printed saddle tee (106, 107) together, using five m2.2x14mm screws (14).

// TODO: 

## Seatbelt

# Electrical Modifications

## Remove the Seat

## Disconnect the battery
### If possible, disconnect one wire from the battery to keep the circuit off while you are working on it. Some cars have a spade terminal that has to be connected to the battery of a new car.

## Get ready to add the PCB

Remove the control box that came with the car. Unscrew the screw securing it and unplug all wires that are connected to it. The control box is not needed and can be discarded. Keep the Y branching cable that connects the two motors to the control box, as it will be used to connect the motors to the GBG-PCB.

Find the left motor plug, the battery plug, the right motor plug, the 6 wire plug and the steering motor plug.

Gently pull on the steering motor plug and discard the brown and blue steering motor wires. The other end was unplugged when you removed the steering motor. The steering motor wires are not needed. You can cut any heatshrink tubing that is around the steering motor plug or even the steering motor wires themselves, if needed, to remove the steering motor wires.

![all the plugs.jpg](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/all the plugs.jpg)

## Connect the PCB to the battery wires

The PCB can be left connected to the battery. It does not need a switch between itself and the battery. The PCB has MOSFETs that stop electricity from flowing when the on/off switch is off. When the PCB is off it draws practically zero current (2 nanoAmps) so it will not make the battery discharge.

Cut the red battery wire where it connects to the battery plug. Strip 3/8" (10 mm) of insulation off the end of the red wire. Connect the red battery wire to the positive large BATTERY screw terminal on the GBG-PCB (labeled "+"). Tighten the screw terminal securely to hold the wire in place.

Cut the black battery wire where it connects to the battery plug. Strip 3/8" (10 mm) of insulation off the end of the black wire. 

Cut the thin black wire off the 6 wire plug. Strip 3/8" (10 mm) of insulation off the end of the black wire.

Put both the black battery wire and the thin black wire from the 6 wire plug into the negative large BATTERY screw terminal on the GBG-PCB (labeled "-"). Tighten the screw terminal securely to hold both wires in place.

## Wire the PCB to the on/off switch

Cut the thin white wire off the 6 wire plug. Strip 1/4" (6 mm) of insulation off the end of the white wire. Connect the white wire to the left side of the ON/OFF screw terminal on the GBG-PCB. It's important that the white wire is connected to the side of the on/off switch that is closer to the left motor screw terminal. The white wire should go to the side of the on/off screw terminal that is closer to the word "off" than the word "on" where it says "on/off" on the PCB.

Cut the thin red wire off the 6 wire plug. Strip 1/4" (6 mm) of insulation off the end of the red wire. Connect the red wire to the small batt screw terminal on the GBG-PCB (labeled "+").

## Wire the PCB to the motors

Cut the two wires for the left motor off the left motor plug. Strip 3/8" (10 mm) of insulation off the ends of the two wires.

## Wire the Joystick



## (optional) Wire Buttons and/or Speed Knob
### Buttons
Plug up to 4 buttons into the headphone-style jacks on the GBG-PCB.

When you connect the GBG-PCB to your computer to change the settings, click the "show all" button and check the box next to "enable button_ctrl". Then, you can set what direction each button should make the car move in.
### Speed Knob
You can add a knob to the car for easily adjusting the maximum speed of the car without needing to reprogram it.

Connect a potentiometer to the screw terminal labeled "speed knob". When you connect the GBG-PCB to your computer to change the settings, click the "show all" button and check the box next to "use speed knob".

## Reconnect the battery

# Software and Settings
## Flash the firmware to the Pico
If you got your GBG-PCB from someone who already programmed it for you, then you can skip ahead to calibrating the joystick and adjusting settings.

Go to [the go baby go programmer website](https://gobabygocarswithjoysticks.github.io/programmer/#new) and follow the instructions to upload code to a new car.

Select the PCB_gbg_program. If you don't see the PCB program, click on Advanced settings and check the box to get car code from the main branch.

## Connect
### Connect the GBG-PCB to your computer with a micro USB cable
### Go to [the go baby go programmer website](https://gobabygocarswithjoysticks.github.io/programmer/#configure)
### Follow the instructions pointed to with the magenta arrow to connect to the car
## Calibrate the joystick and adjust settings
### Click the "calibrate the joystick the easy way" button and follow the instructions on the screen
### You can also adjust the speed and acceleration settings for the car.

# Test the car
## disconnect the car from the computer
## turn on the car using the on/off switch
### the three green lights on the PCB should turn on
### you should hear a short beep from the motors
## the car should drive when you move the joystick
### the blue light on the PCB should turn on when the car is moving and turn off when the joystick is centered
### if the blue light blinks quickly that means the joystick needs to be left centered for a few seconds before trying to move and that the joystick may need to be recalibrated


# Finishing Touches
## re-attach the seat

# Notes on remote control 
## Over wifi
This feature is available on GBG-PCBs with a Pico 1W or 2W.

Check the "use wifi" setting on the programmer website, then follow the instructions and QR codes on the programmer website.

The Pico will create a wifi network and will serve a webpage that allows you to control the car.

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
#### the battery might have been connected backwards. A backwards connection does not damage the board; the board just doesn't turn on.
#### the on/off switch might not be making a connection
