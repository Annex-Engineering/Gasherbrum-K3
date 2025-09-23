# Toolhead Options and Notes

## Useful Notes

- There is an eDrawing for the toolheads that contains a configuration for each
  hotend with sherpa mini, one with sherpa micro and mosquito, and one with
  ascender and mosquito. Click the "Configurations" button in the bottom right
  to access all the configurations.
- Range of motion:
    - X: -8 to 180
    - Y: -2 to 184
- Probe dock location: X-8 Y181
- Homing location: X180 Y-2
- Bowden tube length (mm):

    |               | Sherpa (Mini or Micro)  | Ascender  | LGX Lite  |
    | ---           | ---                     | ---       | ---       |
    | Mosquito      | 26.5                    | 25.5      | 21.5      |
    | VolcoMosq     | 26.5                    | 25.5      | 21.5      |
    | Teakettle     | unknown*                | unknown*  | unknown*  |
    | Dragon        | 27.5                    | 26.5      | 22.5      |
    | Rapido HF     | unknown*                | unknown*  | unknown*  |
    
    - *For each of the hotends with unknown bowden tube length, the bowden tube
      should extend above the main body by the amount shown below, depending on
      which extruder you're using. We do not currently know how far the tube
      extends into these hotends; if you use one of them, please measure the
      overall length of your tube after cutting it so we can add it to this
      guide.
      - Sherpa (Mini or Micro): 8mm
      - Ascender: 7.5mm

- For the Mosquito and VolcoMosq versions, make sure the thickness of the hotend
  fan + the height of the screw head attaching it add up to less than 13.36mm.
- If you use the Rapido, remove the groove mount adapter.
- If you use the Rapido, make sure it is oriented so the wire is exiting in the
  same direction as in the edrawing. Other orientations also work if you use
  M2.5x14 screws to make sure the screw doesn't hit the heatsink.
- Some versions of the toolhead space the fan mounts and probe downward since
  the hotend is longer. With these hotends, you may lose up to the following z
  height:
    - VolcoMosq: 8.5mm
    - Rapido HF: 8.5mm
- There is 1 fan mount hole in the main body that is recessed more than the
  others. This hole requires a button head screw, but the remaining 5 holes can
  be either BHCS or SHCS.
- All versions of the toolhead use a 25mm fan for the hotend, except for the
  Dragon version, which uses a 30mm fan.

## What to print

Please print all parts in the "common parts" section, the section for your
chosen hotend, the section for your chosen extruder, and the section for your
chosen probe:

### Common parts

- `front_fan_mount_x1`
- `front_fan_nozzle_x1`
- `magswitch_probe_mount_x1`
- `omron_d2f-5_microswitch_probe_body_x1`
- `rear_fan_mount_x1`
- `rear_fan_nozzle_x1`

### Hotends

Slice Mosquito
- main body (depends on your extruder):
  - Sherpa Mini: `sherpa_mini_mosquito_main_body_x1`
  - Sherpa Micro: `sherpa_micro_mosquito_main_body_x1`
  - Ascender: `ascender_mosquito_main_body_x1`
  - LGX Lite:
    - `lgx_lite_mosquito_main_body_x1`
    - `lgx_lite_mounting_plate_x1`
- `mosquito_brace_for_probe_mount_x1`
- `mosquito_side_mount_x1`

VolcoMosq
- main body (depends on your extruder):
  - Sherpa Mini: `sherpa_mini_mosquito_main_body_x1`
  - Sherpa Micro: `sherpa_micro_mosquito_main_body_x1`
  - Ascender: `ascender_mosquito_main_body_x1`
  - LGX Lite:
    - `lgx_lite_mosquito_main_body_x1`
    - `lgx_lite_mounting_plate_x1`
- `mosquito_side_mount_x1`
- `volcomosq_brace_for_probe_mount_x1`
- `volcomosq_fan_spacer_x2`

Teakettle
- main body (depends on your extruder):
  - Sherpa Mini: `sherpa_mini_teakettle_main_body_x1`
  - Sherpa Micro: `sherpa_micro_teakettle_main_body_x1`
  - Ascender: `ascender_teakettle_main_body_x1`
- `teakettle_brace_for_probe_mount_x1`
- `teakettle_fan_shroud_outlet_x1`
- `rail_cart_screw_spacer_0.5mm_x1`
  - If your rail cart screw holes are tapped to at least 3.5mm deep, you can
    omit this part.

Dragon-Style Hotend
- main body (depends on your extruder):
  - Sherpa Mini: `sherpa_mini_dragon_main_body_x1`
  - Sherpa Micro: `sherpa_micro_dragon_main_body_x1`
  - Ascender: `ascender_dragon_main_body_x1`
  - LGX Lite:
    - `lgx_lite_dragon_main_body_x1`
    - `lgx_lite_mounting_plate_x1`
- `dragon_brace_for_probe_mount_x1`
- `dragon_fan_shroud_x1`

Rapido HF
- main body (depends on your extruder):
  - Sherpa Mini: `sherpa_mini_dragon_main_body_x1`
  - Sherpa Micro: `sherpa_micro_dragon_main_body_x1`
  - Ascender: `ascender_dragon_main_body_x1`
  - LGX Lite:
    - `lgx_lite_dragon_main_body_x1`
    - `lgx_lite_mounting_plate_x1`
- `volcomosq_brace_for_probe_mount_x1`
- `volcomosq_fan_spacer_x2`
- `rapido_fan_shroud_x1`

### Extruders

Sherpa Mini
- `sherpa_umbilical_mount_x1`
- (sherpa mini extruder with k-series front housing)

Sherpa Micro
- `sherpa_umbilical_mount_x1`
- (sherpa micro extruder with k-series front housing)

Ascender
- `ascender_umbilical_mount_x1`
- (double folded ascender extruder - R4 or newer)

LGX Lite
- `lgx_lite_umbilical_mount_x1`

### Probes

Beacon RevH
- `beacon_mount_(revH)_x1`

Beacon RevD
- `beacon_mount_(revD)_x1`

Quickdraw
- `magswitch_probe_mount_x1`
- `omron_d2f-5_microswitch_probe_body_x1`
