## send [gerbers.zip](/PCB_production/gerbers.zip) to a PCB fabrication company

## [F_SolderPasteMask.dxf](/PCB_production/F_SolderPasteMask.dxf) can be used to get a solder stencil

## The [position.csv](/PCB_production/position.csv) file has the locations for the surface mount components

## The BOM can be imported to a Digikey list
please email gobabygocarswithjoysticks@gmail.com if components are out of stock and you need recommendations for alternatives

[BOM.csv](/PCB_production/BOM.csv) is the normal list of parts (using screw terminals for connections).

[BOM-with-DNP.csv](/PCB_production/BOM-with-DNP.csv) includes alternative parts that you could choose some of, for other configurations of the board.

## [joystick to 4 wire cable connector PCB](https://github.com/gobabygocarswithjoysticks/gbg-pcb/tree/main/joystickpcb)
### This keeps you from needing to solder the joystick wires to a 4 wire cable.

## parameters for PCBs:
* 1oz copper
* 1.0mm board thickness
* 5mil/5mil
* 0.25mm holes
* solder stencils should be 0.12mm

## other configurations

### alternate voltage regulator (U5)
Replace U3, C3, R5, C6, L1, C7, R8, R9, C8

Choose a single THT module that outputs 5V. Make sure the pinout matches. Make sure hte min and max input voltage are compatible with your battery.

Consider pololu5593, D78B05T, RBT05W24S05

### alternate battery and motor connectors (Weelye mode)
The GBG-PCB includes pads for adding connectors that match the connectors on some common weelye control boxes like the RX22 and RX7.

* J102 and J103 replace J5
* J100 and J101 replace J7
* J104 replaces J8

### Other models of Raspberry Pi Pico (P1)
If you want to be able to change settings and remote override the car over a wifi connection [(see information here)](https://github.com/gobabygocarswithjoysticks/car-code/blob/main/rcdocs/remote_control.md#notes-on-wifiwebsite-remote-control) then you can substitute a Pico 1W or Pico 2W for the standard Pico 1.

