# GBG PCB

# A PCB for controlling the motors in a [go baby go car with joystick control](https://gobabygocarswithjoysticks.github.io/index/)

https://github.com/gobabygocarswithjoysticks/gbg-pcb

[![Process KiCad](https://github.com/gobabygocarswithjoysticks/gbg-pcb/actions/workflows/process-kicad.yml/badge.svg)](https://github.com/gobabygocarswithjoysticks/gbg-pcb/actions/workflows/process-kicad.yml)

V2.0

This board replaces the control box of a car's original electronics or the separate ESCs and Arduino in the [usual joystick modification](https://gobabygocarswithjoysticks.github.io/index/). The board has screw terminals for connecting to the battery, motors, and the joystick. With this circuit board, a car can be converted to joystick control without any soldering.

Voltage input: 5 to 26 volts (6v, 12v, and 24v lead acid batteries)

Controls two motors: one for each wheel so that the car can turn in place.

[New in version 2](https://github.com/gobabygocarswithjoysticks/gbg-pcb/edit/main/docs/instructions/instructions.md#new-in-v2-weelye-control-box-compatible): A V2 GBG-PCB can be configured with battery, motor, and signal plugs that match the plugs on the common weelye control boxes. This means some cars can be converted to joystick control without cutting any wires.

For the previous versions of the GBG-PCB see https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/version_1 

## questions? email our support line at gbg-pcb@googlegroups.com or post [here](https://github.com/gobabygocarswithjoysticks/gbg-pcb/discussions/categories/questions-and-troubleshooting)

# Want one?
* Email pnwassistivetech@gmail.com or visit the [PNW Assistive Technology website](TODO/gbg-pcb). Thank you to PNWAT for supporting this project and being a supplier of these boards.
* Use this PCBWay link to order fully assembled boards: [TODO]()
* Email gobabygocarswithjoysticks@gmail.com. We may have a small number of assembled boards to sell or donate to you.
* Or feel free to use these [files](/PCB_production) and get boards yourself.

# Instructions
## [general instructions for using this PCB](https://gobabygocarswithjoysticks.github.io/gbg-pcb/instructions/instructions)
### [instructions for assembling your own GBG-PCBs](TODO) (coming soon)
## Index of Instructions for modifying specific models of cars using GBG-PCBs
* [Aosom Jeep - old model](https://gobabygocarswithjoysticks.github.io/gbg-pcb/instructions/car-specific/aosom-038-jeep/instructions) (car is out of production)
* [Zupapa Bumper Car](https://gobabygocarswithjoysticks.github.io/gbg-pcb/instructions/car-specific/zupapa-bumper-car/instructions) (instructions are complete through electronics but don't include a backrest or joystick holder)
* [coming soon](todo)

# [schematic of PCB](/schematic.pdf)

# [PCB Production files](/PCB_production)

# [joystick to 4 wire cable connector PCB](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/joystickpcb)
### This keeps you from needing to solder the joystick wires to a 4 wire cable.

![schematic](https://raw.githubusercontent.com/gobabygocarswithjoysticks/gbg-pcb/refs/heads/main/docs/instructions/diagrams/circuit_diagram.drawio.png)

# notes for people working on the KiCAD for this project
Use KiCAD 10.0

Run [this github action](https://github.com/gobabygocarswithjoysticks/gbg-pcb/actions/workflows/process-kicad.yml) when you push changes to any of the KiCAD files. The action updates the images of the CAD, the gerber files, the schematic, and other PCB production files. 

# photos
<!-- ![view of assembled PCB from the top](/photos/image0.jpg) -->
<!-- ![view of assembled PCB](/photos/image1.jpg) -->

# images of CAD

![auto generated image, top view](/renders/top.jpg)
![auto generated image, p1](/renders/perspective1.jpg)
![auto generated image, p2](/renders/perspective2.jpg)
![auto_generated_image, back](/renders/back.jpg)

# credits

## Sponsored by PNW Assistive Technology

## Copyright: gobabygocarswithjoysticks and Joshua Phelps, MIT License

