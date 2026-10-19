---
title: "Module Box"
seoDescription: "A box of modules for prototypes at the Tallinn hackspace: relay boards, an ultrasonic rangefinder, keypads, battery holders, prototyping boards and assorted parts."
specs:
  - { label: "Actuators",    value: "relay modules, single and multi-channel" }
  - { label: "Sensors",      value: "an ultrasonic rangefinder and other small parts in antistatic bags" }
  - { label: "Input",        value: "a 4 × 4 membrane keypad" }
  - { label: "Power",        value: "battery holders for various cells" }
  - { label: "Building",     value: "prototyping boards and shields, connectors, hardware" }
  - { label: "Contents",     value: "change constantly; this describes types rather than part numbers" }
---

The box for what did not fit in the sensor kit and is not a consumable: relay modules, keypads,
battery holders, prototyping boards, connectors and the rest of the glue that turns a breadboard
into a working device.

The contents here change more than anywhere else: things get brought in, things go off into
projects. So the list above is about types rather than particular boards.

## About the relay modules in particular

The relays in this box are the most common reason someone connects something to 230 V for the
first time in their life. So, briefly and plainly:

- The low-voltage side of the module (control from a microcontroller) and the high-voltage side
  (the relay contacts) are separated, but **the separation ends where you started soldering
  wires**.
- Mains wires on the module go under the screw terminals, insulated, with no strands sticking out.
  A bare relay contact at 230 V on a bench is not a prototype, it is an injury.
- A module switching mains must not lie bare on the bench. An enclosure is required, even a
  temporary one.
- Check what current the contacts are rated for. The 10 A printed on a relay is for a resistive
  load, not for a motor and not for an incandescent lamp.

If you are about to switch mains and it is your first time, tell us before, not after.

## How to use

1. Take a module together with its bag if it is in one: the bag usually holds the headers and the
   hardware.
2. Look for the chip marking on the board — that finds you the schematic, the pinout and the
   library.
3. Built it, tested it, taken it apart — put the module back in the box and in the same bag.
4. If a module is blown or does not work, do not put it back among the live ones. Set it aside and
   tell us.

Passive parts, jumpers and consumables are in the [component
boxes](/en/equipment/electronics-components-and-consumables). Sensors for first experiments are in
the [37-module kit](/en/equipment/arduino-sensors-kit). Screens are in the [display
container](/en/equipment/displays-and-indicators).

## Access

The container is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed.
