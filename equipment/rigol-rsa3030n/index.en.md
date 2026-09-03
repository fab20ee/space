---
title: "RIGOL RSA3030N Spectrum Analyser"
seoDescription: "Real-time spectrum analyser 9 kHz – 3 GHz with VNA, tracking generator and the EMI option at the Tallinn hackspace. RIGOL RSA3030N, TekBox TEM cell, calibration kit. Access 24/7."
specs:
  - { label: "Frequency range",     value: "9 kHz – 3 GHz" }
  - { label: "Real time",           value: "10 MHz bandwidth" }
  - { label: "Modes",               value: "swept, real-time, EMI, VNA (S11, S21, DTF)" }
  - { label: "Tracking generator",  value: "yes" }
  - { label: "Display",             value: "10.1\" touch" }
  - { label: "Interfaces",          value: "USB, LAN, HDMI" }
  - { label: "Max input",           value: "+30 dBm (1 W), ±50 V DC" }
  - { label: "Next to it",          value: "TekBox TBTC1 TEM cell, NanoVNA demo board, RF adapters, calibration kit" }
---

A spectrum analyser shows what is on the air or on a cable: at which frequencies there is
energy, how strong and how wide. It is the tool for everything radio: check that a LoRa or Wi-Fi
module transmits where it should, find a source of interference, tune an antenna or measure a
filter.

The RSA3030N has three things beyond a plain analyser. Real-time mode catches short bursts and
frequency-hopping signals that a swept analyser misses. The built-in vector network analyser
measures S11 and S21, so antenna matching and a filter's response are visible without a separate
instrument. The EMI option is installed: CISPR bandwidths and a quasi-peak detector to judge the
emissions of your own board before certification.

The antennas of the KIISU project were tuned on it; the analyser is in that project's equipment
list below.

## What lies next to it

- **TekBox TBTC1 open TEM cell**: for pre-compliance EMC checks of a small board, up to 3 GHz,
  190 × 130 × 50 mm of space for the board, termination and DC block included. The board goes
  inside, the analyser shows what it radiates.
- **NanoVNA RF Demo Kit**: 18 test circuits, filters and attenuators, to learn VNA measurements on
  known objects.
- A set of RF adapters of various types and a VNA calibration kit.

All of it stays with the instrument.

## The input

The only thing that can be broken in a second is the input stage.

- Do not connect a transmitter output directly. The input limit is +30 dBm, that is 1 W; work out
  the level and put an attenuator in.
- Do not put DC on the input without a DC block. The limit is ±50 V; the safe value is zero.
- Before connecting a long cable or an antenna, touch the connector body to the instrument's
  chassis to discharge static.
- N and SMA connectors are tightened by hand, without tools and without cross-threading.

## How to use

1. Switch on; for level accuracy let it warm up for a few minutes.
2. Press Preset, then set the centre frequency and span, or the start and stop frequencies.
3. Set the reference level a little above the strongest signal you expect. Narrow the resolution
   bandwidth to see detail, widen it to sweep faster.
4. Markers and peak search are more accurate than reading the grid by eye.
5. For an antenna switch to VNA mode, calibrate with the open, short and load standards from the
   calibration kit at the end of your cable, then connect the antenna and read S11 or SWR.
6. Screenshots go to USB. When done, remove your adapters, put the cables and kits back, switch
   the instrument off.

## Access

The analyser is in the hackspace room, so a plan with hackspace access is required. No induction
is needed, but read the section about the input before you connect anything.
