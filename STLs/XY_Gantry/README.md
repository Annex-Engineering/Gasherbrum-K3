XY Gantry Options
=================

## Motor Mounts

**M6 Corner Screw**
This option accomodates 2020 vertical extrusions that are tapped as M6 instead of M5.

**Custom LDO Motor**
Use this option if you are using the custom long shaft motors from LDO.

## Linear Rail Instructions

**Running RobotDigg Rails**?
If you are using RobotDigg or LDO rails, you should to use the STLs in the `for_6.0mm_thick_rails` folder for the tensioner spacer and rail mounts, as these rails are 0.5mm thinner.

**Spacer Sizing Tips**
- Before printing the tensioner spacer, try slicing the main toolhead plate (with whatever settings you will/did use to print it) and check the distance from the bottom to the surface that sits underneath the upside-down rail. The model is 6.5mm thick, but depending on your slicer and its settings, the part may be sliced slightly thicker or thinner.
- Try slicing the tensioner spacer and check it's sliced height from top to bottom.
    - For 6.5mm (normal) rails, the spacer height should be 13.5mm thicker than the toolhead plate measurement.
    - For 6.0mm (Robotdigg) rails, the spacer height should be 14.0mm thicker than the toolhead plate measurement
    - For example, if the toolhead plate slices at 6.6mm thick and you're using Robotdigg rails, size the spacers so that they are sliced 20.6mm tall.
- Scale the tensioner spacer (in the z axis only) if it is the wrong size when sliced.
- For best alignment of the final assembly, you may choose to physically measure the toolhead plate after printing it, then print the spacers with an extra layer and carefully sand them down to final dimension. Be sure to keep the top and bottom surfaces flat and parallel when sanding.
