---
title: "Infrared BGA Rework Station IR6500"
seoDescription: "Infrared BGA rework station at the Tallinn hackspace. IR6500 with top and bottom heaters for reballing, replacing GPUs, chipsets and other BGA chips on laptop and phone boards."
specs:
  - { label: "Type",            value: "infrared rework, top and bottom heaters" }
  - { label: "Top heater",      value: "IR, dark emitter, adjustable height" }
  - { label: "Bottom preheater", value: "IR, full board preheating" }
  - { label: "Control",         value: "two PID controllers with K-type thermocouples" }
  - { label: "Board holder",    value: "adjustable rails, PCB up to approx. 350 × 400 mm" }
---

<!-- TODO: verify against the actual station — heater powers, maximum board size, which
     thermocouples and stencils are on the bench, whether the profile has been tuned. -->

An infrared rework station is how you replace a chip that has no legs. BGA packages — GPUs,
chipsets, memory, most phone processors — are soldered by hundreds of balls underneath, so a
soldering iron cannot reach them. The IR6500 heats the whole board gently from below and the one
chip strongly from above, following a temperature profile, until the balls melt and the chip
can be lifted off or settles into place.

This is the most demanding tool on the electronics bench. A wrong profile cooks the board or
leaves half the balls unsoldered, so an induction is required before the first job.

## What it is good for

- Removing and refitting BGA chips: GPUs, chipsets, memory, phone SoCs
- Reballing a chip with a stencil and new solder balls
- Reflowing a suspect chip whose joints have cracked
- Preheating a board for hot air work, so the copper does not pull all the heat away

## Safety

- Both heaters are mains-powered and get far hotter than a soldering iron. The board, the
  holder rails and the chip stay dangerously hot for minutes after the cycle ends.
- Do not look into the top IR emitter while it is on.
- Never leave a running cycle. Stay at the station and watch the thermocouple readings.
- Let the board cool on the holder — moving a board with molten balls ruins the job.
- Flux fumes are heavy during reflow; use the fume extractor.

## How to use

1. Remove batteries, plastic covers, stickers and anything that melts from the board. Shield
   nearby plastic connectors with aluminium tape or metal covers.
2. Clamp the board in the rails, level, with the target chip under the top heater. Set the
   heater height per the manual.
3. Tape a thermocouple next to the chip (not on it) and check it reads room temperature.
4. Apply flux around the chip and select or enter the temperature profile for the solder used —
   lead-free needs a higher peak than leaded.
5. Run the cycle and watch the readings. When the peak is reached and the solder has visibly
   melted, lift the chip with the vacuum pen, or leave it to settle if you are reflowing.
6. Let everything cool down completely before touching the board. Clean off the flux.

## Access

The station is in the hackspace room, so a plan that includes hackspace access is required.
**An induction is mandatory** before your first job — it covers heater setup, thermocouple
placement, profiles and what to do if the board starts to smoke.
