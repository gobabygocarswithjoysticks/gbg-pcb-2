Use a GBG-PCB to make a Zupapa bumper car controlled by a joystick without needing to solder anything.

![bumper_car_photo.jpg](https://github.com/gobabygocarswithjoysticks/gbg-pcb/raw/main/docs/instructions/car-specific/zupapa-bumper-car/photos/photo0.jpg)

questions? post [here](https://github.com/gobabygocarswithjoysticks/gbg-pcb/discussions/categories/questions-and-troubleshooting) or email gobabygocarswithjoysticks@gmail.com 

# Parts needed
* a 12 volt Zupapa bumper car [https://www.amazon.com/dp/B0CLLW3FBG?th=1](https://www.amazon.com/dp/B0CLLW3FBG?th=1)
    * These instructions are written specifically for this model of car. Other cars may have different circuits and require different steps. If you are using a different model, take a look at these [general instructions for using this PCB](https://gobabygocarswithjoysticks.github.io/gbg-pcb/instructions/instructions). A GBG-PCB can control most cars as long as they are 12 volts.

* 3d printed parts

* an assembled [joystickpcb](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/joystickpcb) (I'll include these with any GBG-PCBs that I give out)
* an assembled GBG-PCB

{% include how-to-get-boards.md %}

# Tools needed
* wire strippers
* wire cutters
* small (3mm) flathead screwdriver
* large (6mm) flathead screwdriver
* small (2.0) Phillips screwdriver
* 

## ![circuit diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/zupapa-bumper-car/photos/circuit_diagram.drawio.png)


## [PCB Schematic](https://github.com/gobabygocarswithjoysticks/gbg-pcb/blob/main/schematic.pdf)
## [PCB List Of Components](https://github.com/gobabygocarswithjoysticks/gbg-pcb/blob/main/PCB_production/BOM.csv)

# Unpack the Car
![unpacked_car.jpg](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/zupapa-bumper-car/photos/unpacked_car.jpg)

# Connect Wheels

The following steps are assembly steps 1 and 2 in the Zupapa bumper car user manual "Install Car Wheels" and "Install Caster Wheels"

## Assemble the axis (Zupapa calls the axel the "axis" so I'll use their term)

Make sure both nuts are fully screwed on until the axis sticks out through them by a millimeter on both ends.

## Place the Axis assembly into the car

Turn the car upside down

## Attach the 2 motor covers with 2 small-head screws each

## Attach the 2 axis covers with 4 small-head screws each

## Attach the 2 universal (AKA swivel or caster) wheels with 4 large-head screws each


# Electrical Modifications
Turn the car back upright
## Remove the Seat and the Battery Cover

Unscrew the 2 screws holding the seat in place and lift it off. Then, unscrew the screw on the white wire holder and the 4 screws holding the battery cover in place and remove the cover.

## Disconnect the battery
It should be shipped with the red wire to the battery already disconnected. If a wire is connected to the red terminal of the battery, disconnect it to keep the car off and safe while you work on it.

Put tape over the red terminal of the battery to prevent accidental short circuits.

## Connect the GBG-PCB
### Identify all the wires
Find the white wire going to the 9 wire plug on the control box. Cut the white wire close to the plug.

Strip a quarter inch (6 mm) of insulation off the end of the white wire, put it into the 

### Connect the PCB to the battery wires
_The PCB can be left connected to the battery. It does not need a switch between itself and the battery. The PCB has MOSFETs that stop electricity from flowing when the on/off switch is off. When the PCB is off it draws practically zero current (2 nanoAmps) so it will not make the battery discharge._

Cut the red battery wire close to the fuse. Strip 3/8" (10 mm) of insulation off the end of the red wire. Connect the red battery wire to the positive large BATTERY screw terminal on the GBG-PCB (labeled "+"). Tighten the screw terminal tightly to hold the wire in place.

Cut the black battery wire where it connects to the battery plug. Strip 3/8" (10 mm) of insulation off the end of the black wire. 

Cut the thin black wire off the 6 wire plug. Strip 3/8" (10 mm) of insulation off the end of the black wire.

Put both the black battery wire and the thin black wire from the 6 wire plug into the negative large BATTERY screw terminal on the GBG-PCB (labeled "-"). Tighten the screw terminal securely to hold both wires in place.

### Wire the PCB to the on/off switch

### Wire the PCB to the motors

### Add the wires for the joystick

## Connect the joystick



## (optional) Wire Buttons and/or Speed Knob
### Buttons
Plug up to 4 buttons into the headphone-style jacks on the GBG-PCB.

When you connect the GBG-PCB to your computer to change the settings, click the "show all" button and check the box next to "enable button ctrl". Then, you can set what direction each button should make the car move in.

### Speed Knob
You can add a knob to the car for easily adjusting the maximum speed of the car without needing to reprogram it.

Connect a potentiometer to the 3 screw terminals labeled "speed knob". 

When you connect the GBG-PCB to your computer to change the settings, click the "show all" button and check the box next to "use speed knob".

## Reconnect the battery
The cars are sold with a red wire disconnected from the battery to keep the car from turning on during shipping. This also made it safer to work on the electrical system. Now that you're done with the wiring, you can connect the wire to the battery.

# Software and Settings
## Flash the firmware to the Pico
If you got your GBG-PCB from someone who already programmed it for you, then you can skip ahead to calibrating the joystick and adjusting settings.

Go to [the go baby go programmer website](https://gobabygocarswithjoysticks.github.io/programmer/#new) and follow the instructions to upload code to a new car. Select the __PCB_gbg_program__ not the standard __gbg_program__.

## Connect
### Connect the GBG-PCB to your computer with a micro USB cable
### Go to [the go baby go programmer website](https://gobabygocarswithjoysticks.github.io/programmer/#configure)
### Follow the instructions pointed to with the magenta arrow to connect to the car
## Calibrate the joystick and adjust settings
### Click the "calibrate the joystick the easy way" button and follow the instructions on the screen
### You can also adjust the speed and acceleration settings for the car.

# Test the car
## disconnect the car from the computer
## turn on the car using the on/off button on the dashboard
### the three green lights on the PCB should turn on
### you should hear a short beep from the motors
## the car should drive when you move the joystick
### the blue light on the PCB should turn on when the car is moving and turn off when the joystick is centered
### if the blue light blinks quickly that means the joystick needs to be left centered for a few seconds before trying to move and that the joystick may need to be recalibrated


# frame
// TODO
# seatbelt and backrest
// TODO



### Congratulations! You're done!

# Check your work
Check your work with this [inspection checklist]() #TODO

# Troubleshooting

## If you would like help troubleshooting your car or if you have any questions, please email gobabygocarswithjoysticks@gmail.com

# The car doesn't drive in the direction the joystick is pointing in
#### follow these steps to reprogram the car if it drives in the wrong direction:
### 0. Connect the programmer website and calibrate the joystick
### 1. If moving the joystick forwards makes the car spin, use the website to reverse the motor that the car turned towards (show all the settings then press the reverse motor button next to the "motor fast" setting)
### 2. If moving the joystick forwards makes the car drive backwards, use the website to reverse both motors
### 3. If the car spins the opposite direction from the direction that the joystick is points, use the website to swap the motors, then repeat the 3 steps starting at step 1
# The car doesn't drive
## if the blue light blinks quickly
### that means the joystick needs to be left centered for a few seconds before trying to move (this is a safety feature)
#### Let go of the joystick for 5 seconds and wait for the light to stop blinking
### it could also mean that the joystick needs to be recalibrated
#### If the blue light continues to blink quickly after letting go of the joystick for 5 seconds, then you should recalibrate the joystick using the programmer website. Connect the GBG-PCB to your computer, go to the programmer website, connect the website to the GBG-PCB, then click the "calibrate the joystick the easy way" button and follow the instructions on the screen.
## if none of the green lights on the PCB turn on,
#### the battery might have been connected backwards. A backwards connection does not damage the board; the board just doesn't turn on.
#### the on/off switch might not be wired correctly
#### the battery might need to be charged
