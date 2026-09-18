---
title: "FNIRSI FNB58 USB Power Meter"
seoDescription: "FNIRSI FNB58 at the Tallinn hackspace: a USB tester for 4–28 V and 7 A with fast-charge protocol detection, ripple measurement and cable resistance."
specs:
  - { label: "Voltage",     value: "4 – 28 V" }
  - { label: "Current",     value: "0 – 7 A" }
  - { label: "Power",       value: "up to 120 W" }
  - { label: "Connectors",  value: "USB-A, USB-C, micro-USB — in and out" }
  - { label: "Protocols",   value: "QC2.0/3.0, PD2.0/3.0, Huawei FCP and SCP, Samsung AFC, VOOC and SuperVOOC, MTK-PE" }
  - { label: "Also",        value: "ripple, cable resistance, amp-hour and watt-hour counters" }
  - { label: "Display",     value: "2\" colour TFT" }
  - { label: "Inside",      value: "a 16-bit ADC and a dedicated PD chip" }
---

The meter goes between the charger and the device and shows what is actually happening in the
cable: voltage, current, power, and how many amp-hours and watt-hours have gone through. It answers
the everyday questions — why the phone charges slowly, whether the charger is honest about its
watts, and whether the cable is still alive.

Two things set it apart from a simple USB tester. It identifies the fast-charge protocol, which is
to say it tells you what the charger and the device actually agreed on. And it measures cable
resistance — the thing that makes "the same charger" with a different lead charge at half the
speed.

## What it is good for

- Checking the power a charger really delivers, rather than what is printed on it
- Finding a bad cable: the resistance and the voltage drop under current show up immediately
- Seeing which protocol engaged and at what voltage the charger and device settled
- Measuring how much energy went into charging a particular device
- Checking the ripple on the output of a cheap power supply
- Finding out what your PD charger can do before powering the [FNIRSI
  DPS-150](/en/equipment/portable-power-supply-fnirsi-dps-150) from it

## PD trigger mode

The tester can ask a charger for a specific voltage itself — 9, 12, 15 or 20 V. That is useful for
confirming that a charger really provides the modes it claims, and for getting a voltage you need
out of an ordinary PD charger.

The dangerous part is obvious: **in this mode there is up to 20 V on the line**. Nothing else
should be in the circuit at that moment — a phone that was expecting its five volts will not
survive it. The manufacturer's own advice is to leave the trigger off and turn it on deliberately.

## How to use

1. Put the tester between the source and the load. The input and output connectors are marked on
   the case; follow the arrows.
2. Read voltage, current and power on the main screen; the energy and time counters are on the
   neighbouring ones.
3. To check a cable, use the resistance mode: it needs two readings at different currents and the
   meter walks you through the order.
4. Protocol detection is its own menu item, with the device connected.
5. Only switch the PD trigger on when you are certain what is on the other side.

## Renting it

This one goes home with you: checking your own chargers, power banks and cables is easier where
they live. The daily rate and the term are in the rental block on this page.

## Access

The tester is in a container on the shelf in the hackspace room, so a plan that includes hackspace
access is required. No induction is needed.
