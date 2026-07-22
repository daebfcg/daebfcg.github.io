---
title: "Slide Switch - 3-Position"
date: "2026-07-20T16:41:44Z"
cover: ""
tags: ["wiring"]
series: []
keywords: []
description: "Notes on the Switchcraft DPTT 3-position switch - How it works and potential uses"
showFullContent: false
readingTime: false
draft: false
---

## The Switchcraft 11D1049X

![Switchcraft 11D1049X](https://www.switchcraft.com/assets/1/24/DimRegular/11D1049X.webp?11263)

<https://www.switchcraft.com/fender-mustang/11d1049x/>

- Dual Pole, Triple Throw
- 8 pins
- Also known as the "Fender Mustang" switch
- Good source: <https://www.amplifiedparts.com/products/slide-switch-switchcraft-dptt-3-position>

## How it Works

### Schematic Symbol

{{<imgresize dptt_schematic.png "300x300" "Schematic of the DPTT swtich">}}

The pin connections, visualized:

{{<imgresize positions.png "300x300" "Visualization of pin connections by position">}}

### Table of Connections

|**Position**|**Connected Pins**|
|------------|------------------|
|Up          | 1-2, 7-8         |
|Center      | 2-3, 6-7         |
|Down        | 3-4, 5-6         |

Notably, this switch has no _common_ pins unlike most switches.  It is not to be confused with some types of DP3T sliders that have pins 3 and 7 configured as always connected to one other pin.

### Is it On-On-On or On-Off-On?

Yes.

---

## Uses

Here are a collection of schematics from on-line examples and some of my own ideas.

### Pickup Phase Reversal

Used in Fender Mustang wiring.

By itself (alone, or other pickup off), up or down are the same.  When combined with another pickup and one is up and the other down, the pickups are out of phase.

{{<imgresize Phase_Switch.png "400x400" "Phase Switch">}}

|**Position**|**Function**            |
|------------|------------------------|
|Up          | On                     |
|Center      | Off                    |
|Down        | On (reverse phase)     |

---

### Pickup Selector

{{<imgresize Pickup_Selector.png "400x400" "Pickup Selector">}}

|**Position**|**Function**            |
|------------|------------------------|
|Up          | Pickup A only          |
|Center      | A+B, in parallel       |
|Down        | Pickup B only          |

---

### Series/Parallel switch

See [Mod Garage: Rewiring a Fender Mustang](https://www.premierguitar.com/mod-garage-rewiring-a-fender-mustang).  Technically, this could be done with a 2-position switch.  The implementation of this mod uses the existing switch in the guitar.

---

## Ideas

What follows are some ideas for this switch that I thought of in the context of having dedicated `on`/`something`/`off` switches for each individual pickup on a guitar, inspired by 60s Japanese guitars.

To me it seems most intuitive to have the `off` position last.

### Pickup: On, Half-Out-Of-Phase, Off

This is similar to the original Fender Mustang Phase Switch wiring above, except that it:

1. Uses the so-called half-out-of-phase (HOoP) capacitor trick instead of all the way out, for a more usable sound (minimal volume drop).
1. Puts the modes in order of **most-signal to least-signal** instead of `off` being in the middle.

Again, note that the OoP effect happens when used in conjunction with another pickup that is in normal phase, either in parallel or series.

{{<imgresize HOoP_Switch.png "400x400" "HOop Switch">}}

`C1` approx .01 µF

|**Position**|**Function**            |
|------------|------------------------|
|Up          | On (In Phase)          |
|Center      | On (Half out of Phase) |
|Down        | Off                    |

---

### Pickup: On, On + Treble Cut, Off

Works by adding a capacitor to ground in parallel with the signal path, to cut high frequencies.  Intended to be used with a smaller value cap to shave off just a bit of the top end, giving a [boosted resonant peak effect]({{< ref "posts/202605121328/" >}}).

{{<imgresize Treble_Cut.png "400x400" "Treble Cut Switch">}}

`C1` approx .0015 µF

|**Position**|**Function**            |
|------------|------------------------|
|Up          | On (normal)            |
|Center      | On (treble-cut effect) |
|Down        | Off                    |

---

### Pickup: On, On + Bass Cut, Off

In the center position, adds a capacitor in series with the signal to cut out some of the lower frequencies.

{{<imgresize Bass_Cut.png "400x400" "Bass Cut Switch">}}

`C1` approx .001 µF

|**Position**|**Function**            |
|------------|------------------------|
|Up          | On (normal)            |
|Center      | On (bass-cut effect)   |
|Down        | Off                    |

---

### Pickup: On, On + Mid Cut, Off

For when the pickup is **next** (i.e. not the first) in a **series** of pickups.  The [mid-cut effect]({{< ref "/posts/202606191143" >}}) relies the capacitor-to-ground being between two pickups in series.

{{<imgresize Mid_Cut.png "400x400" "Mid Cut Switch">}}

`C1` approx .022 µF

|**Position**|**Function**            |
|------------|------------------------|
|Up          | On (normal)            |
|Center      | On (mid-cut)           |
|Down        | Off                    |

---

### Pickup: On (Full output), On (Tapped output), Off

Useful for pickups with tapped outputs.  Order of modes goes from **most to least** output.

{{<imgresize Tap_Switch.png "400x400" "Tap Switch">}}

|**Position**|**Function**            |
|------------|------------------------|
|Up          | On (Full)              |
|Center      | On (Tapped)            |
|Down        | Off                    |
