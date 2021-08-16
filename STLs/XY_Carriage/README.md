# K3 Toolhead README

## Useful Notes

- There is an eDrawing for the toolheads that contains a configuration for each hotend with sherpa mini, and one with ascender and mosquito. Click the "Configurations" button in the bottom right to access all the configurations.
- Range of motion:
    - X: -8 to 180
    - Y: -2 to 184
- Probe dock location: X-8 Y181
- Homing location: X180 Y-2
- Bowden tube length (mm):

    |               | sherpa mini   | ascender  |
    | ---           | ---           | ---       |
    | Mosquito      | 26.5          | 26.0      |
    | Copperhead    | 46.5          | 46.0      |
    | VolcoMosq     | 26.5          | 26.0      |
    | Dragon        | 27.5          | 27.0      |
    | Dragonfly BMO | unknown*      | unknown*  |
    | Dragonfly BMS | unknown*      | unknown*  |
    | Dragonfly HIC | unknown*      | unknown*  |
    
    *For each of the Dragonfly hotends, the bowden tube should stick out of the top of the heatsink by `(mosquito bowden tube length) - 1.0`. We do not  currently know how far the tube extends into these hotends; if you use a Dragonfly hotend, please measure the overall length of your tube after cutting it so we can add it to this guide.

- For the Mosquito and VolcoMosq versions, make sure the thickness of the hotend fan + the height of the screw head attaching it add up to less than 13.36mm.
- If you use the Dragonfly BMO, remove the groove mount adapter.
- If you use the Copperhead, Dragonfly BMS, or Dragonfly HIC, remove the collet.
- Some versions of the toolhead space the fan mounts and probe downward since the hotend is longer. With these hotends, you may lose up to the following z height:
    - Copperhead: 4.5mm
    - VolcoMosq: 8.5mm
    - Dragonfly BMS: 1.85mm
    - Dragonfly HIC: 12.4mm
- There is 1 fan mount hole in the main body that is recessed more than the others. This hole requires a button head screw, but the remaining 5 holes can be either button head or cap head.
- The probe dock is the same one used for K1/K2, and the probe used is the R2 version. The stls for the dock and probe body are included in this folder.
- All versions of the toolhead use a 25mm fan for the hotend, except for the Dragon and Dragonfly HIC versions, which use a 30mm fan.

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
- copperhead_brace_for_probe_mount_x1
- copperhead_fan_spacer_x2

VolcoMosq
- sherpa_mosquito_main_body_x1 or ascender_mosquito_main_body_x1
- volcomosq_brace_for_probe_mount_x1
- volcomosq_fan_spacer_x2

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