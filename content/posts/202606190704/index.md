---
title: "DPDT On-On-On"
date: "2026-06-19T12:04:36Z"
cover: ""
tags: ["wiring", "switches"]
series: []
keywords: []
description: "Notes on this unusual yet useful type of switch"
showFullContent: false
readingTime: false
draft: false
---

This is a switch that:

- Is classified as dual-pole, dual-throw (DPDT) having 6 total connection pins
- Has three actuator positions (up, center, down)
- The center position makes contact between certain up and down pins, different from the more common on-off-on where the center position makes no contacts

The most commonly available form of this switch is the "mini" size, having a 6.35 mm bushing with 1/4-40 threads, fitting in 1/4 diameter holes.

[Example](https://lovemyswitches.com/taiway-dpdt-on-on-on-switch-solder-lug-long-shaft/):
![Taiway mini DPDT On-On-On](https://cdn11.bigcommerce.com/s-rsm98uvo0c/images/stencil/500x659/products/355/1966/taiway-dpdt-on-on-on-long-solder-lug-toggle-switch-100-dp6-t100b1m1qe__06307.1674688914.jpg?c=2)

Similar "large-bat" models are more unusual but not too hard to find, that have a 15/32-32 threaded bushing and fit in 1/2 inch diameter holes.

## How the pins are connected

Schematically, the switch is represented by a symbol derived from a pair of SP3T switch symbols, with the center connector pins removed and permanent jumped connections between certain outer pins.

The default view being the "down" position.

{{<imgresize DPDT_on_on_on_symbol.png "400x400" "DPDT On-On-On Schematic">}}

## Table of Connections

|**Position**|**Connected Pins**|
|------------|------------------|
|Down        | 1-2, 4-5         |
|Center      | 2-3, 4-5         |
|Up          | 2-3, 5-6         |

## Mini switch types

These come in two "types", which refers the how the connections are physically laid out in relation to the pins.  This is not an industry standard but a more community-established terminology, so manufacturers will not specify this distinction.

Note how the center positions differ.

{{<imgresize type_1_type_2_physical_connections.jpg "600x600" "Type 1 and Type 2 Physical Connections">}}

**Important**: This "type" difference refers only to the physical orientation and NOT the numbered pin connections.  **They are schematically equivalent!**

The only difference is what pin you decide to be "pin 1" and which ends you designate as up or down.

{{<imgresize type_1_type_2_pin_numbering.jpg "600x600" "Type 1 and Type 2 Pin Numbering">}}

Either way, the pin connection numbers match.

## The AxLabs 2-Pole 6-Lug Toggle Switch

[This](https://axlabshardware.com/products/axlabs-3-way-6-pole-toggle-switch?variant=43872761905410) is another DPDT On-On-On useful as a guitar pickup selector, in the form of a spring-leaf switch.

![AxLabs 2-Pole 6-Lug Toggle Switch](https://axlabshardware.com/cdn/shop/files/AX-TS-3W-6P-N.jpg?v=1776711147)

There are 6 spring leaves each exposing a solder lug.  Two lugs are exposed on one side (left in the above picture) and four on the other.  (A seventh ground lug on one side connects to the frame).

The leaves are stacked such that they can be numbered logically 1 through 6.  The most sensible numbering to me is to start with either of the two outermost lugs and continue circularly.

My numbering:

{{<imgresize axlabs_lugs.jpg "400x400" "AxLabs toggle switch lugs numbered">}}

Interestingly, the switch comes with lugs 3 and 4 bent together, assumed to aid in wiring a typical neck/parallel/bridge pickup selector.  These can easily be separated for different scenarios.

Examination of the positions and how the leaves connect confirms that it is indeed a standard DPDT On-On-On switch. (My numbering.)

{{<imgresize axlabs.jpg "800x800" "AxLabs toggle switch pin connections">}}

I had to deduce all of the above information since AxLabs only provides pictures and no instructions on how to use this switch.

## Additional Notes

- DPDT On-On-On Can be substituted for a SPDT On-Off-On. This is what I did on my guitar to get two pickups in series in the center position.
