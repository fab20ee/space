---
title: "FNIRSI DPS-150 Portable Power Supply"
seoDescription: "FNIRSI DPS-150 at the Tallinn hackspace: a pocket bench power supply up to 30 V and 5 A, running off a USB-C PD charger. Available to rent and to work with anywhere."
specs:
  - { label: "Output",        value: "0 – 30 V, 0 – 5 A, up to 150 W" }
  - { label: "Setting step",  value: "10 mV for voltage, 1 mA for current" }
  - { label: "Ripple",        value: "under 20 mV" }
  - { label: "Input",         value: "USB-C with PD or QC, or a DC barrel jack, 5 – 30 V" }
  - { label: "Modes",         value: "CV and CC, six memory slots M1 – M6" }
  - { label: "Protection",    value: "over-voltage, over-current, over-power, over-temperature, short circuit, reverse polarity" }
  - { label: "Display",       value: "2.8\" IPS, flips through 90°" }
  - { label: "Metering",      value: "amp-hours, watt-hours, time under load" }
  - { label: "Size",          value: "106 × 76 × 28 mm, 178 g" }
  - { label: "Supplied with", value: "crocodile clip leads" }
---

A bench power supply the size of a deck of cards. It gives anything from zero to 30 V and up to
5 A, limits current, counts the amp-hours and watt-hours it has delivered — everything a big bench
supply does, except that it fits in a pocket and runs off an ordinary laptop charger.

For serious work the hackspace has the [OWON SPE3102](/en/equipment/power-supply-owon-spe3102):
two channels, mains powered, honest specifications. The DPS-150 is for the other case — when the
power has to come to where you are working, or go home with you.

## Powering it, and the one real limit

It runs from USB-C with PD — any laptop charger in the hackspace will do — or from an ordinary
supply with a barrel jack, 5 to 30 V. The two inputs must not be plugged in at the same time,
which is printed on the case.

Then the important part: **the DPS-150 is a step-down converter**. The output voltage is always
lower than the input. From a PD charger it takes at most 20 V, so what you get out is a little
under twenty. If you want something close to thirty, you need a separate 24–30 V supply on the
barrel jack. Do not feed it more than 30 V in — that kills it.

Power works the same way: 150 W only happens from a source that can deliver it. A 65 W charger
gives you about 65 W, which is fine — just know why.

## What it is good for

- Powering a prototype or a board with a current limit, so a wiring mistake does not become a
  firework
- Setting a voltage to 10 mV and watching how a device behaves at the edge of its range
- Charging or discharging something under control and seeing how many amp-hours went in
- Taking power to equipment that cannot be brought to the bench
- Working at home, if that is where your bench is

## How to use

1. Take the instrument and the crocodile leads from the container on the shelf, and any free PD
   charger in the hackspace.
2. Plug the input in. The screen shows the input voltage, so you can see straight away what the
   charger gave you and what to expect from it.
3. **Before connecting the load**, set Vset and Iset. The current limit is not a formality; it is
   the one thing that saves your board when something is wrong.
4. Connect the crocodile leads the right way round and switch the output on.
5. The CV or CC indicator tells you which limit the supply has hit: your voltage or your current.
   Dropping into CC unexpectedly means the load is drawing more than you allowed, which is a
   reason to switch the output off and find out why.
6. Settings you use often go into the M1 – M6 slots.
7. When done, switch the output off, disconnect the load and put the supply and its leads back
   into the container.

## Renting it

This one goes home with you. **The charger is not part of the rental** — bring your own laptop or
phone charger, as long as it does PD. The daily rate and the term are in the rental block on this
page.

## Access

The container is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed.
