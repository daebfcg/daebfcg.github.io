---
title: "Installing Electronics"
date: "2026-06-06T02:09:21Z"
cover: ""
tags: ["wiring"]
series: ["Electric Guitar Build 2025-2026"]
keywords: []
description: "Wiring up the pickups and controls into the guitar"
showFullContent: false
readingTime: false
draft: false
---

The components were placed on the mdf template and the solder connections made.  The wiring was done if four phases.

1. Shield/Grounding (green wire)
1. Signal connections (yellow wire)
1. Signal return ground (black wire)
1. Capacitors (black wire)

It is quite a rats-nest once it is all together.

{{<imgresize assembly.jpg "800x800" "Components assembled">}}

A couple last-minute changes from the schematic:

1. I skipped adding the resistor to the volume pot to drop it to 333k, and just left it at the 484k it is.

1.Instead of the "blocking capacitor" I found something that seems a bit better, [this guy](https://avjoy.biz/safety-circuit.html) which uses a 220k resistor and a .022 cap in parallel for shock prevention.  It is even mentioned in a Dan Erlewine book that I have, so it must be legit.

## Grounding the Tokoy Cosmos pots and the Carling switches

To create a solid connection to the shielding ground (the user-touchable components) I added some homemade thin copper lugs to the bushings of the pots and switches that get wired to a single lug that is screwed into the side of the guitar into the shielding.  This lug is then attached to the signal ground at the jack via the aforementioned safety-connector.

So in theory touching the metal pot shafts or metal knobs, and metal switch actuators will not be directly connected to the signal ground, but instead connected to the shielding ground which is effectively grounded but has the cap/resistor in between for safety (and possibly noise isolation).

The Tocos pots are a bit unusual in that the backs of the cases are metal but are not electrically connected to the bushings and shaft.  Usually these have continuity so by grounding one you ground the other.  I did not feel like soldering a wire between these points for fear of damaging these pots, so used a bit of the copper shielding tape to make a connection between the back casings and the bushings.  This might be overkill, since the guitar cavity is fully shielded and the pot backs probably will not be picking up interference.

## Installation

Once the circuit is all wired up, I had to get it into the guitar cavity.  The was a horrendous process but it worked in the end.

{{<imgresize installation.jpg "800x800" "Installation">}}

And it is in!

{{<imgresize installed.jpg "800x800" "Components installed">}}

Amazingly it all worked as expected.

The only slight glitch was the pickup selector toggle.  For some reason, in the bridge position the leaves 1 and 2 were not making solid contact, and getting some neck pickup bleed through.  Not sure what happened, but I managed to fix it by pushing the leaf and bending it back into place for a tighter connection.

## Wiring Done

Got all the knobs back on and now to play it for a while.

{{<imgresize done_detail.jpg "600x600" "Wiring done">}}
