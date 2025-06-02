
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

# Frame and Wheel Modifications
## Back wheels
## Front Caster Wheels
## PVC Frame
## Seatbelt

# Electrical Modifications

## Remove the Seat

## Disconnect the battery
### If possible, disconnect one wire from the battery to keep the circuit off while you are working on it. Some cars have a spade terminal that has to be connected to the battery of a new car.

## Wire the PCB to the motors

## Connect the PCB to the battery wires

The PCB can be left connected to the battery. It does not need a switch between itself and the battery. The PCB has MOSFETs that stop electricity from flowing when the on/off switch is off. When the PCB is off it draws practically zero current (2 nanoAmps) so it will not make the battery discharge.

## Wire the PCB to the on/off switch

### An electrical connection between the two terminals of the on/off screw terminal block will turn the PCB on.

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
