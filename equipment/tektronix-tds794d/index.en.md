---
title: "Tektronix TDS 794D Oscilloscope, 2 GHz"
seoDescription: "A four-channel 2 GHz Tektronix TDS 794D oscilloscope at the Tallinn hackspace: 4 GS/s, digital phosphor. The fastest instrument in the workshop, for fast edges."
specs:
  - { label: "Bandwidth",    value: "2 GHz" }
  - { label: "Channels",     value: "4" }
  - { label: "Sample rate",  value: "4 GS/s on one channel, 2 GS/s on two, 1 GS/s on three or four" }
  - { label: "ADC",          value: "8 bit" }
  - { label: "Display",      value: "built-in, dim — we recommend an external VGA monitor" }
  - { label: "Interfaces",   value: "VGA, GPIB, RS-232, Centronics, a 3.5\" floppy drive" }
---

The fastest instrument in the workshop. Where the
[Micsig TO3004](/en/equipment/oscilloscope-micsig-to3004) and its 300 MHz already show a rounded
step instead of an edge, the TDS 794D shows the edge itself — with the ringing, the overshoot and
everything else that is really happening in it.

You do not need that often, but when you do, nothing else will do. An edge of a few hundred
picoseconds, a clock line in the hundreds of megahertz, a reflection in a badly matched trace:
all of it exists only for an instrument with this bandwidth.

## About the display

**The built-in screen is dim.** This is a 1990s instrument and its backlight has done its time. It
works, and you can find your way around on it, but staring at it all evening is not much fun.

So **connect an external monitor over VGA**. The connector is on the rear panel, and a monitor
usually sits on top of the shelf beside it. The picture there is full and bright, and that settles
the matter.

## What it is good for

- Seeing the real shape of fast edges rather than an approximate silhouette
- Debugging high-speed digital interfaces
- Catching short glitches that a slower instrument simply does not see
- Watching four fast signals at once
- Measuring delays and jitter on a scale where nanoseconds count

For everything else, take the Micsig: it starts in three seconds, has a proper screen and does not
take up half the bench.

## About the sample rate

The sample rate is shared between the channels in use: 4 GS/s on one, 2 on two, 1 on three or
four. Turning on all four channels when you need two means throwing away half your time
resolution for nothing.

## The input

The one thing you can destroy in a second is the input path.

- The voltage limits on inputs with this bandwidth are far lower than on an ordinary
  oscilloscope. Read the marking by the connector before you connect.
- Mains voltage does not go on the input. Not ever, not through anything.
- The probes for this instrument are not the Micsig's probes. Use the ones kept with it.
- Discharge static before connecting: touch the connector body to the chassis.

## How to use

1. Switch it on and let it warm up. It is old, and the first few minutes drift.
2. Connect an external VGA monitor if you intend to work for more than five minutes.
3. Connect a probe and set the attenuation ratio in the channel menu.
4. Autoset gives you a starting point; after that the scale and the trigger level are set by hand.
5. When done, switch it off and put the probes back.

## Access

The oscilloscope is in the hackspace room, so a plan that includes hackspace access is required.
No induction is needed, but read the section about the input before you connect anything.
