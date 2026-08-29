---
title: "Programmable Power Supply OWON SPE3102"
seoDescription: "Programmable bench power supply at the Tallinn hackspace. OWON SPE3102: 0–30 V, 0–10 A, 200 W, with overvoltage and overcurrent protection and a USB charging port."
specs:
  - { label: "Output",       value: "0–30 V, 0–10 A, 200 W" }
  - { label: "Resolution",   value: "1 mV / 1 mA" }
  - { label: "Protection",   value: "OVP, OCP, overtemperature" }
  - { label: "Display",      value: "2.8\" colour LCD with V/A trend graph" }
  - { label: "Extras",       value: "5 V / 1 A USB charging port, USB for PC control" }
---

<!-- TODO: verify against the actual instrument — firmware, whether PC control is set up, which
     leads are with it. -->

The main bench supply. A programmable supply gives you a clean, adjustable DC voltage with a
current limit you set yourself — so when a fresh circuit has a short, the supply just clamps to
the limit instead of letting the smoke out. With 10 A available it also powers motors, LED strips
and heaters, not only small logic boards.

The display shows voltage and current live and draws a trend graph, which is handy for
watching how much a device actually draws over time.

## What it is good for

- Powering a prototype at exactly the voltage it needs, with a safe current limit
- Finding a short: set the limit low, watch the voltage collapse, feel for the warm part
- Measuring the consumption of a device — idle, active, sleep
- Charging or testing batteries under supervision, with OVP set as a guard
- Running motors, pumps, LED strips and other loads up to 200 W

## Safety

- Set the current limit **before** connecting your circuit, and set it as low as the circuit
  allows. This is what saves boards.
- Check polarity twice. Red is plus, black is minus; the green terminal is earth, not minus.
- 10 A through thin wires or a breadboard is a fire hazard — use proper leads for high currents.
- Never connect the supply output to a live circuit or to another supply.
- Do not use it for lithium cells without a proper charger circuit or someone who knows what
  they are doing.

## How to use

1. Switch on with the output **off**. Set the voltage with the knob and the V button, then set
   the current limit with the I button.
2. Optionally set OVP and OCP a little above your working values as a second guard.
3. Connect the leads to your circuit, check polarity, then press On/Off to enable the output.
4. Watch the display: if the CC indicator lights up, the supply is in current limit — your
   circuit draws more than you allowed.
5. When done, switch the output off first, then disconnect the leads, then power down.

## Access

The supply is on the electronics bench in the hackspace room, so a plan that includes hackspace
access is required. No induction is needed.
