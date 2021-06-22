# K3 Toolhead README

## Useful Notes

- range of motion:
    - X: -8 to 180
    - Y: 0 to 186
- probe dock location: X-8 Y186
- homing location: X180 Y0
- bowden tube length (mm):

    |               | sherpa mini   | ascender  |
    | ---           | ---           | ---       |
    | mosquito      | 26.5          | 26.0      |
    | copperhead    | 46.5          | 46.0      |
    | dragon        | 27.5          | 27.0      |
    | dragonfly BMO | unknown*      | unknown*  |
    | dragonfly BMS | unknown*      | unknown*  |
    | dragonfly HIC | unknown*      | unknown*  |
    
    *For each of the dragonfly hotends, the bowden tube should stick out of the top of the heatsink by `(mosquito bowden tube length) - 1.0`. We do not  currently know how far the tube extends into these hotends; if you use a dragonfly hotend, please measure the overall length of your tube after cutting it so we can add it to this guide.

- For the mosquito version, make sure the thickness of the hotend fan + the height of the screw head attaching it add up to less than 13.36mm.
- If you use the dragonfly BMO, remove the groove mount adapter.
- If you use the copperhead, dragonfly BMS, or dragonfly HIC, remove the collet.
- Some versions of the toolhead space the fan mounts and probe downward since the hotend is longer. With these hotends, you may lose up to the following z height:
    - copperhead: 4.5mm
    - dragonfly BMS: 1.85mm
    - dragonfly HIC: 12.4mm
- There is 1 fan mount hole in the main body that is recessed more than the others. This hole requires a button head screw (6-8mm long), but the remaining 5 holes can be either button head or cap head.
- The probe dock is the same one used for K1/K2, and the probe used is the R2 version. The stls for the dock and probe body are included in this folder.
- All versions of the toolhead use a 25mm fan for the hotend, except for the dragon and dragonfly HIC versions, which use a 30mm fan.

## What to print

Please print all parts in the "common parts" section, the section for your chosen hotend, and the section for your chosen extruder:

### Common parts

- front_fan_mount_x1
- front_fan_nozzle_x1
- magswitch_probe_mount_x1
- omron_d2f-5_microswitch_probe_body_x1
- rear_fan_mount_x1
- rear_fan_nozzle_x1

### Hotends

Slice Mosquito
- sherpa_mosquito_main_body_x1 or ascender_mosquito_main_body_x1
- mosquito_brace_for_probe_mount_x1
- mosquito_side_mount_x1

Slice Copperhead
- sherpa_mosquito_main_body_x1 or ascender_mosquito_main_body_x1
- mosquito_brace_for_probe_mount_x1
- copperhead_brace_spacer_x1
- copperhead_fan_spacer_x2

Dragon-Style Hotend
- sherpa_dragon_main_body_x1 or ascender_dragon_main_body_x1
- dragon_brace_for_probe_mount_x1
- dragon_fan_shroud_x1

Dragonfly BMO
- sherpa_dragonfly_bmo_main_body_x1 or ascender_dragonfly_bmo_main_body_x1
- mosquito_brace_for_probe_mount_x1
- dragonfly_bmo_fan_shroud_x1

Dragonfly BMS
- sherpa_mosquito_main_body_x1 or ascender_mosquito_main_body_x1
- mosquito_brace_for_probe_mount_x1
- dragonfly_bms_fan_spacer_x2
- dragonfly_bms_hotend_mount_x1

Dragonfly HIC
- sherpa_mosquito_main_body_x1 or ascender_mosquito_main_body_x1
- dragonfly_hic_fan_spacer_x2
- dragonfly_hic_hotend_mount_x1

### Extruders

Sherpa Mini
- sherpa_umbilical_mount_x1
- (sherpa mini extruder with k-series front housing)

Ascender
- ascender_umbilical_mount_x1
- (mirrored variant of the double folded ascender extruder)