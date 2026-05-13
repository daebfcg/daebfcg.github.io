---
title: "New Tone Control Option"
date: "2026-05-12T18:28:09Z"
cover: ""
tags: ["wiring"]
series: ["Electric Guitar Build 2025-2026"]
keywords: []
description: "Adding the option to switch between a normal treble tone control and a small direct capacitor"
showFullContent: false
readingTime: false
draft: false
---

This introduces another switch for two useful and distinct treble-tone options.  The added option bypasses the typical treble-tone signal flow and connects the signal directly to ground through a small capacitor.

This sort of mod is often used on Telecasters. I gave it a try and found it **highly effective** for a mid-rangey, cutting, almost fuzzy, searing lead tone.

On this guitar, I found the .0015 µF capacitor worked best, which is coincidentally one order of magnitude smaller than the cap I like for the normal tone.

    1. signal → 500K Pot → .015 µF capacitor → ground.
    2. signal → .0015 µF capacitor → ground.

Alternatively, the switch could be placed after the pot and have it function as a capacitor-selector only, which is often a nice option.  This does add the ability to dial in more or less of the effect of the small cap.  However the small cap is mostly noticeable when the pot is on 0 (no resistance to ground).  So I find it more useful to be able to alternate between the small cap with no resistance and the normal cap with higher/variable resistance just by flipping the switch for a more dramatic change.

## Updated Schematic

Added the "TrebleCap" switch and additional capacitor.

{{<imgresize schematic_20260512.png "800x800" "Schematic with updated tone control">}}

## Example Recordings

### Pickups in series (bridge full, neck tapped), mids 0, bass 10

Original .015 µF cap, treble 10:

{{< blog_media_audio filename=paddy_015_tone10_20260513.flac >}}

New .0015 µF cap direct to ground:

{{< blog_media_audio filename=paddy_0015_20260513.flac >}}

### Bridge pickup only (full), bass on 10

Original .015 µF cap, treble 4:

{{< blog_media_audio filename=paddy_015_bridge_20260513.flac >}}

New .0015 µF cap:

{{< blog_media_audio filename=paddy_0015_bridge_20260513.flac >}}

### A few more for comparison

#### .015 µF cap

Pickups in series (bridge full, neck tapped), mids 0, bass 10, treble 5:

{{< blog_media_audio filename=paddy_015_tone5_20260513.flac >}}

Pickups in series (bridge full, neck tapped), mids 0, bass 10, treble 3:

{{< blog_media_audio filename=paddy_015_tone3_20260513.flac >}}

#### .0015 µF cap

Pickups in series (bridge full, neck full), mids 10, bass 0:

{{< blog_media_audio filename=paddy_0015_mids10_20260513.flac >}}
