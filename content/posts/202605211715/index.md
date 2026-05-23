---
title: "Circuit and Components"
date: "2026-05-21T22:15:50Z"
cover: ""
tags: []
series: ["Electric Guitar Build 2025-2026"]
keywords: []
description: "Final plan for circuit and components selection"
showFullContent: false
readingTime: false
draft: false
---

## Final Version

Updated schematic:

{{<imgresize schematic_new.png "800x800" "Final schematic">}}

A few changes from before.

- Volume pot `RV4` is specified as a 333KΩ,  This is a reduction from the original 500K.  It sounds slightly smoother and less harsh.  Lots of single-coil pickup guitars use 250K for this reason.  There is a slight drop in overall volume but it is almost imperceptible.  I thought 250 was a bit too soft sounding, so added a 1MΩ resistor across the 500K pot to make it 333 for a good middle ground.

- Treble tone capacitor is now .022 µF instead of .015 µF.  Just slightly more treble and mid roll off.

- Treble and Middle tone share the same capacitor `C1`.  Since they are both now .022 µF, they can utilize the same capacitor, which is an old Fender trick.  In their case, they are saving a couple pennies on a component and also avoiding doubling up the capacitance when two tone controls are used together in parallel.  In my case, the combining is not an issue but it does save on a capacitor.

- Addition of a .33 µF blocking capacitor `C4`.  This is a safety measure which I learned about  from [guitarnuts](https://guitarnuts2.proboards.com/thread/4187).  All user-touching components (strings, bridge, knobs, etc) and the shielding are connected to ground as usual but separated from the signal ground by this capacitor.  The purpose is to ~~prevent~~ reduce operator injury if amp voltage ever gets sent back to the guitar over the ground wire path.  Not sure if this is really necessary but they make a good case so I figured why not.

## Components

I have finally accumulated all the necessary components.  I tried to get the most durable, highest-quality parts.

{{<imgresize components.jpg "800x800" "Electronic Components">}}

`C1` .022 µF Polystyrene Capacitor.  This is a new-old-stock MIAL polystyrene, made in Germany probably in the late 1970s.  There are rare to find this big.  I really like polystyrene.  They sound better than anything else in my experience.  Some people like paper-in-oil, some folks like orange drops, and some people say the type does not matter at all and only the value of the capacitance affects the sound.  And they make a great logical case for this argument.  At any rate, these polystyrenes _look_ cool and there is some good counter argument that they are superior for audio.  They are relatively cheap too, compared to other popular types.  (More info [here](https://web.archive.org/web/20260125020221/https://www.electrocube.com/pages/white-paper-what-happened-to-polystyrene-capacitors-data-sheet))   My meter says this one is 22.5 nF.

`C2` 1000 pF silver mica capacitor for the bass tone control.

`C3` Pair of 750 pF silver micas to be used in parallel for the required .0015 µF  in the "Fuzz" tone.  I could not find a nice looking .0015 µF cap for this, so two half-size together works just asPs well.

I did not bother measuring these silver micas. They sound good.

{{<imgresize capacitors.jpg "800x800" "Close up of the tone capacitors">}}

`C4` .33 µF, 630V blocking cap.  Just a run of the mill polyester metalized film.

`J1` Puretone jack

Also shown is the Electrosocket tele-style jack plate.

`SW1`, `SW2`, `SW5` Carling SPDT On/On switches.  These are full size (not huge, but not minis either) and very durable.   I decided to skip using any mini switches and went with these heavy duty guys.  I want this guitar to be rock solid and not need wiring repairs too soon in its lifetime.

I was also worried these large switches would add some extra resistance but they only measure at .2 Ω which is virtually nothing.  I checked some cheap mini switches I had and they were in the .4 to .5 Ω range, so I guess these are higher quality.

Capacitance wise, they are showing .2 nF, although my meter is not super accurate at these low levels.  Mini switches look like around .2 to .3 nF as well.  So I am inferring that these Carling switches will add equal or less unwanted influence on signal quality compared to mini switches.

`RV1` Tokyo Cosmos, 1 MΩ Audio-Taper pot, for the mid tone.  These "TOCOS" are rather high end and cost $10 each.  I have not used them yet but they feel smooth and should sound good and not crap out in the near future.  Checked on my meter, this one actually measures at a resistance of .894 MΩ.

`RV2` Tokyo Cosmos, 500 KΩ Audio-Taper pot, for the treble tone.  Actual measured resistance: 472 KΩ.

`RV3` Tokyo Cosmos, 1 MΩ Audio-Taper, for the bass tone.  Actual measured resistance: .955 MΩ

`RV4` Tokyo Cosmos, 500 KΩ Linear-Taper, for the volume.  I find linear taper for volume is more usable than audio taper, which many other people agree with although audio seems to be the more conventionally used taper for volume controls.  To me, the linear volume change is more continuous and does not have the quick spike / drop-off in the "8-10" range that I hear with audio taper pots.  Actual measured resistance: 486 KΩ.

`SW3` AxLabs 6-Lug, 2-Pole toggle switch.  Decent quality toggle switch that can be wired as on-off-on.  And in black!  The superior alternative might be the Switchcraft model like this that is used for double-necks, but is too expensive for now.  This AxLabs switch when engaged is measuring at .35 nF capacitance and .5 Ω resistance.  Probably negligible but technically inferior to other switches?  Interesting...

`SW4` Carling DPDT On/On for the "Firehose" (pickups direct to jack) switch.  Measurements same as the SPDTs.

### Knobs

All black, solid aluminum knobs here.  The 1/2 inch diameter are for the tone controls.  This is smaller than usual, but I think still usable and fits the aesthetic.  The volume is 3/4 inch, which is a bit more normal size.

I wonder if the lack of numbers will bother me.  I do like to get a sound dialed in and being able to get it back by turning to a specific number.  We will see.

The real issue is how to fit all this into the guitar.
