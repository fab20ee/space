---
title: "Nordic Power Profiler Kit II"
seoDescription: "The Nordic PPK2 at the Tallinn hackspace: measures current from hundreds of nanoamps to one amp at 100,000 samples per second. For battery-powered devices."
specs:
  - { label: "Current range", value: "200 nA to 1 A, resolution from 100 nA" }
  - { label: "Sample rate",  value: "100,000 samples per second" }
  - { label: "Modes",        value: "ampere meter (external supply) and source meter" }
  - { label: "Voltage",      value: "0.8 – 5 V in source mode, up to 1 A" }
  - { label: "Logic inputs", value: "8 digital inputs — a simple logic analyser" }
  - { label: "Connection",   value: "USB to a computer" }
  - { label: "Software",     value: "nRF Connect for Desktop, the Power Profiler app" }
---

An instrument for one question: how much does your device actually draw, and when?

For anything running on a battery that is the question. A sensor that wakes once a minute lasts
years on a cell — if it draws microamps while asleep. If it draws half a milliamp while asleep,
because a pull-up or an LED was left enabled somewhere, the cell lasts a month. You only see the
difference with an instrument that can measure microamps and hundreds of milliamps in the same
recording.

The PPK2 can: 200 nA to 1 A, a hundred thousand samples per second. A two-millisecond transmit
burst shows up as a burst, not as an average.

## Two modes

- **Ampere meter.** The device runs off its own supply; the PPK2 goes in series with the power and
  only measures.
- **Source meter.** The PPK2 supplies 0.8–5 V itself and measures what is taken. Handier when you
  want behaviour at different supply voltages: what the board eats at 3.6 V and what at 2.2 V,
  when the cell is nearly flat.

Plus eight digital inputs. You clip them to pins on your own board, and then one graph shows what
was happening at the moment of a current spike: here the firmware raised a pin, here the radio
came on, here is the 40 mA peak.

## What it is good for

- Measuring sleep current and working out whether the device will last its claimed lifetime
- Catching whatever is keeping the device from sleeping
- Totting up the real consumption of one work cycle and turning it into months from a given cell
- Comparing two firmware builds by consumption rather than by feel
- Seeing the inrush current at power-on

## How to use

1. Install **nRF Connect for Desktop** on a computer and the **Power Profiler** app inside it.
2. Connect the PPK2 over USB.
3. Pick a mode: ampere meter if the board has its own supply, source meter if the PPK2 is to power
   it.
4. Wire up to the board with the supplied leads: in ampere meter mode the instrument goes **in
   series** with the supply, not across it.
5. If you want event markers, clip the logic inputs to the pins you care about.
6. Start recording, run the scenario on the device, stop, and read the graph.

## Things to watch

- In ampere meter mode the instrument is in series with the power. Swapping the leads means
  measuring the wrong thing.
- The limit is 1 A. A device with a motor, a powerful radio or a battery charger does not belong
  here.
- The interesting numbers are not the average current but the sleep current and the length of the
  peaks. An average is something a multimeter will also give you, and it usually lies in a
  comfortable direction.

## Renting it

It goes home with you: low-power firmware gets written wherever it is comfortable. The leads and
the harness go with it. The daily rate and the term are in the rental block on this page.

## Access

The instrument is in a container on the shelf in the hackspace room, so a plan that includes
hackspace access is required. No induction is needed.
