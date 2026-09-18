---
title: "tinySA Ultra Portable Spectrum Analyser"
seoDescription: "Pocket spectrum analyser, 100 kHz – 5.3 GHz, at the Tallinn hackspace: tinySA Ultra with a built-in signal generator. Battery powered, and available to rent."
specs:
  - { label: "Input range",      value: "100 kHz – 800 MHz, up to 5.3 GHz in Ultra mode" }
  - { label: "Resolution filters", value: "0.2 / 1 / 3 / 10 / 30 / 100 / 300 / 600 / 850 kHz" }
  - { label: "Generator",        value: "sine 100 kHz – 800 MHz, −115…−19 dBm in 1 dB steps; square wave up to 4.4 GHz" }
  - { label: "Max input",        value: "+6 dBm at 0 dB attenuation, ±5 V DC" }
  - { label: "Display",          value: "4\" touch, 480 × 320" }
  - { label: "Power",            value: "internal battery, about 2 hours; charges over USB-C" }
  - { label: "Storage",          value: "microSD card in the slot, screenshots go to it" }
  - { label: "In the box",       value: "telescopic SMA antenna, wrist strap" }
---

A spectrum analyser shows at which frequencies there is energy and how much. The tinySA Ultra
does that from 100 kHz to 5.3 GHz, fits in a jacket pocket and runs off its own battery. You use
it to check whether a module transmits and on which frequency, and to track down where noise is
coming from — where the question came up, rather than back on the bench.

We already have a [RIGOL RSA3030N](/en/equipment/spectrum-analyzer-rigol-rsa3030n): big,
accurate, with VNA and EMI. The RIGOL sits on the bench and measures properly; the tinySA can be
carried away. Interference in a flat, a radio module checked on the spot, an analyser taken to a
site — that is the tinySA. Honest levels, dynamic range and pre-compliance work — that is the
RIGOL.

It also has a signal generator, so the instrument works the other way round too: send a signal
and see what a filter, a cable, an attenuator or a receiver does to it.

## What it is good for

- Checking that a 433/868 MHz, Wi-Fi or BLE module transmits where it should and not on the
  next channel
- Looking at your transmitter harmonics and deciding whether it needs a filter
- Finding a source of interference: a switching supply, a charger, an LED strip driver
- Comparing two antennas and seeing which one is better at the frequency you care about
- Testing a cable, an adapter or an attenuator with the built-in generator
- Checking how busy a band is before you put your own radio on it

## The generator

Below 800 MHz it puts out a sine wave from −115 to −19 dBm in 1 dB steps — enough to feed a
receiver a controlled weak signal and find its sensitivity threshold.

Above 800 MHz and up to 4.4 GHz the output is a square wave. A square wave is rich in harmonics,
so it is no use as a level reference; for checking whether a signal gets through, it is enough.

The signal leaves through the same RF connector that the input uses. The separate CAL connector
is a 30 MHz reference for the instrument self-test, not a second output.

## How not to blow the input

Printed on the case next to the connector: "+6 dBm RF, 5 VDC Max".

- +6 dBm is the absolute maximum at zero attenuation. A transmitter output, even a small one,
  goes in through an attenuator and nothing else.
- DC on the input must stay below ±5 V, and zero is the safe value. A cable carrying power on
  the centre conductor (a mast amplifier, an active GPS antenna) needs a DC block.
- Before connecting a long cable or an antenna, touch the connector body against the chassis to
  discharge static.
- SMA is tightened with fingers — no spanner, no cross-threading.

Attenuators, DC blocks, adapters and cables live in a separate RF container with its own card
and its own sticker.

## How to use

1. The instrument is in a plastic container on the shelf. Its place on the shelf carries the
   same M06 sticker — that is where it goes back.
2. Switch on and check the charge. It charges over USB-C and runs about two hours on a full
   battery.
3. Set start and stop frequencies, or a centre frequency and a span.
4. Ultra mode is already unlocked on this unit, so it sweeps above 800 MHz out of the box. If a
   firmware update leaves the sweep stuck at 800 MHz, turn it back on: CONFIG → MORE → ENABLE
   ULTRA, unlock code 4321.
5. Narrow the resolution bandwidth to see narrow signals, widen it to sweep faster. At 0.2 kHz a
   full span takes a very long time, so use the narrow filters on a narrow span.
6. A marker and peak search read frequency and level better than your eye reads the grid.
   Screenshots go to the microSD card.
7. The telescopic antenna is for hunting interference and for "signal / no signal" answers. Level
   measurements need a cable, and its loss has to be taken into account.
8. Switch off, collapse the antenna, put the instrument back in its container and the container
   back in its place.

## Renting it

This one goes home with you: booked on the site, picked up by the code on the sticker at any hour.
Most people take it to find what is making noise at home or in their workshop, or to a site where
they are putting up radio. The daily rate and the term are in the rental block on this page.

## Access

The container is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed, but read the section about the input before you connect anything to it.
