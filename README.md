# GBG PCB
## work in progress. this will be updated after the boards are tested.
* Update for v1.0: the motor drivers work, the circuit board supplied 15A from one motor port for 4 minutes without overheating, the reverse voltage protection MOSFETS need to be redesigned for v1.1
* Update for v1.1: reverse voltage protection works, on/off switch works, still working on testing current

# A PCB for controlling the motors in a [go baby go car with joystick control](https://gobabygocarswithjoysticks.github.io/index/)

https://github.com/gobabygocarswithjoysticks/gbg-pcb

[![Process KiCad](https://github.com/gobabygocarswithjoysticks/gbg-pcb/actions/workflows/process-kicad.yml/badge.svg)](https://github.com/gobabygocarswithjoysticks/gbg-pcb/actions/workflows/process-kicad.yml)

questions? post [here](https://github.com/gobabygocarswithjoysticks/gbg-pcb/discussions/categories/questions-and-troubleshooting) or email gobabygocarswithjoysticks@gmail.com 

## Want one?
1. Feel free to use or modify this design and make your own boards. 
2. Email gobabygocarswithjoysticks@gmail.com, I might have assembled boards to sell or donate to you. The components cost approximately $50.

# [instructions for using this PCB to modify a car](https://gobabygocarswithjoysticks.github.io/gbg-pcb/instructions/instructions)

# [schematic](/schematic.pdf)

# [PCB Production files](/PCB_production)
send [gerbers.zip](/PCB_production/gerbers.zip) to a PCB fabrication company

here are the parameters for the PCBs that have been tested:
* 1oz copper
* 0.8mm board thickness
* 8mil/8mil
* 0.3mm holes

[F_SolderPasteMask.dxf](/PCB_production/F_SolderPasteMask.dxf) can be used to get a solder stencil

The [BOM.csv](/PCB_production/BOM.csv) file can be imported to a Digikey list

The [position.csv](/PCB_production/position.csv) file has not yet been used to buy fully assembled PCBs, but it should be accurate.

# [joystick to 4 wire cable connector PCB](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/joystickpcb)
### This keeps you from needing to solder the joystick wires to a 4 wire cable.

# notes for people working on the KiCAD for this project
Use KiCAD 9.0

Run [this github action](https://github.com/gobabygocarswithjoysticks/gbg-pcb/actions/workflows/process-kicad.yml) when you push changes to any of the KiCAD files. The action updates the images of the CAD, the gerber files, the schematic, and other PCB production files. 

# photos
![view of assembled PCB from the top](/photos/image0.jpg)
![view of assembled PCB](/photos/image1.jpg)

# images of CAD

![auto generated image, topview](/renders/top.jpg)
![auto generated image, p1](/renders/perspective1.jpg)
![auto generated image, p2](/renders/perspective2.jpg)
![auto_generated_image, back](/renders/back.jpg)

# results from testing the PCB
# v1.1:

## How much current does the PCB draw when it's off?
### 0.0000000018 Amps

That is practically zero current. The PCB won't make the battery discharge any faster than the battery would just sitting in storage with nothing connected.

I measured the current by adding a 3MOhm resistor in series with the PCB and a 12V power supply. I measured the voltage across the resistor as 5.5mOhm and then calculated the current that was flowing through the resistor and PCB.

I=V/R=0.0055/3000000=1.83E-9 Amps (2 nanoAmps)

## How much current can the PCB supply to a motor?
TODO

## What voltages can the PCB run on?
### 12 Volts
It won't run on 6 volts, the motor driver ICs need over 8 volts.

It hasn't been tested above 12 Volts.

The PCB was only designed for 12 Volt ride on cars. Feel free to email if you are interested in trying it at other voltages.

# v1.0: 
The reverse voltage protection MOSFETS need to be redesigned. The motor drivers work and the circuit board supplied **15A** from one motor port for 4 minutes without overheating.

Here's an IR image from the end of the test:
![thermal camera image](/photos/IR1.jpg)

