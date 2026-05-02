---
title: "Sound Test - With Audio"
date: "2026-05-02T15:06:04Z"
cover: ""
tags: []
series: ["Electric Guitar Build 2025-2026"]
keywords: []
description: "Some sound samples from testing the circuit"
showFullContent: false
readingTime: false
draft: false
---

## Sound Test

[Jump down to the recordings...]({{< ref "#sound-samples" >}})

## Circuit Test Rig

For testing I attached JST-SM connectors to the pickup leads, as well as one from the string-ground/shielding wire.  These make convenient and stable test connections - much better than alligator clips.

Recall that of these pickups has three wires:

- full output
- tapped output
- ground

{{<imgresize test_connectors.jpg "800x800" "Pickups connected with JST-SM connectors">}}

Here is a photo of the test rig.  It looks like a big mess, and it kind of is.

{{<imgresize test_rig.jpg "800x800" "Circuit testing rig">}}

From the bottom right, and moving counter-clockwise:

### 1. Input switch box (copper colored square with the white breadboard on top)

The pickups go directly into this.  It lets me switch each pickup between the full and tapped output, and also has a three-way switch to select each pickup individually or combine both in series.

### 2. Neck and Middle Tone  (white box, red breadboard)

This consists of a rotary switch for selecting different capacitors and a pot for the amount applied.

This is coming out of the series connection and affects the neck pickup as a tone control, acts like a mid-cut when the pickups are together, and has no effect on the bridge pickup alone.  It seems pretty useful in that I can have the neck pickup with a lot of tone applied but then switch to the middle or bridge position a still have a bright sound.  

I currently have a .005, .015 and a .022 capacitor in this, and I think I like the .022 here.  

1 MG pot, too, so when it is on 10 it has virtually no attenuation.

### 3. Main output module (large breadboard)

This has the output jack and various pots and such that I am using for bass-cut tone control and the master volume control (the last two components in the circuit).

Volume is a 500k linear pot.

Bass cut is a 1 MG pot with an 1100 picofarad capacitor in parallel with the signal.  I tried a few cap values and this one seemed the best.

### 4. Tone Control Tester (black box)

This is another tone tester with a rotary switch and pot.  I am using it for the master tone control, which affects all pickup combinations.

Caps are .015 and .022.  I am leaning towards the .015 in this case.  I also tried a .044 and as expected did not like the amount of mid range it removed.

500K audio pot.

### 5. Direct Out Switch (blue breadboard)

This is comes next in line after the pickup selector, and allows completely bypassing all the volume and tone controls so the pickups goe directly to the jack.  I really like this option since it gives such a pure, bright, and LOUD sound at the flick of a switch.

Actually, that neck/middle tone stays in the circuit since it comes in parallel with this switch, so the real direct-out only happens when the bridge pickup is selected by itself, but that is ok.

## Sound Samples

Here are some recordings of me noodling around.  In each case, I started with the pickup(s) direct out, and then applied various combinations of volume, tone, and tap switching.

### Neck Pickup

{{< blog_media_audio filename=ElectricGuitar20252026Test_NeckPickup.flac >}}

---

### Pickups Together

{{< blog_media_audio filename=ElectricGuitar20252026Test_BothPickups.flac >}}

---

### Bridge Pickup

{{< blog_media_audio filename=ElectricGuitar20252026Test_BridgePickup.flac >}}

---

These were recorded with no amp directly into an Audient ID4 audio interface into Ardour, with no signal processing applied at all.

The "reverb" you might hear is just the strings themselves resonating sympathetically which is how I tend to play.

The electric buzzing / static noises are due to all the unshielded wires in the test rig, and should not be present in the completed guitar.

I will record some more tests through an amp soon.  And maybe play some actual tunes.
