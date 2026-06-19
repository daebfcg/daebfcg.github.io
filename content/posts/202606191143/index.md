---
title: "Mid Tone Control"
date: "2026-06-19T16:43:12Z"
cover: ""
tags: ["wiring"]
series: []
keywords: []
description: "A Passive Mid-Tone Guitar Control"
showFullContent: false
readingTime: false
draft: false
---

I first came across this when researching wiring two pickups in series.  I found [this post on TDPRI](https://www.tdpri.com/threads/2-humbucker-series-wiring.953573/post-9121393) where a forum member shared their schematic titled "Kay Catalina 2-pickup modded".  The schematic shows an unusual, additional tone control labeled TAP that comes from the series-junction pin of the toggle switch.

I finally learned that this does the following, based on the toggle switch position:

- Bridge Only - nothing
- Center (pickups in series) - mid tone control
- Neck Only - additional tone control

I was skeptical, but when I tried this it absolutely did act as a very useful mid tone control when the two pickups were in series.  To me this actually makes the combined pickups usable.  I usually find the center position the least favorable mode of all my 2-pickup guitars, regardless of them being series or parallel.

On my latest guitar with two single-coil pickups in series, the sound has a pronounced honky quack, i.e that classic, signature Stratocaster sound.  Which can be good, but also not so good.  With this mid control, I can reduce or completely dial out the quack and get new, cleaner sounds from the two pickups in series.

This control has turned out to be an indispensable feature of that guitar.

## Schematic

In its most basic, stripped down form, the control is this:

{{<imgresize lc_filter.png "800x800" "Mid Tone Control">}}

A typical RC filter tone control but connected to the series junction of the two pickup coils.

I am not an electronics expert by any means, but I **think** this is actually making an LC Filter (inductor-capacitor), which cuts middle-range frequencies.  The inductor part of the LC is from one of the pickup coils.

## Future Experiments

I do not know why this would not also work when connected to the series-junction wires on a humbucker pickup.  And if so, why is this not more widely used?
