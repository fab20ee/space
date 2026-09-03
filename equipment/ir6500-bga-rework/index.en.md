---
title: "IR6500 Infrared BGA Rework Station"
seoDescription: "Infrared BGA rework station at the Tallinn hackspace: IR6500, 400 W top heater, 800 W bottom preheater, boards up to 400 × 305 mm, thermocouples, balls and flux on site. Access 24/7."
specs:
  - { label: "Type",             value: "infrared, top and bottom heaters" }
  - { label: "Top heater",       value: "IR 400 W, 80 × 80 mm, adjustable height" }
  - { label: "Bottom preheater", value: "IR 800 W, 180 × 180 mm" }
  - { label: "Board",            value: "up to 400 × 305 mm" }
  - { label: "Control",          value: "two independent PID controllers, K-type thermocouples" }
  - { label: "Next to it",       value: "thermocouples, balls, BGA flux" }
---

A station for chips without legs. BGA packages, that is GPUs, chipsets, memory, phone processors,
are soldered with hundreds of balls under the package, and neither an iron nor hot air can reach
them. The IR6500 heats the whole board from below with an infrared emitter and one chip from above
along a temperature profile until the balls melt: then the chip can be lifted, a new one placed, or
a chip with cracked joints simply reflowed.

The station is here just in case; nobody at the hackspace has used it yet and there is no profile
set up for a particular solder. So there is no induction either. If you know what this is and how
to use it, use it at your own risk.

## What lies next to it

K-type thermocouples, reballing balls, BGA flux. No vacuum tweezers and no stencils yet.

## How it works

1. Batteries, plastic covers and anything that melts come off the board. Nearby plastic connectors
   are covered with aluminium tape.
2. The board is clamped in the rails, the chip under the top heater, heater height per the manual.
3. A thermocouple is glued next to the chip, not onto it.
4. Flux goes around the chip and a profile is set for the solder in use: lead-free needs a higher
   peak than leaded.
5. The cycle is started and nobody walks away. When the solder has visibly melted, the chip is
   lifted or left to settle.
6. The board cools in the holder. Moving it with molten balls ruins the job.

## Take care

- Both heaters run off the mains and get hotter than any iron. The board, the rails and the chip
  stay hot for several minutes after the cycle.
- Do not look into the top emitter while it is on.
- There is a lot of flux fume; open a window.
- If the board starts to smoke, switch the station off and tell the staff.

## Access

The station is in the hackspace room, so a plan with hackspace access is required. There is no
induction, see above.
