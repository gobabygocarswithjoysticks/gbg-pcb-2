## send [gerbers.zip](/PCB_production/gerbers.zip) to a PCB fabrication company

## [F_SolderPasteMask.dxf](/PCB_production/F_SolderPasteMask.dxf) can be used to get a solder stencil

## The [position.csv](/PCB_production/position.csv) file has the locations for the surface mount components

## The BOM can be imported to a Digikey list
please email gobabygocarswithjoysticks@gmail.com if components are out of stock and you need recommendations for alternatives

[BOM.csv](/PCB_production/BOM.csv) is the normal list of parts (using screw terminals for connections).

[BOM-with-DNP.csv](/PCB_production/BOM-with-DNP.csv) includes alternative parts that you could choose some of, for other configurations of the board.

## parameters for PCBs:
* 1oz copper
* 1.0mm board thickness
* 4mil/4mil
* 0.25mm holes

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

