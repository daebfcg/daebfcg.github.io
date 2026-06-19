---
title: "Schematic"
date: "2026-06-19T16:11:03Z"
cover: ""
tags: ["wiring"]
series: ["Electric Guitar Build 2025-2026"]
keywords: []
description: "The updated schematic of the final circuit used"
showFullContent: false
readingTime: false
draft: false
---
## Final Version

{{<imgresize schematic.png "800x800" "Final version of the guitar schematic">}}

## Notes

### Toggle Switch

Schematic updated to reflect the DPDT On-On-On switch actually used.  (`SW3`)

Interestingly, the middle-tone `RV1` can now be connected to pin 3 of the switch which is only ever in contact with the series-junction (via the pin 2-4 jumper) in the center position only.  This is much preferred over the previous SPDT on-off-on wiring where the only option was having the middle-tone connected to the neck pickup at all times and acting as a redundant treble tone control when the neck pickup was selected.

### Tone Pot Pin Numbers

Previous schematics had the tone pots flipped and the signal incorrectly going to pin 3, with pin 1 unused.  Updated to show the correct wiring of signal to pin 1 on the tone pots with pin 3 unused. (`RV1` and `RV2`)

### Safety Coupler

The shielding and user-touchable components to ground connection being made through a capacitor and resistor for shock prevention is now reflected on the schematic. (`R1`, `C4`)
