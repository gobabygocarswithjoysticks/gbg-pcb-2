# GBG PCB
## work in progress. this will be updated after the boards are tested.
* Update for v1.0: the motor drivers work, the circuit board supplied 15A from one motor port for 4 minutes without overheating, the reverse voltage protection MOSFETS need to be redesigned for v1.1
* Update for v1.1: waiting to receive boards


# A PCB for controlling the motors in a [go baby go car with joystick control](https://gobabygocarswithjoysticks.github.io/index/)

https://github.com/gobabygocarswithjoysticks/gbg-pcb

[![Process KiCad](https://github.com/gobabygocarswithjoysticks/gbg-pcb/actions/workflows/process-kicad.yml/badge.svg)](https://github.com/gobabygocarswithjoysticks/gbg-pcb/actions/workflows/process-kicad.yml)

open with KiCAD 9.0

* 2 motor drivers
* screw terminals
* Raspberry Pi Pico 1/1W/2/2W

# [schematic](/schematic.pdf)

# [PCB Production files (gerbers)](/PCB_production)
send gerbers.zip to a PCB fabrication company
* 1oz copper
* 0.8mm board thickness
* 8mil/8mil
* 0.3mm holes

The BOM.csv file can be imported to a Digikey list

# [joystick to 4 wire cable connector PCB](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/joystickpcb)
![cad render](https://github.com/gobabygocarswithjoysticks/gbg-pcb/blob/main/joystickpcb/images/3d.jpg)

# notes for people working on the KiCAD for this project
Run [this github action](https://github.com/gobabygocarswithjoysticks/gbg-pcb/actions/workflows/process-kicad.yml) when you push changes to any of the KiCAD files. The action updates the images of the CAD, the gerber files, the schematic, and other PCB production files. 

# photos
![view of assembled PCB on a desk with the battery wires connected](https://github.com/gobabygocarswithjoysticks/gbg-pcb/blob/main/photos/image1.jpg)

# images of CAD

![auto generated image, topview](/renders/top.jpg)
![auto generated image, p1](/renders/perspective1.jpg)
![auto generated image, p2](/renders/perspective2.jpg)
![auto_generated_image, back](/renders/back.jpg)
