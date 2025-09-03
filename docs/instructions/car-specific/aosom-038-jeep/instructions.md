![jeep_photo.jpg](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/jeep_photo.jpg)

questions? post [here](https://github.com/gobabygocarswithjoysticks/gbg-pcb/discussions/categories/questions-and-troubleshooting) or email gobabygocarswithjoysticks@gmail.com 

# Parts needed
* an Aosom jeep (Aosom SKU: 370-038, I also see an identical looking car on costzon.com)
* [2x 5” caster w/ 1/2”-13 x 1-1/2” threaded stem and “No Brake” option](https://www.sescasters.com/product/cr26l05sx0x-rpfggnx/)
* 4x washer with 1/2" inner diameter
* 2x 1/2"-13 lock nuts
* Radiolink joystick replacement for RC controllers AT9 and AT10 (get the “back to middle” type that springs back on both axes)
* 4.5’ length of four-wire ribbon cable
* 2x 4-40 nut
* 2x 4-40 1.25 inch machine screw with phillips head
* 12” of 1/4 split loom plastic wire protector tube
* [18x m2.2x14mm screws](https://www.mcmaster.com/95893A174/)
* 10 foot length of 3/4 inch schedule 40 PVC tubing
* 2x 1/4-20 locknut
* 2x 1/4-20 3/4 inch machine screw with rounded head
* 8x 3/4 inch PVC pipe 90 degree elbows
* 4x 2 inch long #6 wood screws (for attaching the frame to the car)
* 4x plywood chunks (about 1 inch by 1.5 inches by 2 inches)
* 3/4” x 1 3/4” piece of 1/16” rubber gasket sheet
* 2x large zip ties
* harness or seatbelt or velcro or foam kickboard (any supplies needed to make a backrest and provide enough support for the child to sit in the car. the harnesses we used to use are out of stock)

* [3D printed parts](https://github.com/gobabygocarswithjoysticks/index?tab=readme-ov-file#cad) (3 handles, 3 joystick holder components)
* an assembled [joystickpcb](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/joystickpcb) (I'll include these with any GBG-PCBs that I give out)
* an assembled GBG-PCB

{% include how-to-get-boards.md %}

# Tools needed
* small flathead screwdriver (3mm)
* flathead screwdriver (larger)
* small phillips head screwdriver (2.0)
* phillips head screwdriver bit for a drill or electric screwdriver
* screwdriver bit for a drill or electric screwdriver that fits the wood screws
* wire strippers
* wire cutters
* micro USB cable
* box cutter
* clamps
* rotary tool (Dremel) with cutting wheel
* hammer
* pvc glue
* T6 Torx screwdriver
* duct tape that matches the color of the car
* permanent marker (or label maker)
* hot glue
* drill
* 1/16" drill bit (for drilling holes in the 3D printed parts)
* 5/64" drill bit (for drilling pilot holes for the wood screws for the frame)
* 3/32" drill bit (for drilling out the holes in the joystick handles)
* adjustable wrench (at least 3/4 inches wide)
* channel lock pliers
* 3D printer access
* Computer with internet access and a usb port

# Circuit diagram
![circuit diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/circuit_diagram.drawio.png)

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

### not pictured: Y branching motor cable that comes connected to the control box

![Jeep parts photo.jpg](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/jeep%20parts.jpg)

Left over parts of the Jeep can be discarded.

# Frame and Wheel Modifications
## Back wheels
Remove all nuts and washers from the back axle.

Slide the back axle into place as shown below.

![back axle photo](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/back%20axle%20photo.jpg)

Put the two back motors on the back axle. Make sure to check the labels on the motors that say L or R and put the L motor on the side of the car that will be on the left side when the car is upright from the perspective of the driver, and put the R motor on the right side of the car. If the motors are on the wrong sides the car will drive backwards.

Install back motors, back wheels, washers, nuts (tighten the nuts on the two ends of the axle, simultaneously), and hubcaps as shown in the manual (image below). Use the provided plastic wrenches. 

![back axle diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/back%20wheels.jpg)

Check to make sure that the back wheels spin freely. If they don't, loosen the nuts a little bit.

## Front Caster Wheels
The front steering motor will not be used. The motor is on the underside of the car. Unplug the wires to the motor. Unscrew the motor, remove and discard.

![front steering motor](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/front%20steering%20motor.jpg)

Unscrew the locknuts from the metal steering mechanism to remove the front bar and use a clamp to securely hold the front bar for cutting the welds on it, in the next step.

![front bar photo](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/front_bar.png)

Remove the round tubes on the front bar by using the rotary tool and a cutting wheel to cut through the welds that hold the tubes in place. (Try to maintain the structural integrity of the square bar while cutting; the round tubes will be disposed of, so damaging them while cutting is acceptable.) After the welds are cut, use a hammer to tap the tubes out (make sure to hammer from the side of the tube OPPOSITE the weld).

Place the casters into the holes in the bar (where the tubes were), with washers on both sides of the hole. Bolt the casters to the bar using ½-13 lock nuts, using large channel lock pliers to keep the caster from spinning while turning the nut with a ¾” wrench. Make sure that the casters are not installed upside-down; mounting tabs on the bar should be on the wheel side.

Use screws found in the Jeep parts to screw the front bar to the Jeep.

![front caster wheels](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/front_caster_wheels.png)

## PVC Frame
### Cut the 10 foot length of 3/4 inch PVC pipe to the following lengths, as also shown in the diagram below:
* 2x 26.5" pieces
* 1x 14.5" piece
* 2x 13" pieces
* 2x 7.5" pieces
* 1x 5" piece
* 2x 3" pieces

![pvc frame diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/pvc%20frame.png)

Join the two parts of each 3D printed saddle tee together, using five m2.2x14mm screws.

![3D printed saddle tee](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/3d_printed_saddle_tee.png)

Place a ¼-20 locknut into the pocket at the end of each connector tee, then screw a ¼-20 ¾” machine screw with rounded head through the hole at the side of the tee and into the nut, just enough to hold the nut in place. (the nuts and bolts can also be added later, after the frame is assembled)

Attach the saddle tees to the ends of the 14.5" piece of PVC (push them onto the ends, rotated at the same angle – the flat sides of the tees should be oriented in the same direction). Drill 1/16" pilot holes into the PVC pipe, and secure with 2 m2.2x14mm screws.

Slide the saddle tees onto the two 26.5" pieces (you may need to loosen the machine screw on the end of the tee a bit to allow them to slide easily). When attached to the rest of the frame, the flat side of the saddle tees should be on the underside of the tee, and the machine screws can be tightened to lock the tees in place.

Assemble the frame as shown using the cut PVC pipe and 8 PVC elbows, trying to rotate the printed text on the PVC to the underside of the pipe so that it remains hidden from view. DO NOT GLUE THE PART OF THE JOINTS CIRCLED IN GREEN (MAKE SURE THE TOP PART – THE BACKREST – IS REMOVABLE BY LIFTING UP). Other joints should be glued with PVC glue after verifying that the elbow angles are appropriate.

![pvc frame diagram](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/pvc%20frame.png)

Use four wood screws to secure the frame to the Jeep, using two screws to attach the front posts to the side of the hood and two screws to attach the frame to the upper edge of the rear of the Jeep. Make pilot holes first using a 5/64" drill bit, then use screws. Screw into plywood chunks placed inside of the Jeep (one chunk for each screw). Tip for the back screws: if you remove the taillights (their screws can be accessed by reaching up from under the Jeep) you can hold the wood blocks through the holes, and then you can replace the lights. TO AVOID INJURY, TAKE APPROPRIATE CARE TO KEEP FINGERS CLEAR FROM THE SCREWS WHILE SCREWING INTO THE WOODEN BLOCKS.

Cover the 4 screw heads with duct tape

## Seatbelt
Improvise, based on requests from a physical therapist.

(the car seat harnesses we were using are out of stock everywhere)

# Electrical Modifications

## Remove the Seat

## Disconnect the battery
If possible, disconnect one wire from the battery to keep the circuit off while you are working on it. Some cars have a spade terminal that comes disconnected from the battery of a new car.

## Get ready to add the PCB

Remove the control box that came with the car. Unscrew the screw securing it and unplug all wires that are connected to it. The control box is not needed and can be discarded. Keep the Y branching cable that connects the two motors to the control box, as it will be used to connect the motors to the GBG-PCB.

Find the left motor plug, the battery plug, the right motor plug, the 6 wire plug, the steering motor plug, and the Y branching cable that was connected to the control box. The plugs are shown in the image below.

![plugs.png](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/plugs.drawio.png)


Gently pull on the steering motor plug and discard the brown and blue steering motor wires. The other end was unplugged when you removed the steering motor. The steering motor wires are not needed. You can cut any heatshrink tubing that is around the steering motor plug or even the steering motor wires themselves, if needed, to remove the steering motor wires. Don't cut any of the thin wires that might be bundled with the 2 steering motor wires.

## Connect the PCB to the battery wires

_The PCB can be left connected to the battery. It does not need a switch between itself and the battery. The PCB has MOSFETs that stop electricity from flowing when the on/off switch is off. When the PCB is off it draws practically zero current (2 nanoAmps) so it will not make the battery discharge._

Cut the red battery wire where it connects to the battery plug. Strip 3/8" (10 mm) of insulation off the end of the red wire. Connect the red battery wire to the positive large BATTERY screw terminal on the GBG-PCB (labeled "+"). Tighten the screw terminal tightly to hold the wire in place.

Cut the black battery wire where it connects to the battery plug. Strip 3/8" (10 mm) of insulation off the end of the black wire. 

Cut the thin black wire off the 6 wire plug. Strip 3/8" (10 mm) of insulation off the end of the black wire.

Put both the black battery wire and the thin black wire from the 6 wire plug into the negative large BATTERY screw terminal on the GBG-PCB (labeled "-"). Tighten the screw terminal securely to hold both wires in place.

## Wire the PCB to the on/off switch

Cut the thin white wire off the 6 wire plug. Strip 1/4" (6 mm) of insulation off the end of the white wire. Connect the white wire to the left side of the ON/OFF screw terminal on the GBG-PCB. It's important that the white wire is connected to the side of the on/off switch that is closer to the left motor screw terminal. The white wire should go to the side of the on/off screw terminal that is closer to the word "off" than the word "on" where it says "on/off" on the PCB.

Cut the thin red wire off the 6 wire plug. Strip 1/4" (6 mm) of insulation off the end of the red wire. Connect the red wire to the small BATT screw terminal on the GBG-PCB (labeled "+").

![power wires](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/power_wires.jpg)

## Wire the PCB to the motors

Plug the Y branching cable that was connected to the control box into the two motor plugs. Then, cut the plug where the 4 wires meet the plug.

![motorplugs.drawio.png](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/motorplugs.drawio.png)

Strip 3/8" (10 mm) of insulation off the ends of the wires. 

Connect the motor wires to the left and right motor screw terminals on the GBG-PCB. The red wires should go to the sides of the terminals marked with a small "+" and the black wires should go to the sides of the terminals marked with a small "-".

![motors wired](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/motors_wired.jpg)

## Wire the Joystick
### Route the joystick cable
Take the 4 wire cable and put it through the hole at the front right of the battery compartment (following the wires that had gone to the 6 wire plug). The 4 wire cable should go inside the plastic guard under the gear shift lever. If you can't push the cable through so it comes out in front of the plastic guard, you could unscrew the plastic guard, run the cable, then put the plastic guard back in place.

Unscrew the dashboard.

Identify the plug that powers the music and horn. Label it "UNPLUG TO DEACTIVATE MUSIC".

![dashboard photo.drawio.png](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/dashboard%20photo.drawio.png)

Route the 4 wire cable up to the dashboard, following the red, white, and black wires that go to the dashboard. The 4 wire cable should then go out of the dashboard through the hole for the steering wheel and reach about 13 inches (33 cm) outside the dashboard.

Cut a 12 inch (30 cm) length of wire protector tubing and slide it over the length of the 4 wire cable that is outside the dashboard. This will protect the wires from being pulled by the kid.

Add a zip tie around the 4 wire cable and the wire protector tubing on the inside of the dashboard, to keep the cable from being pulled out of the dashboard.

![dashboard photo 1](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/dashboard_photo_1.jpg)

Screw the dashboard back in place, leaving the "unplug to deactivate music" plug out of the dashboard.

![dashboard photo 2](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/dashboard_photo_2.jpg)

Plug the joystick into the joystick pcb.

Connect the 4 wire cable to the screw terminal on the joystick pcb. Strip 1/4" (6 mm) of insulation off the ends of the wires and connect them to the screw terminal on the joystick pcb.

Hot glue the joystick pcb inside the 3d printed joystick holder so that it can't move around and jam the joystick. Match the position in the photo below.

Add a ziptie to the end of the wire protector, to keep the wires from being pulled out.

![joystick pcb photo](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/joystick_pcb_photo.jpg)

Before closing up the joystick holder, drop a 4-40 nut into the slot for the top hole. This nut will be used to secure the joystick holder to the pvc frame later.

Screw the top of the joystick holder to the bottom of the joystick holder, using 4 m2.2x14mm screws. If the joystick is incorrectly rotated, the 3d printed parts won't fit together. The ziptie and wire protector should be inside the joystick holder.

At the other end of the 4 wire cable, in the space under the seat, strip 1/4" (6 mm) of insulation off the ends of the wires. Connect the wires to the screw terminal on the GBG-PCB labeled "joystick". Make sure that between the GBG-PCB and the joystick pcb, the wires are connected in the same order. "X", "3V", "Y", "GND" on the two boards should be connected together.

### Attach Joystick Holder
Cut a 0.75 inch (19mm) by 1.75 inch (45mm) rectangular piece of 1/16” thick rubber gasket sheet.

Put the piece of rubber into the recessed rectangle of the joystick holder clamp. (You may have to trim the piece of rubber to size)

Remove the 4-40 machine screws that are temporarily holding the 4-40 nuts in the joystick holder, taking care not to let the nuts fall out of their slots. Then slide the bolts through the two holes in the 3d printed clamp piece.

![clamp_piece.png](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/clamp_piece.png)

Bolt the joystick holder base to the clamp around the PVC crosspiece. It should take almost no force with the screwdriver – if you feel resistance, check the alignment of the nuts and try again. Tighten both bolts similar distances.

![joystick_holder_clamp_photo.png](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/joystick_holder_clamp_photo.png)

Twist the two silver metal pieces off of the joystick threaded shaft and discard.

Screw one of the 3D printed joystick handles onto the shaft of the joystick. Don’t over tighten since you’re screwing into plastic. It may help to drill out the hole with a 3/32" drill bit. 
_Alternatively, you could modify the handle models and use a threaded heat set insert to connect the joystick handle to the joystick shaft._

Add some hot glue where the joystick wires enter the dasbhoard and where the joystick wires enter the joystick holder as additional strain relief.

## (optional) Wire Buttons and/or Speed Knob
### Buttons
Plug up to 4 buttons into the headphone-style jacks on the GBG-PCB.

When you connect the GBG-PCB to your computer to change the settings, click the "show all" button and check the box next to "enable button ctrl". Then, you can set what direction each button should make the car move in.

### Speed Knob
You can add a knob to the car for easily adjusting the maximum speed of the car without needing to reprogram it.

Connect a potentiometer to the screw terminal labeled "speed knob". 

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


# Finishing Touches

Secure the GBG-PCB inside the battery compartment using hot glue (make sure the USB port can still be used).
![secure_pcb.JPG](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/secure_pcb.jpg)

Clean out bits of wires and insulation that might have fallen into the car or electronics compartment. Ideally, use a vacuum cleaner.

Re-attach the seat and screw it into place using screws that came with the car.

Label the "on/off" button (the red power button on the dashboard)

Screw the grey reinforcement pieces to the bottom of the car using screws that came with the car.

![grey_reinforcement.jpg](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/car-specific/aosom-038-jeep/photos/grey_reinforcement.jpg)

Print a [user guide](https://docs.google.com/document/d/1gazkX-ZfFOiyW0IYRKWDf3U71-eo1b7SZ_yoa84WfKo/edit?usp=sharing) for the car.

### Congratulations! You're done!

# Check your work
Check your work with this [inspection checklist](https://docs.google.com/document/d/16H79A8kvLGwDgCY7LqITseffnMbmoiTtzU1TYeZi0BQ/edit?usp=sharing)

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
### that means the joystick needs to be left centered for a few seconds before trying to move
#### Let go of the joystick for 5 seconds and wait for the light to stop blinking
### it could also mean that the joystick needs to be recalibrated
#### If the blue light continues to blink quickly after letting go of the joystick for 5 seconds, then you should recalibrate the joystick using the programmer website. Connect the GBG-PCB to your computer, go to the programmer website, connect the website to the GBG-PCB, then click the "calibrate the joystick the easy way" button and follow the instructions on the screen.
## if none of the green lights on the PCB turn on,
#### the battery might have been connected backwards. A backwards connection does not damage the board; the board just doesn't turn on.
#### the on/off switch might not be wired correctly
