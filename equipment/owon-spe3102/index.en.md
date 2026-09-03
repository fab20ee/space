---
title: "OWON SPE3102 Programmable Power Supply"
seoDescription: "Bench power supply at the Tallinn hackspace: OWON SPE3102, 0–30 V, 0–10 A, 200 W, current limit, OVP and OCP protection, a consumption graph on the screen. Access 24/7."
specs:
  - { label: "Output",      value: "0–30 V, 0–10 A, 200 W" }
  - { label: "Resolution",  value: "1 mV / 1 mA" }
  - { label: "Protection",  value: "OVP, OCP, over-temperature" }
  - { label: "Display",     value: "2.8\" colour, voltage, current and a graph" }
  - { label: "Also",        value: "USB 5 V / 1 A for charging; PC control not set up" }
  - { label: "Leads",       value: "plugged into the supply, spares on the shelf" }
---

The main power supply on the electronics bench. Voltage and current limit are set to a millivolt
and a milliamp, and when a fresh circuit has a short, the supply sits at the limit instead of
letting out smoke. 10 A is enough for motors, LED strips and heaters, not just microcontroller
boards. The graph on the screen shows how much a device draws over time.

## How to use

1. Switch the supply on with the output off. Set the voltage with the V button and the knob, the
   current limit with the I button. Set the limit as low as the circuit allows: that is what saves
   boards.
2. Optionally set OVP and OCP a little above the working values as a second safety net.
3. Connect the leads, check polarity: red is plus, black is minus, the green terminal is earth, not
   minus. Press On/Off to enable the output.
4. The CC indicator means the circuit draws more than you allowed and the supply is holding the
   current.
5. When done, switch the output off first, then remove the leads, then switch the supply off.

## Take care

- 10 A through thin leads or a breadboard heats them to a fire. For high currents take proper
  leads from the shelf.
- Do not connect the output to a live circuit or in parallel with another source.
- Do not charge lithium cells from it; that needs a charging circuit.

## Access

The supply is on the electronics bench in the hackspace room, so a plan with hackspace access is
required. No induction is needed. The supply stays in the room.
