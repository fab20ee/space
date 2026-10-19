---
title: "InfiRay T2S+ Thermal Camera"
seoDescription: "The InfiRay T2S+ thermal camera at the Tallinn hackspace: clips onto a phone, 256 × 192, 12 µm pixel, manual focus over a wide range. See what is getting hot on a board."
specs:
  - { label: "Sensor",      value: "256 × 192" }
  - { label: "Pixel",       value: "12 µm" }
  - { label: "Connection",  value: "USB-C, straight into the phone" }
  - { label: "App",         value: "Xtherm (Google Play), free" }
  - { label: "Lens",        value: "manual focus over a wide range" }
  - { label: "Storage",     value: "a hard zip case" }
---

A module the size of an eraser that plugs into a phone's USB-C port and turns it into a thermal
camera. A 256 × 192 sensor is 49 thousand points where temperature is measured, and for
electronics that is more resolution than you usually need.

The real point of the T2S+, though, is its **manual focus over a wide range**. Most clip-on
cameras, including distinctly more expensive ones, are fixed focus, and on a dense board that
means a blurry smear instead of a component. Here the lens turns, so you can focus until
individual packages are distinguishable and you can tell which one is the hot one.

A thermal camera answers questions nothing else will. Which of the forty parts on the board is
getting hot. Where exactly the bad contact in a cable is. Whether a chip is working at all or just
sitting there cold. What is happening inside an enclosure you cannot open while it runs.

## What it is good for

- Finding the part that overheats on a board: it shows up at once, long before anything smells
- Catching a short circuit — the shorted spot heats first
- Checking whether a 3D printer's heated bed warms evenly
- Seeing what actually runs hot inside a power supply under load
- Finding a cold solder joint by the fact that nothing past it warms up
- Household work: heat leaking round a window, underfloor heating, a blocked radiator

## How to use

1. Take the module out of its case. The phone is your own, and it needs a USB-C port.
2. Install **Xtherm** from Google Play — it is free.
3. Plug the module in. The app starts by itself, or asks for permission to use the device.
4. Aim it and **turn the lens ring**: focus here is manual, and an out-of-focus thermal camera
   shows a blurry smear instead of a component.
5. Capture frames in the app; they are saved to the phone.
6. Put the module back in its case and the case back in the container.

A phone with the app already installed and set up is due to join it in the same container — after
that you will not need to get your own out.

## What to understand about the readings

A thermal camera measures **radiation**, not temperature directly, and converts one to the other
through an emissivity figure. For a board, for plastic and for paint it is close to the truth. For
shiny metal it is not: a polished heatsink shows the temperature of whatever is reflected in it
rather than its own. To measure something shiny, stick a piece of matt tape on it and look at
that.

Glass is opaque to thermal radiation: through a window or a glass lid you see the temperature of
the glass itself.

## Renting it

The module goes home with you: usually to see what runs hot in your own equipment, or to find the
cold spots in a flat. The phone is yours and needs USB-C. The daily rate and the term are in the
rental block on this page.

## Access

The module is in a container on the shelf in the hackspace room, so a plan that includes hackspace
access is required. No induction is needed.
