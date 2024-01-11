# Overview
A 40% ortholinear mx mechanical keyboard powered by a proMicro or equivalent.

This keyboard is discontinued. While it should still work, there may be incompatibilities with some current and future operating systems.

# Specifications
-1.6mm PCB
-proMicro (or equivalent) controller board
-44x SOD-123 diodes
-44x mx switches

# Assembly instructions
1) solder the diodes and the reset switch (optional).
2) solder the proMicro with the USB port facing up (the controler chip should be visible)
3) Put the mx switches into the top plate, and put screw-in stabilisers into the PCB in the spacebars. Place the two assemblies on top pf each other, so that the pins of the switches in the plate line up to the holes for the switches in the PCB. Solder these in.
4) using m2 screws and 12mm standoffs, mount the basepiece to the plate.
5) flash the firmware to the proMicro using QMK Toolbox, either by shorting the reset and ground pins on the proMicro, or by Pressing and holding the reset button under the plate.

# Known flaws
- The keyboard uses a potentially outdated QMK release, which may have incompatibilities with future operating systems.
- USB C-C cables cannot be used due to the limitations of the proMicro
- The firmware is written for an Amtel AtMega32U4 based proMicro. Other microcontrollers may not work, or you may need to rewrite the firmware yourself.
