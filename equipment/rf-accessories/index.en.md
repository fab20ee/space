---
title: "RF Accessories: Adapters, Calibration Kits, Antennas"
seoDescription: "The RF accessories box at the Tallinn hackspace: N, SMA and BNC adapters, open/short/load calibration kits, a DC block to 6 GHz, and 433 and 868 MHz antennas."
specs:
  - { label: "Calibration kits", value: "open / short / load, one N-type set and one SMA" }
  - { label: "DC block",     value: "up to 6 GHz" }
  - { label: "Adapters",     value: "N-type, SMA, BNC, binding posts, in assorted combinations" }
  - { label: "Antennas",     value: "SMA whips for 433 and 868 MHz, and a telescopic SMA" }
  - { label: "Demo board",   value: "NanoVNA RF Demo Kit — filters and test circuits with known values" }
  - { label: "Cables",       value: "SMA and N, various lengths" }
---

A separate container with everything that goes between an instrument and an antenna. It measures
nothing by itself, and no radio instrument in the workshop works without it: the
[tinySA Ultra](/en/equipment/portable-spectrum-analyzer-tinysa-ultra) has an SMA connector, the
[RIGOL RSA3030N](/en/equipment/spectrum-analyzer-rigol-rsa3030n) has N, your cable most likely has
a third, and the only thing that joins them is an adapter.

So all of the RF bits live in one place instead of being scattered among the instruments.

## Calibration kits

Two open / short / load sets: one with N-type connectors, one SMA.

This is what a vector network analyser cannot measure anything meaningful without. The instrument
is calibrated **at the end of your cable**, with the adapters you intend to use: you connect the
open, the short and the 50 Ω load in turn, the instrument learns what the path itself contributes,
and subtracts it from then on. Without calibrating you measure a cable with adapters, not an
antenna.

The standards are precision parts. Do not drop them and do not torque them down.

## The DC block

It passes RF and blocks DC. It goes on the instrument's input whenever the cable might be carrying
DC: an active antenna phantom-powered through the centre conductor, a circuit output sitting on a
bias, a mast amplifier.

The tinySA's DC limit is ±5 V and the RIGOL's is ±50 V. The DC block is rated to 6 GHz, which
covers the range of both.

## The NanoVNA RF Demo Kit

A board with a dozen and a half test circuits: high-pass and low-pass filters, a 10.7 MHz band-pass,
matched and mismatched loads, 50 and 75 Ω. Every value is known in advance and printed on the
board itself.

It is for learning to measure on something whose answer you already know: if the demo board does
not show what is written on it, the problem is in your calibration or your cable, not in the
circuit under test.

## Antennas

SMA whips for 433 and 868 MHz — the working frequencies of LoRa, sensors and the rest of everyday
radio telemetry. The telescopic SMA is broadband, for hunting interference and for "is there a
signal at all".

An antenna cut for one frequency always beats the telescopic one at that frequency, and is always
worse at every other.

## Handling the connectors

The connectors are the expensive part of this container, and everybody breaks them the same way.

- Turn **the nut, not the cable or the instrument**. Rotating the centre pin destroys the
  connector.
- By hand. N and SMA go finger-tight; we do not have a torque wrench everywhere, and
  over-tightening reliably ruins the thread.
- Do not cross-thread: the nut should start freely on the first turn.
- SMA and RP-SMA look identical but their centre contacts are mirrored. If it "will not go in",
  that is why — do not force it.
- Do not mix 50 and 75 Ω. The impedance is marked on the board and on some of the adapters.
- Put the caps back on the standards and on the instruments' connectors.

## What is not in the box

**Attenuators.** The tinySA, HackRF One and RIGOL cards all say that a transmitter output only
reaches an instrument through an attenuator — which is true, but there is no attenuator in the
container at the moment. If you need to feed an analyser anything stronger than a milliwatt, write
to us rather than improvising.

## Access

The container is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed. The kit is not rented out — it belongs to the instruments that stay here.
