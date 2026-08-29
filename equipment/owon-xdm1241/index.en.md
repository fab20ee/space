---
title: "Bench Multimeter OWON XDM1241"
seoDescription: "55,000-count bench multimeter at the Tallinn hackspace. OWON XDM1241 with true RMS, capacitance, frequency, temperature and USB logging for precise measurements on the electronics bench."
specs:
  - { label: "Resolution",  value: "55,000 counts, 4½ digits" }
  - { label: "Measures",    value: "V, A, Ω, capacitance, frequency, temperature, diode, continuity" }
  - { label: "AC",          value: "true RMS" }
  - { label: "Display",     value: "3.7\" colour LCD, dual readout" }
  - { label: "Interfaces",  value: "USB for logging and PC software" }
  - { label: "Inputs",      value: "10 A, mA/µA, COM, V/Ω/°C" }
---

<!-- TODO: verify against the actual instrument — which probes and the thermocouple are with
     it, whether PC software is installed on the bench computer. -->

A bench multimeter is a hand-held meter that grew up: mains-powered, a big display, more digits,
and it does not wander off. With 55,000 counts it resolves 0.1 mV on the 5 V range, which is what
you need to check a voltage reference, match resistors, or see the drop across a sense
resistor. The dual display shows two quantities at once — voltage and frequency, say.

It also logs over USB, so you can record how a value drifts over an hour without sitting there
writing numbers down.

## What it is good for

- Precise DC voltage and current measurements on prototypes
- Matching resistors and capacitors, sorting components from the bins
- True RMS measurement of AC signals that are not sine waves
- Temperature with the K-type thermocouple
- Continuity and diode tests when debugging a board
- Logging a slowly changing value to a PC

## Safety

- Check which sockets the leads are in **before** measuring. Voltage on the current inputs
  blows the fuse at best.
- The 10 A input is unfused for high current — do not exceed it, and never use it on mains.
- Keep fingers behind the probe guards, and do not measure mains voltage unless you know what
  you are doing and have told someone.
- Discharge capacitors before measuring capacitance or resistance.

## How to use

1. Switch on, plug the leads into COM and the socket for what you measure — V/Ω for voltage
   and resistance, mA or 10 A for current.
2. Select the function with the front buttons; auto-range is fine for most work, fix the range
   with Range if the reading hunts.
3. For current, break the circuit and put the meter in series — the meter is a short circuit on
   this setting.
4. Use Dual to show a second value, and Record or the PC software to log over time.
5. When done, put the leads back to the voltage sockets so the next person does not blow the
   current fuse, and switch off.

## Access

The meter is on the electronics bench in the hackspace room, so a plan that includes hackspace
access is required. No induction is needed.
