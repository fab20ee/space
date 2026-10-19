---
title: "Rohde & Schwarz SMIQ 03B Signal Generator"
seoDescription: "A Rohde & Schwarz SMIQ 03B vector signal generator at the Tallinn hackspace: 300 kHz – 3.3 GHz, −140 to +13 dBm, analogue and digital modulation."
specs:
  - { label: "Range",        value: "300 kHz – 3.3 GHz" }
  - { label: "Level",        value: "−140 to +13 dBm, 0.1 dB steps" }
  - { label: "Frequency step", value: "0.1 Hz" }
  - { label: "Modulation",   value: "analogue (AM, FM, ΦM, pulse) and vector I/Q" }
  - { label: "Output",       value: "50 Ω" }
---

An instrument that puts out a radio signal whose frequency, level and modulation you know exactly.
You need it whenever you test the receiving side: a spectrum analyser shows what is on the air, a
generator lets you put exactly what you meant onto it.

The important end here is the bottom of the level range. Minus a hundred and forty dBm is a signal
at the limit of a receiver's sensitivity, and it is at levels like that you find out whether your
device hears anything at all.

## What it is good for

- Measuring a receiver's sensitivity: feed it a signal and lower the level until reception falls
  apart
- Testing a filter or an amplifier by feeding a known signal into it
- Debugging a radio module against a reference at a known frequency
- Checking whether your device goes deaf next to a strong signal on a neighbouring frequency
- Feeding a modulated signal in and seeing what the chain does to it

## Things to remember

- **The output is delicate.** Nothing goes into it from outside: no transmitter, no DC, and no
  antenna that will pick up somebody else's signal. There is protection, but it is not worth
  testing.
- **Set the level before connecting**, not after. The instrument remembers the previous setting,
  and that is usually +13 dBm, which somebody's receiver may not survive.
- Connectors and adapters are in the [RF container](/en/equipment/rf-accessories), along with the
  calibration kits and the DC block.

## How to use

1. Switch on and let it warm up — for level accuracy that matters.
2. Set frequency and level. Start low and come up, not the other way round.
3. Turn on modulation if you need it, and the output with its own button.
4. Check what came out with the [RIGOL spectrum
   analyser](/en/equipment/spectrum-analyzer-rigol-rsa3030n) or the
   [tinySA](/en/equipment/portable-spectrum-analyzer-tinysa-ultra).
5. When done, switch the output off, then the instrument.

## Access

The generator is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed.
