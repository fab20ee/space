---
title: "Miniware TS1C Cordless Soldering Iron"
seoDescription: "The Miniware TS1C cordless soldering iron at the Tallinn hackspace: a supercapacitor instead of a battery, five-minute charge, 100–400 °C, TS80-series tips."
specs:
  - { label: "Pen power",     value: "750 F supercapacitor, no battery" }
  - { label: "Run time",      value: "about 10–12 minutes per charge" }
  - { label: "Charging",      value: "5–7 minutes in the dock" }
  - { label: "Heating power", value: "up to 36 W" }
  - { label: "Temperature",   value: "100–400 °C, ±3 % stability" }
  - { label: "Tips",          value: "TS80 / TS80P series, 3.5 mm interface" }
  - { label: "Dock",          value: "128 × 64 OLED, two buttons and an encoder, Bluetooth link to the pen" }
  - { label: "Dock supply",   value: "USB-C PD, up to 45 W at 20 V" }
---

A soldering iron with no cable. Not "with a battery" but with a supercapacitor: the pen charges in
the dock in five minutes and then works on its own for ten or twelve.

What that changes is not the power but the geometry of the work. A soldering iron's cable catches
on things, pulls your hand sideways and spoils your aim on fine pitch. With no cable you can come
at the board from any side, work inside an enclosure, hold something up in the air, or reach into
a rack — places a corded iron simply does not reach.

## How it works

The pen and the dock are two separate devices talking over Bluetooth. That is why the dock's
screen says **Search device** at switch-on: it is looking for the pen. The temperature is set with
the encoder on the dock, and the two buttons are two presets.

A supercapacitor instead of a battery also means the thing does not degrade with charge cycles and
does not mind being left flat. The price is run time, and the run time really is short.

## When to take this, and when the station

- **The TS1C** — quick jobs and awkward places: tack a wire inside a case, fix a single joint,
  work where a cable is in the way.
- **[The ATTEN ST-8802 station](/en/equipment/soldering-station-atten-st-8802)** — anything longer
  than ten minutes at a stretch, large copper masses, connectors, ground planes.

Trying to build a whole board on the TS1C means ten minutes of soldering and five of waiting, over
and over.

## How to use

1. Take the pen out of the dock. If the dock has no power, fetch a 65 W USB-C PD brick: ours are
   plugged into sockets around the hackspace and kept in the common box of power supplies.
2. Check on the screen that the dock has found the pen and is showing its temperature.
3. Set the temperature with the encoder. For ordinary lead-free solder 320–350 °C is enough, and
   just over 300 °C for leaded.
4. Solder. When the pen starts to cool off, put it back in the dock — charging is faster than you
   expect.
5. When you finish, leave the pen in the dock.

## Tips

It takes TS80 and TS80P series tips — fine ones, which is exactly what the iron is built for:
small parts, wires, fine-pitch leads. Change the tip cold.

A fine tip is no good for a massive joint on any iron: it cannot deliver heat fast enough, so you
end up holding it there longer and cooking the board around it.

Spare tips live either in the container with the iron or in the big consumables box.

## Safety

- A cordless iron looks harmless and is still an iron at 400 °C. It goes in the dock, nowhere
  else.
- Do not leave the pen hot outside the dock, even for a minute: there is no cable here to remind
  you it exists.
- Do not try to charge the pen from anything but its own dock or the dock's USB-C.

## Renting it

This one goes home with you — being cordless is exactly when that is useful. **The power supply is
not part of the rental**: our USB-C PD bricks are shared, so bring your own, 45 W or better. The
daily rate and the term are in the rental block on this page.

## Access

The iron is at the soldering bench in the hackspace room, so a plan that includes hackspace access
is required. No induction is needed.
