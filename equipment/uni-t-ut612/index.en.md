---
title: "UNI-T UT612 Handheld LCR Meter"
seoDescription: "UNI-T UT612 LCR meter at the Tallinn hackspace: inductance, capacitance and resistance at five frequencies up to 100 kHz, with ESR, Q factor and loss angle."
specs:
  - { label: "Measures",       value: "L, C, R, DCR, plus Q, D, θ and ESR" }
  - { label: "Test frequencies", value: "100 Hz, 120 Hz, 1 kHz, 10 kHz, 100 kHz" }
  - { label: "Inductance",     value: "20 µH – 2000 H, ±(0.5 % + 5)" }
  - { label: "Capacitance",    value: "200 pF – 20 mF, ±(0.5 % + 5)" }
  - { label: "Resistance",     value: "20 Ω – 200 MΩ, ±(0.3 % + 5)" }
  - { label: "Display",        value: "20,000 counts, secondary readout 2,000 counts" }
  - { label: "Test signal",    value: "0.6 V rms, 120 Ω output impedance" }
  - { label: "Modes",          value: "series and parallel equivalent circuit, auto LCR, relative mode, tolerance sorting, calibration" }
  - { label: "Interface",      value: "USB" }
  - { label: "Power",          value: "9 V battery or USB" }
---

A multimeter measures a capacitor at one frequency and gives you one number. An LCR meter asks at
which frequency you intend to use that capacitor, and answers with a different one. The difference
is not academic: an electrolytic that shows its honest 100 µF at 100 Hz can behave like a piece of
resistive wire at 100 kHz.

The UT612 measures inductance, capacitance and resistance at five frequencies from 100 Hz to
100 kHz, and shows not only the value itself but what sits next to it: ESR, quality factor,
dissipation factor, phase angle.

Inductance deserves a separate word: very few instruments measure it at all. Nothing else in the
hackspace shows inductance — not the bench multimeter, not the handheld ones. If you need an
inductance, there is exactly one option, and this is it.

## What that is for in practice

- **ESR of a capacitor** is the diagnosis for electrolytics. The capacitance can still be in
  spec while the ESR has gone up tenfold, and then a power supply starts whistling and getting
  hot. An ordinary multimeter does not see this.
- **The inductance of a coil** you wound yourself: the turns are what you counted, and the
  inductance is something else, because the core is not what you thought.
- **Matching pairs**: two capacitors or two coils with the same printed value and different real
  ones.
- **Sorting** the small stuff out of the component bins: tolerance mode shows the deviation as a
  percentage rather than an absolute value.
- **The Q of a coil** at its working frequency — if you are building a filter or a tuned circuit,
  that is the parameter that decides.

## Series or parallel

The meter models the part as two elements, and you can choose how. The rule is simple: small
capacitances and large resistances are measured in the parallel circuit, large capacitances and
small resistances in the series one. When in doubt, leave it in auto LCR: the meter works out what
it is looking at and chooses sensibly.

## How to use

1. **Discharge the capacitor before measuring.** The meter applies its own test signal and does not
   expect the part to have energy stored in it. This is printed on the case for a reason.
2. Plug the leads into the "+" and "−" sockets.
3. Choose a frequency with FREQ, guided by the working frequency of the circuit: 100 or 120 Hz for
   mains filtering, 1 kHz for a general check, 10 and 100 kHz for switching circuits.
4. Calibrate: press CAL with the leads open, then with them shorted. This subtracts the
   capacitance and resistance of the leads, which is plainly visible on small values.
5. Use FUNC to choose what appears as the secondary reading: D, Q, θ or ESR.
6. To match pairs, press REL after the first part; the meter then shows the deviation from it.
7. When done, switch it off and put it back with its leads into the container on the shelf.

## What it does not do

This is not an in-circuit component tester. The part has to come out, or at least have one leg
lifted, or you measure everything connected in parallel with it on the board. And no voltage goes
onto the input sockets — the meter measures with its own signal.

## Renting it

This one goes home with you: the usual reason is repairing a power supply or an amplifier, where
the electrolytics need checking by ESR without carrying the whole thing to the hackspace. The daily
rate and the term are in the rental block on this page.

## Access

The meter is in a container on the shelf in the hackspace room, so a plan that includes hackspace
access is required. No induction is needed.
