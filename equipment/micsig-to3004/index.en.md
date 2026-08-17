---
title: "Oscilloscope Micsig TO3004"
seoDescription: "300 MHz four-channel tablet oscilloscope in the Tallinn hackspace. Debug embedded hardware, buses and power supplies with proper equipment."
specs:
  - { label: "Bandwidth",   value: "300 MHz" }
  - { label: "Channels",    value: "4" }
  - { label: "Format",      value: "tablet, touch screen, battery powered" }
  - { label: "Interfaces",  value: "USB, LAN" }
---

<!-- TODO: verify against the actual instrument — sample rate, memory depth, which probes and
     accessories are present, whether the serial bus decoding option is licensed. -->

An oscilloscope shows you what a signal actually does over time, instead of what the datasheet
says it should do. With 300 MHz of bandwidth and four channels it covers most of what embedded
work throws at you: clocks, resets, PWM, switching power supplies, and serial buses seen next to
each other on the same timebase.

The tablet form factor matters in practice — it runs on battery and can be carried to whatever
bench or machine you are debugging.

## What it is good for

- Finding out why a microcontroller resets or a bus stops responding
- Measuring rise times, jitter, ripple and noise
- Comparing four signals at once — for example clock, chip select and both data lines
- Checking switching supplies under load
- Capturing rare glitches with triggering rather than by staring at the screen

## Safety

- Ground the probe correctly before touching a circuit; a floating ground turns measurements into
  fiction and can damage the instrument.
- Never connect the probe ground to a live mains conductor. Mains-referenced work needs an
  isolation transformer or a differential probe — ask before starting.
- Respect the probe's voltage rating, including the attenuation setting (×1 and ×10 differ).
- Do not open the case. If something is wrong with the instrument, report it.

## How to use

1. Switch on, check the battery, and set the probe attenuation to match the setting on screen.
2. Compensate the probe on the calibration output before precise measurements.
3. Connect the ground clip as close to the measurement point as possible.
4. Set the timebase and vertical scale roughly, then use auto-set only as a starting point.
5. Use triggering deliberately — edge for periodic signals, pulse width or serial for glitches.
6. When done, save your screenshots to a USB drive, wipe the probes, and put everything back.

## Access

The instrument is in the hackspace room, so a plan that includes hackspace access is required.
It stays on site — do not take it home.
