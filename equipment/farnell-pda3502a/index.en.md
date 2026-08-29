---
title: "Dual Channel Power Supply Farnell PDA3502A"
seoDescription: "Dual-output linear bench supply at the Tallinn hackspace. Farnell PDA3502A: two independent 0–35 V, 0–2 A channels with tracking mode for symmetric ±V analogue circuits."
specs:
  - { label: "Outputs",   value: "2 independent channels" }
  - { label: "Per channel", value: "0–35 V, 0–2 A" }
  - { label: "Modes",     value: "independent, or master/slave tracking" }
  - { label: "Type",      value: "linear, analogue meters" }
---

<!-- TODO: verify against the actual instrument — calibration state, whether both channels are
     within spec, condition of the terminals. -->

An old-school linear supply with two outputs and needle meters, and there is a reason it is
still on the bench: two channels. Many analogue circuits — op-amps, audio stages, instrumentation
amplifiers — need a positive and a negative rail at the same time. In tracking mode the second
channel follows the first, so one knob gives you a clean, symmetric ±12 V or ±15 V.

Being linear, it has very little switching noise, which matters when you are looking at small
signals on the oscilloscope. The meters are marked "for indication only" — use a multimeter when
the exact value matters.

## What it is good for

- Symmetric supplies for op-amp and audio circuits
- Powering two separate boards, or a board and its sensor, at different voltages
- Low-noise supply for measurements where a switching supply would show up on the scope
- Anything that needs up to 35 V — higher than the other supplies on the bench

## Safety

- Turn the current knobs down before connecting a new circuit, and raise them only as far as
  needed.
- In tracking mode the two channels are connected in series inside — check the manual's wiring
  diagram before making a ±V supply for the first time.
- Red is plus, black is minus, the green terminal is earth. Two channels means twice as many
  chances to get it wrong.
- The unit gets warm in use; keep the vents clear.

## How to use

1. Switch on with the outputs off. Choose INDEP or TRACK with the mode switch.
2. Set the voltage on each channel (or on the master in tracking mode) and the current limit.
3. Connect the leads, check polarity, and switch the output on.
4. Read the exact voltage with a multimeter if precision matters.
5. When done, switch the outputs off, disconnect the leads, and power down.

## Access

The supply is on the electronics bench in the hackspace room, so a plan that includes hackspace
access is required. No induction is needed.
