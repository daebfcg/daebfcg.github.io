---
title: "Drawing Schematics"
date: "2026-05-10T13:35:56Z"
cover: ""
tags: ["wiring"]
series: ["Electric Guitar Build 2025-2026"]
keywords: []
description: "Using KiCad Schematic Editor"
showFullContent: false
readingTime: false
draft: false
---

My first schematic, made for the guitar circuit.

{{<imgresize schematic.png "800x800" "Schematic">}}

## KiCad Schematic Editor

I am just recently getting comfortable reading and creating schematics.  I found a nice oss editor that is part of the KiCad suite of tools.

{{<imgresize kicad.png "800x800" "Screenshot of KiCad Schematic Editor">}}

This program seems good although there is some learning curve.  It is helpful to know the keyboard commands for the various tools.  The most useful is "A" to place an item.  You hit A and are presented with a modal that lets you pick from thousands of various schematic symbols.

{{<imgresize symbol_dialog.png "800x800" "Screenshot of symbol selector dialog">}}

To draw a wire between components, you enable the Wire tool by hitting W.  It is best to have the cursor ON the pin where you want the wire to start.  This is because you do not click down to draw like a typical drawing program, but instead it just starts making a wire as you move the mouse starting with where you were when the tool was enabled.

{{<imgresize wire_tool.png "800x800" "Wire tool">}}

### Escape

**Important Tip:** Any time you want to get back to the main Select tool, just hit **ESC**.

### Deleting

One annoying aspect is that anytime you click a wire it automatically puts you into Wire tool mode, and is is easy to draw bunch of unwanted wires.  Deleting short little wires is harder than it seems like it should be.

{{<imgresize wires.png "800x800" "Small wires hard to delete">}}

### Export

Oddly, it does not export to an image file, but instead image data to the clipboard.  Not a big deal, just and extra step to create image for use in another program.
