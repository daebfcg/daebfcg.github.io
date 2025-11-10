---
title: "Electronics Plan V1"
date: "2025-11-10T13:36:33Z"
cover: ""
tags: []
series: ["Electric Guitar Build 2025-2026"]
keywords: []
description: "Initial idea for the guitar controls"
showFullContent: false
readingTime: false
draft: false
---

Some cold weather today so I am staying out of the shop and taking a closer look at the electronics planned for the guitar.  Once the guitar is fully assembled and strung up for the first time (before finishing, though) I will see what it sounds like and test out different circuits and components using an external breadboard before drilling the final holes for the potentiometers (pots) and switches.

## Initial Idea

{{<imgresize electronics-layout-800.jpg "800x800" "initial idea for electronics">}}


### Pickup Selector Toggle

This is a Les Paul style [three-position toggle](https://www.stewmac.com/electronics/components-and-parts/switches/axlabs-3-way-6-pole-toggle-switch/) for the neck pickup, bridge pickup, or both in parallel. Black.  I considered other options such as individual on/off switches for each pickup or a Telecaster-style blade pickup, but landed on the toggle with the idea that it is the most fool-proof way to easily flip while playing.  The exact placement will be determined once I actually try to play the guitar to see where my hand goes when moving my elbow to get it in just the right spot.  I will also angle switch movement so as not to make it _too_ easy to flip to avoid accidentally switching it during vigorous strumming.

### Neck and Bridge Tap Switches

These will be [mini on/on toggle switches](https://lovemyswitches.com/taiway-dpdt-on-on-switch-solder-lug-short-shaft-black-plated/) to control the pickup taps.  The plan is to use [Seymour Duncan Quarter Pound Strat](https://www.seymourduncan.com/single-product/quarter-pound-strat
) Tapped pickups, which have a normal, modern high-output lead plus an additional tapped lead for a more vintage half-power output.  This will allow the player to get two different sounds out of each pickup.  I expect the normal (up) position will be more suitable for modern high-gain styles and the tapped (down) will produce more a traditional clean/jangly strat-type sound.

### Tone ByPass

Mini on/on toggle that will allow bypassing the tone circuit completely.  When down, the normal tone and volume signal path is active.  When switched up, the tone controls are bypassed and have no effect, so only the volume control is in the circuit.  The thinking is that tone controls do attenuate the signal even when turned all the way up, because the resistance of the pots is not infinite and some signal is still getting grounded.  Add in the capacitors, and there _is_ tone being changed even when the tone is on "10".  So this allows the player to get an even more pure and raw signal from the pickups without any influence by the tone controls.  Only the volume control still works.

### Tone Knob 1 - Bass Cut

This is a bit different from a normal single-tone control on a guitar.  This guitar will have separate treble and bass controls (passive).  This is directly copying the G&L S500 wiring.  Most guitars just have a single tone control which attenuates the high frequencies.  Here with the additional bass-frequency attenuation, the player will be able to clean up the signal to cut through a mix better by cutting out some bass.  This will be a 1MG Ohm audio taper pot, with a small capacitor around 1000 picofarads.  When testing the circuit I will determine the best capacitor value.  Black, [20mm aluminum knobs](https://lovemyswitches.com/anodized-aluminum-knob-the-hi-fi-1-4-smooth-shaft-20mm-od/) for the tone controls.

### Tone Knob 2 - Treble Cut

This is the more traditional tone control that just cuts the high end.  I am thinking 500k audio-taper pot, with a .022 microfarad capacitor.  Again, will experiment to find a good sounding capacitor.

### Volume

Basic volume control.  250k linear pot.  I prefer linear pots for volume, as opposed to audio-taper.   Note the large knob... I am thinking of using [freakishly large 32mm knob](https://lovemyswitches.com/solid-aluminum-knob-mission-control-1-4-smooth-shaft-32mm-od/) for the volume to allow the player to easily grab it with their pinky finger while playing to do dramatic volume swells.

### Direct Out

One last on/on toggle switch near the volume, which will bypass both the volume and tone from the circuit and send the pickup signal directly to the jack.  This is for an even more pure, raw signal unaffected by any pots or capacitors.   This can act as a mini "boost" effect during a performance.  Used this way, it is sometimes called a blower switch.  It might also be useful for recording, where all tone and volume is controlled during mixing and you want the purest and loudest signal to be recorded.

### Jack

I am thinking of trying one of these [PureTone](https://www.amplifiedparts.com/products/jack-pure-tone-mono-open-circuit) jacks.  In black of course to match all the other hardware.  The jack will be in the side of guitar, Telecaster style, using a nice [recessed plate](https://www.stewmac.com/parts-and-hardware/jack-plates/electrosocket-jack-mount/).

## Breadboarding

What I usually do is mount the pickups into the guitar and connect the leads to a breadboard tester on my desk, which is then connected to an amp.  The allows me to fiddle around with different components and wiring schemes before soldering anything. 

More photos and updates to come on this subject.
