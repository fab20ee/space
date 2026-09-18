---
title: "150 W Electronic Load"
seoDescription: "A 150 W electronic load at the Tallinn hackspace: test a power supply under load, measure the real capacity of a battery, with cut-off by current, voltage and time."
specs:
  - { label: "Power",        value: "up to 150 W" }
  - { label: "Mode",         value: "constant current (CC)" }
  - { label: "Metering",     value: "amp-hours and watt-hours delivered, time under load" }
  - { label: "Cut-off",      value: "by current, by voltage and by time" }
  - { label: "Connection",   value: "screw terminal, supports four-wire sensing" }
  - { label: "Power input",  value: "external supply only; it lives with the load" }
  - { label: "Cooling",      value: "heatsink with a fan" }
  - { label: "Model",        value: "none — the board carries no markings" }
---

An electronic load is a resistor you can command. You tell it "draw three amps", it draws exactly
three amps, and it turns all the power it receives into heat on the heatsink.

It is there for testing sources. With nothing connected, any power supply shows a beautiful
12.00 V. The interesting questions are what it shows at three amps, whether it trips at five, and
what state it is in after an hour. Batteries and power banks are the same story: the milliamp-hours
on the label and the real ones are often different numbers, and the load counts them.

The instrument has no name. There is no model and no serial number on the board, only a production
code, so there is no point looking for a manual — everything it does is described here.

## It needs its own power supply

Many cheap loads run off the very source they are measuring. **This one does not.** It needs its
own supply, which lives in the container with it. Without that the load will not switch on, and
that is not a fault, that is how it is built.

## Four-wire sensing

The load can measure voltage through a separate pair of wires, right at the source's terminals
rather than at its own input. The difference shows at high currents: at five amps the drop across
ordinary wires is a few tenths of a volt. Without four wires the voltage cut-off fires somewhere
other than where you intended, and the battery capacity comes out wrong.

## What it is good for

- Checking whether a power supply holds its rated current, and how far the voltage sags while it
  does
- Measuring the real capacity of a cell, a pack or a power bank in amp-hours and watt-hours
- Running a source under load for a set time and seeing what became of it
- Finding the current at which the source's protection trips
- Discharging a cell to a chosen voltage before storage or before a measurement

## How to use

1. Take the load and its power supply from the container on the shelf.
2. Connect the supply to the load.
3. Connect the source under test to the screw terminal, watching the polarity. If you are
   measuring capacity, or the cut-off voltage matters, use a separate pair of wires for sensing.
4. Set the current and the cut-offs: by voltage, by current and by time. For a lithium cell the
   voltage cut-off is not optional — discharging below its minimum kills the cell.
5. Switch the load on and watch for the first half minute that the current is the one you asked
   for.
6. Zero the amp-hour and watt-hour counters before a new measurement, or you will be adding to
   somebody else's figures.
7. When done, switch the load off, let the heatsink cool and put everything back in the container.

## Safety

- The load turns power into heat. The heatsink and the air from the fan are hot, and that is
  normal.
- Do not block the fan, and do not stand the load on paper, on a cloth or in a tight box.
- 150 W is a power limit, not a current limit. Five amps at thirty volts is already the limit.
- Polarity. Connecting it backwards is not "it will not work", it is smoke.

## Access

The load is in a container on the shelf in the hackspace room, so a plan that includes hackspace
access is required. No induction is needed.
