---
title: "Control Layout"
date: "2026-05-06T11:47:45Z"
cover: ""
tags: []
series: ["Electric Guitar Build 2025-2026"]
keywords: []
description: "Thoughts on the knobs and switches and their arrangement on the guitar"
showFullContent: false
readingTime: false
draft: false
---



## Version 1

{{<imgresize layout_1.jpg "600x600" "Control Layout 1">}}

1. Pickup Selector toggle switch (neck/series/bridge)
2. Neck Pickup Tap switch (up: full, down: tapped)
3. Bridge Pickup Tap switch (up: full, down: tapped)
4. Direct Out switch (up: direct out, down: normal)
5. Volume (.75 inch diameter knob)
6. Treble tone (.5 inch knob)
7. Middle tone (.5 inch knob)
8. Bass tone (.5 inch knob)

I like the grid-arrangement of these, although it might be somewhat congested.  Ideally the hand would not accidentally hit another control when trying to make an adjustment to one.

I like the direct-out being down at the bottom where it is out of the way, but easy to get to quickly when needed.

## Version 2

{{<imgresize layout_2.jpg "600x600" "Control Layout 2">}}

1. Pickup tap combo (4-position rotary switch with .5 inch knob)
2. Treble tone
3. Middle tone
4. Bass tone
5. Volume
6. Pickup Selector toggle
7. Direct Out switch

### Rotary Option

Since there are four total combinations of pickup-tap selections, I realized the two tap switches could be combined into one 4-way rotary switch.  

The combinations are:

1. Neck Full, Bridge Full
1. Neck Full, Bridge Tapped
1. Neck Tapped, Bridge Tapped
1. Neck Tapped, Bridge Full

Since it is a rotary switch, there is no "stop" so you can get from position 4 back to 1 with one turn.

This is one less hole to drill, cheaper, and likely more reliable long-term.  I also find the arrangement can go in a more spaced-out, circular pattern, which is not too bad.

I suspect it would not be as intuitive to use though, compared to two separate up/down switches.  The player would need to remember which position on the dial corresponded to the pickup tap combination.

(I considered a more visually-indicative knob for this such as a chicken-head, but decided it would be aesthetically wrong for this guitar.)

Furthermore with either pickup selected by itself, two sequential positions of the knob could possibly have the same result. In other words with one pickup selected it would require either one **or** two turns to change from tapped to normal depending on the current position.  Only when the two pickups are selected together (using the separate toggle switch) would each position on the rotary give a different result.

### Bonus Capacitor Selector

Another interesting "twist" to the 4-position rotary switch is that [this one](https://www.amplifiedparts.com/products/rotary-switch-3-poles-4-position) is a 3-pole switch.  To  get the pickup tap combinations I only need to use two of the poles, leaving some extra lugs.  One use of these would be to also select different tone capacitors while selecting pickup taps.  This is actually pretty cool because I found that with the pickups in tapped-mode I prefer a higher value capacitor.  So I could have it where when selecting one of the tapped options, the treble tone control would be through a .022 uf cap, but when selecting one of the full output positions, the treble tone would go through a .015 cap.  Or even have four different cap values for each position!

## Knobs

I think I have settled on these black, solid aluminum knobs.

.75 inch diameter for the volume.
![.75 inch diameter](https://www.amplifiedparts.com/sites/default/files/uc_products/p-k311_0.png)
https://www.amplifiedparts.com/products/knob-aluminum-notched-tip-indicator-set-screw-75-diameter

.5 diameter for the rest
![.5 inch diameter](https://www.amplifiedparts.com/sites/default/files/uc_products/p-k655_reshoot_0.png)
https://www.amplifiedparts.com/products/knob-aluminum-set-screw-short-line-05-diameter

## Switches

I was originally planning to use some [mini-toggle switches](https://lovemyswitches.com/taiway-spdt-on-on-switch-solder-lug-short-shaft-black-plated/) for the pickup taps and possibly the direct-out.  I learned more about these and apparently they are not very durable and tend to break during service.  I found some "fat bat" versions [on Amazon](https://www.amazon.com/dp/B0732PBRDF) which seem a bit more solid and have a full 15/32 bushing yet are still in the mini form factor inside.  I think they might be ok for the pickup taps.

Another good looking option for the on-on pickup taps would be these non-mini, [full size Carling switches](https://www.amplifiedparts.com/products/toggle-switch-carling-spdt-short-bat-solder-lugs-3a).  They look great but I think they might be a tight squeeze in the guitar.

That decision on which switches to use for the pickup taps is off the table if the rotary switch is used...

For the pickup selector toggle, I discovered the [AxLabs 2-pole/6-lug toggle switch](https://axlabshardware.com/products/axlabs-3-way-6-pole-toggle-switch) which can indeed be wired as an on-off-on. (And it comes in black!)  The on-off-on is needed to get the two pickups in series.  This is different from a typical two-pickup selector where the middle position puts the pickups in parallel by being on-on-on.  I was thinking I would need to resort to some type of heavy-duty industrial type of on-off-on switch, use a flaky mini-toggle, or modify a standard les-paul type leaf-spring toggle switch to get it to work as on-off-on.  This AxLabs switch was a great discovery.

For the direct-out, I like the idea of also using a leaf-spring toggle switch that is easy to flip, as opposed to a short-fat-bat mini toggle or heavy-duty switch.  Looking at the AxLabs 6-lug switch, I can take it apart and flip one of the leaves and get it to work as (on)-on-on, meaning it essentially has two positions, ideal for the direct-out switch.

The tip of the direct-out switch will be red.
