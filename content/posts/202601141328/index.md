---
title: "Bridge Design"
date: "2026-01-14T19:28:29Z"
cover: ""
tags: []
series: ["Electric Guitar Build 2025-2026"]
keywords: []
description: "Evaluating multi-scale guitar bridge options"
showFullContent: false
readingTime: false
draft: false
---
In this post I will share some of the decision process used to select the type of bridge used on the guitar.

## Background

The bridge of a multi-scale guitar needs to accommodate the different string lengths, and cannot simply be perpendicular to the strings like on a normal guitar.  More specifically, the saddles themselves are not all the same distance from the nut-end of the neck.  For this specific guitar, the bridge-end of the strings form a 14 degree angle.

This requires some special treatment for the builder, since most off-the-shelf bridges will not work.  There are a few bridge options that can be purchased, the option of a custom-made bridge, or the option of making my own.

### MIDI Guitar

This adds another twist to the thought-process.  I have been considering making the guitar a MIDI controller as well.  I have been looking into the [GraphTech Ghost](https://graphtech.com/products/ghost-pickups-strat-tele-2-1-16-spac) saddles, which have Piezo transducers embedded within them which allows sending to an acoustic preamp board or a MIDI converter through their "Hexpander" board.  GraphTech has a [system of modular components](https://graphtech.com/collections/ghost-pickup-systems-kits/products/ghost-acousti-phonic-hexpander-preamp) that work with these saddles.

#### Ghost Saddles

![GraphTech Ghost saddles](https://graphtech.com/cdn/shop/products/PN-8000-00.jpg?v=1587572523)

These saddles essentially allow you to send a signal for each individual string.  The saddles connect to a circuit board in the guitar (the Hexpander) which outputs to a 13-pin MIDI connector jack.  The 13-pin connector from the guitar goes to an external MIDI converter which takes the string signals and outputs midi events which are then sent to a synth.  The 13-pin is somewhat of a standard, and there are converter units available such as from Roland, Yamaha, and Axon.  (None of this is inexpensive.)  I believe this GraphTech system is used in the Parker Fly guitars.

#### Hexpander Kit

![GraphTech Hexpander board](https://graphtech.com/cdn/shop/products/pe-0440-00-a.jpg?v=1587572508)

I have not fully decided on this route, but it would be nice to have this option later and using an appropriate bridge now will make this much easier.

## Requirements

- Strat-style saddles
- 14 degree angle

Nice-to-haves:

- Slot for Piezo wires (Ghost Saddles)
- Inexpensive

## Options

### Hipshot Multi Scale Bridge

![Hipshot Multi Scale Bridge](https://hipshotproducts.com/cdn/shop/products/4MS06110B.jpg?v=1504663820&width=1280)

https://hipshotproducts.com/collections/guitar-bridges/products/6-string-multi-scale-fixed-guitar-bridge

This was my initial first choice when planning the guitar project.

It comes in 11 degree option which is not exactly the 14 I need, but it would be close enough.

Pros

- Seems like a solid, well-made bridge
- Low risk of making a bad choice

Cons

- Somewhat expensive, just over $100
- Does not have slots for Piezo wires, would need to modify
- Would require additional cost to upgrade to Ghost saddles

### Hipshot Solo Bridges

![Hipshot Solo single string bridge](https://hipshotproducts.com/cdn/shop/products/4S100B.jpg?v=1748958268&width=1280)

 https://hipshotproducts.com/collections/guitar-bridges/products/solo-single-string-guitar-bridge

With these, you buy one for each string and position them individually on the guitar according to the spacing and angle required.

 Pros

- Can be mounted to form any custom angle
- Built-in slots for Piezo wires
- Grooves for height-adjustment screws seems like a nice detail
- Supports top-loaded strings in addition to body-through (cool, although unneeded)
- Can be purchased individually

Cons

- Expensive.  $25 to $30 EACH.  (But again, I could by them one-by-one over a few months and spread the cost out)
- Would require additional cost to upgrade to Ghost saddles

Overall, I think is the best option, barring the cost.

### Other Off-The-Shelf Options

There are a few other multi-scale bridge solutions available to buy.  I am ruling them all out due to  their cost and other various reasons why I do not like them.

#### ABM Single Bridge

![ABM Single Bridge](https://abm-guitarpartsshop.com/images/product_images/popup_images/3210b_1.jpg)

https://abm-guitarpartsshop.com/ABM-GUITAR-PARTS/Single-Bridges/Guitar/ABM-3210/ABM-3210b-Black::229.html

#### Guyker Headless Guitar Bridges

![Guyker Headless Guitar bridge](https://www.guyker.com/cdn/shop/files/CNC_Aluminum_Alloy_Headless_Guitar_Bridge_with_Brass_Saddles_Guyker-1.jpg?v=1767773600&width=800
)

https://www.guyker.com/products/guyker-wt003-cnc-aluminum-alloy-headless-guitar-bridge-with-brass-saddles

#### Musiclily

![Musiclily bridges](https://m.media-amazon.com/images/I/81pRab0g1UL._AC_SL1500_.jpg)
https://www.amazon.com/Musiclily-Non-tremolo-Individual-Separable-6-Saddle/dp/B0CCS3WG2G

## DIY Bridge

It seems feasible that I could make my own simple bridge from brass bar/sheet stock.  I could color it black using Birchwood-Casey Brass Black.

I would need to buy the saddles, though, but could get the Ghost saddles right away, or could start with GraphTech string-savers and upgrade to Ghosts later.

Pros

- Lower cost
- Will be at correct angle
- Full control of design / can be as simple as needed
- Can use whichever saddles I want without having to "buy" extra that come with an premade bridge

Cons

- Probably will not look as clean as a machined bridge
- More risk in mistakes
- Potential downside of making unconventional holes/routes into the guitar body that would not be compatible or covered by another type of bridge if I ended up buying.

### V1

Here is my first go at a design.  It is basically two pieces.  One is a 1/4 inch thick brass bar that the saddles screw into.  I am thinking it can be partially embedded into a routed slot in the guitar body.  The other piece is a 1/8 thick brass plate for the saddles to rest on.

The main gist of this design is that the holes for the saddle screws are drilled at the required 14 degree angle, and slightly countersunk on both sides for the screw-head and spring to sit into.

{{<imgresize diy-bridge-design.jpg "800x800" "Drawing of diy bridge design">}}

I thought about trying to replicate the design of the HipShot Solo saddles.  This seems to require a bend or removing a lot of metal to get the right-angle shape.  I am not an metal expert, but believe bending 1/8 thick brass is a no-go unless it is anealed.  I am not skilled in this practice so am ruling it out.  In short I do not think the HipShot Solo bridge is a feasible design for me to produce.

### V2

I soon realized that I could use individual saddle mounts instead of a single solid bar.  Some 1/4 inch round brass rod with a hole through the side might work.

{{<imgresize diy-bridge-design-2.jpg "800x800" "Drawing of diy bridge design, version 2">}}

3/8 rod would probably be better.  In addition to the hole for the saddle screw, the ends of the hole will need to be drilled wider for the screw head and spring.

Top view showing hole-through, with ends drilled wider:

{{<imgresize bridge-post.jpg "400x400" "Drawing of diy bridge post showing hole profile">}}

All that remains now is some brass plate for the height adjustment screws to bear upon.  This does not need to be a single piece either.  Some small, minimal plates might work, if they could be attached cleanly.

#### Barrel Nuts

There are actually pre-made hardware objects that are almost exactly to this spec.  They come in black, too.  I have not been able to find the exact size needed though.

![Black barrel nuts from Amazon](https://m.media-amazon.com/images/I/71tlR5Kg3kL._SL1500_.jpg)

https://www.amazon.com/Mardatt-Barrel-Zinc-Plated-Slotted-Furniture/dp/B0FBFTLKY1

I have also seen these nuts in an "offset" version where the hole is closer to one end, almost just like my design.  If I could find these in black, it might be ideal.

Incidentally, I used one of these to attach the mortise-and-tenon neck on my Super K guitar (à la [Cumpiano](https://www.cumpiano.com/an-improved-neck-body-joint)).  These furniture fasteners seem to keep coming up.

## Custom Made Bridge

Another option is to design my own bridge, or individual parts, but get [SendCutSend](https://sendcutsend.com/) to make them for me.  I have used them before for an acrylic fret spacing template and they provide a great service at very reasonable prices.

Pros

- Can get the exact design I want
- Can use whichever saddles I want without having to buy extra

Cons

- Requires learning how to 3D-CAD an object (this could be considered a pro actually)
- Most likely prohibitively expensive