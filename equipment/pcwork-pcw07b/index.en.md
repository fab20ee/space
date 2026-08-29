---
title: "Compact DC Power Supply PCWork PCW07B"
seoDescription: "Compact adjustable DC bench supply at the Tallinn hackspace. PCWork PCW07B: 0–30 V, 0–5 A, coarse and fine control, LED readout — a simple second supply for everyday work."
specs:
  - { label: "Output",     value: "0–30 V, 0–5 A" }
  - { label: "Modes",      value: "constant voltage / constant current" }
  - { label: "Control",    value: "push knobs, coarse and fine" }
  - { label: "Display",    value: "LED, voltage and current" }
---

<!-- TODO: verify the current rating and the resolution against the nameplate; note which leads
     belong to it. -->

A small, no-frills adjustable supply. Two knobs, one output, a readout — everything you need to
power a microcontroller board, an op-amp circuit or a sensor while the big OWON supply is busy
with something else. It sits in constant voltage mode until the load pulls more than the set
current, then it switches to constant current and holds the limit.

## What it is good for

- Powering a second circuit on the bench
- Simple experiments where 5 A is plenty
- Feeding a fixed voltage to a board while you probe it with the oscilloscope
- Lending a "known good" supply to a board you suspect of a power problem

## Safety

- Turn the current knob down before connecting a new circuit, then raise it only as far as the
  circuit needs.
- Red is plus, black is minus; the green terminal is earth.
- Do not connect the output to a live circuit or in parallel with another supply.
- Do not use it as a battery charger for lithium cells.

## How to use

1. Switch on with nothing connected. Set the voltage with the coarse and fine knobs.
2. Set the current limit: short the output briefly with a lead, turn the current knob to the
   limit you want, remove the short. Or, more simply, start low and raise it once the circuit
   is connected.
3. Connect the leads, check polarity, press Output.
4. If the C.C. indicator lights, the circuit is drawing more than the limit.
5. When done, press Output to switch it off, disconnect the leads, and power down.

## Access

The supply is on the electronics bench in the hackspace room, so a plan that includes hackspace
access is required. No induction is needed.
