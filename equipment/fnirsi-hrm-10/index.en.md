---
title: "FNIRSI HRM-10 Battery Internal Resistance Tester"
seoDescription: "FNIRSI HRM-10 at the Tallinn hackspace: a battery internal resistance tester using four-wire Kelvin clips, reading resistance and voltage at the same time. A milliohmmeter in your pocket."
specs:
  - { label: "Measures",       value: "internal resistance and voltage at the same time" }
  - { label: "Resistance",     value: "up to 200 Ω; in the milliohm range it resolves hundredths of a milliohm" }
  - { label: "Voltage",        value: "up to 100 V DC" }
  - { label: "Method",         value: "four-wire (Kelvin), lead and contact resistance excluded" }
  - { label: "Memory",         value: "measurement history, eight voltage/resistance pairs on screen, export as a table" }
  - { label: "Display",        value: "colour TFT" }
  - { label: "Supplied with",  value: "four-contact Kelvin clips" }
---

The capacity of a battery tells you how much is stored in it. The internal resistance tells you how
fast it can give that back — and whether the cell is alive at all. An 18650 can read an honest
4.1 V and still sag to cut-off under load, because its internal resistance is 300 mΩ where it used
to be 30.

The HRM-10 measures both at once: clip it on, and you see the voltage and the resistance. Measuring
milliohms with an ordinary multimeter is pointless — the resistance of its own leads is larger than
the thing you are trying to measure.

## Why four wires

The clips are not ordinary ones but Kelvin clips: each jaw has two separate contact pads. One pair
of wires carries the current, the other measures the voltage right at the battery terminal. The
resistance of the leads, of the clips and of the oxide on the terminal never enters the result.
That is why this instrument sees tenths of a milliohm and a multimeter does not.

## What it is good for

- Sorting used 18650 and 21700 cells: a dead one has several times the internal resistance of a
  live one, even when both show a normal voltage
- Matching cells for a pack: cells put in parallel or in series should have similar resistance,
  or one of them does the work for everybody and gets hot
- Checking spot welds on nickel strip in a pack — a bad weld shows up as extra milliohms
- Checking contacts, connectors, fuses and traces: it is also simply a milliohmmeter
- Diagnosing a lead-acid battery without taking it out of the car

## How to use

1. Switch on and make sure what you are measuring is DC. **Never apply AC voltage**, and the DC
   limit is 100 V.
2. Clip on so that both pads of each jaw touch metal. If one pad hangs in the air, the four-wire
   method quietly becomes a two-wire one and the reading drifts off.
3. Let the reading settle and read both values.
4. When sorting cells, measure them under the same conditions: same state of charge, same
   temperature, same spot on the terminal. Only then is the comparison worth anything.
5. Save the results you need to memory and export them as a table afterwards.

## What not to do

- Do not connect it to mains or to any AC voltage.
- Do not measure the resistance of a circuit with something running in it: the instrument injects
  its own current.
- Do not bridge both terminals of a battery with the clips while in voltage mode — that is not a
  measurement, that is a short circuit through a clip.

## Renting it

This one goes home with you: the usual reason is going through a box of used 18650 cells and
working out which of them are still worth anything. The daily rate and the term are in the rental
block on this page.

## Access

The instrument is in a container on the shelf in the hackspace room, so a plan that includes
hackspace access is required. No induction is needed.
