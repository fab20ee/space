---
title: "Arduino Sensors Kit, 37 in 1"
seoDescription: "A 37-piece sensor and module kit for Arduino at the Tallinn hackspace: temperature, light, motion, sound, hall and IR, in an organiser with labelled compartments."
specs:
  - { label: "Modules",      value: "37, each in its own compartment" }
  - { label: "What is in it", value: "temperature and humidity, light, hall, tilt, shock, sound, IR receive and transmit, buttons, an encoder, buzzers, LED modules" }
  - { label: "Interface",    value: "mostly three or four pins: power, ground, signal" }
  - { label: "Insert",       value: "a sheet with pictures and names of every module" }
---

An organiser where every compartment is a module on a small board: a sensor, a button, a buzzer,
an LED. Thirty-seven of them, with an insert sheet of pictures that tells you which is which.

This is a kit for the first step. The question "how do I even measure temperature with a
microcontroller" gets answered here in ten minutes: take a module, three wires, a library example,
and there is your number. What to do next becomes clear on real hardware rather than in theory.

## What is in it

The exact contents are on the insert, but broadly:

- **Environment**: temperature and humidity, an analogue temperature sensor, light
- **Position and motion**: tilt, shock and vibration, a hall sensor, a reed switch
- **People**: buttons, a rotary encoder, a touch sensor, a pulse sensor
- **Light and IR**: LED modules in various colours, an IR transmitter and receiver, a laser module
- **Sound**: a microphone, active and passive buzzers

Almost everything connects the same way: power, ground and one signal pin, analogue or digital.

## What not to expect from it

This is a learning kit, not instrumentation. The sensors here give you an order of magnitude and
the fact that something happened — "it got warmer", "something knocked", "the light came on". If
you need real accuracy, get a proper sensor and read its datasheet rather than this organiser.

And the modules are built for Arduino's 5 V logic. With a 3.3 V board some of them will work, some
will not, and some will put five volts on a signal pin and ruin an input. Check before you connect.

## How to use

1. Find the module on the insert and take it out of its compartment.
2. Work out what chip is on the board and find an example: most of these modules have a ready
   library.
3. Build it on a breadboard. Jumpers and breadboards are in the [component
   boxes](/en/equipment/electronics-components-and-consumables).
4. **Put the module back in the same compartment.** A kit with everything mixed up stops being a
   kit: searching it takes longer than ordering a new one.

## Access

The organiser is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed.
