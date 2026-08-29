---
title: "Real-time Spectrum Analyzer RIGOL RSA3030N"
seoDescription: "9 kHz – 3 GHz real-time spectrum analyzer with vector network analysis at the Tallinn hackspace. RIGOL RSA3030N for antenna tuning, RF debugging, EMI hunting and filter measurement."
specs:
  - { label: "Frequency range",  value: "9 kHz – 3 GHz" }
  - { label: "Real-time bandwidth", value: "up to 40 MHz" }
  - { label: "Modes",            value: "swept SA, real-time SA, VNA (S11, S21), tracking generator" }
  - { label: "Display",          value: "10.1\" touch screen" }
  - { label: "Interfaces",       value: "USB, LAN, HDMI" }
  - { label: "Max input",        value: "+30 dBm (1 W), ±50 V DC — never exceed" }
---

<!-- TODO: verify against the actual instrument — which options are licensed (RTSA bandwidth,
     EMI, VNA), which cables, adapters and the calibration kit are on the shelf. -->

A spectrum analyzer shows what is in the air, or on a cable, by frequency: where the energy is,
how strong, and how wide. It is the instrument for anything radio — checking that an LoRa or
Wi-Fi module transmits where and how hard it should, finding the source of interference, tuning
an antenna, or measuring a filter.

The RSA3030N adds two things a basic analyzer lacks. Real-time mode captures short bursts and
frequency-hopping signals that a swept analyzer would miss. And the built-in vector network
analyzer measures S11 and S21, so you can see an antenna's match (SWR) or a filter's response
directly, without a separate instrument.

## What it is good for

- Verifying transmit frequency, power and harmonics of a radio module
- Tuning antennas: return loss, SWR and resonance with the VNA
- Measuring filters, attenuators and cables with the tracking generator
- Hunting EMI and interference on a board or in the room
- Watching Bluetooth, Wi-Fi and other hopping signals in real time
- Checking a receiver's front end and the spectrum of a switching supply

## Safety

- **The input is the fragile part.** Never connect a transmitter output directly — even 1 W
  destroys the front end. Use an attenuator, and check the level on paper first.
- Never put DC on the input without a DC block; ±50 V is the absolute limit and the safe answer
  is zero.
- Discharge cables and antennas before connecting: touch the connector shell to the chassis
  first. Static from a long antenna is enough to kill the input.
- Do not force connectors. N and SMA are torque-fit; hand-tight is enough, cross-threading is
  permanent.
- The instrument stays on site, and its cables and adapters stay with it.

## How to use

1. Switch on and let it warm up for a few minutes if you care about level accuracy.
2. Press Preset to get to a known state, then set centre frequency and span — or start and stop
   frequencies — for the signal you are interested in.
3. Set the reference level a little above the strongest signal you expect; lower the resolution
   bandwidth to see detail, raise it to sweep faster.
4. Use markers and peak search instead of reading the grid by eye.
5. For antenna work switch to VNA mode, calibrate with the open/short/load standards at the end
   of your cable, then connect the antenna and read S11 or SWR.
6. Save screenshots to USB, remove your adapters, put the cables back, switch off.

## Access

The analyzer is in the hackspace room, so a plan that includes hackspace access is required.
**An induction is mandatory** before first use — it is short, and it is mostly about not
destroying the input.
