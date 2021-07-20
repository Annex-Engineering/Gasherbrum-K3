XY Gantry Options
=================

## Motor Mounts

**M6 Corner Screw**
This option accomodates 2020 vertical extrusions that are tapped as M6 instead of M5.

**Custom LDO Motor**
Use this option if you are using the custom long shaft motors from LDO.

## Linear Rail Instructions

**Running Robotdigg Rails**?
If you are using robotdigg rails, you should to use the STLs in the `for_6.0mm_thick_rails` folder for the tensioner spacer and rail mounts, as these rails are 0.5mm thinner.

**General Sizing Tips**
- Before printing the tensioner spacer, try slicing the main toolhead plate (with whatever settings you will/did use to print it) and check the distance from the bottom to the surface that sits underneath the upside-down rail.
- Try slicing the tensioner spacer, and make sure its sliced height from top to bottom is 14.0mm more than your measurement from the toolhead plate.
    - For example, if the thickness on the toolhead plate ends up being 6.6mm, then your tensioner spacer should end up being 20.6mm tall.
- Scale the tensioner spacer (in the z axis only) if it is the wrong size when sliced.
