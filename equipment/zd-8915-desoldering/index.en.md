---
title: "Desoldering Station ZD-8915"
seoDescription: "Vacuum desoldering station at the Tallinn hackspace. ZD-8915 with a heated suction gun removes through-hole components cleanly without damaging the board."
specs:
  - { label: "Type",         value: "vacuum desoldering gun with built-in pump" }
  - { label: "Temperature",  value: "160–480 °C, digital control" }
  - { label: "Tips",         value: "interchangeable suction tips, several diameters" }
  - { label: "Display",      value: "LCD with set and actual temperature" }
---

<!-- TODO: verify against the actual station — heater power, which tip diameters are on the
     bench, condition of the filters. -->

A desoldering station does one thing well: it melts a solder joint and sucks the solder out in
the same motion. The gun has a heated hollow tip and a vacuum pump behind it — press the trigger
and the joint is empty. Removing a 40-pin connector this way takes a minute and leaves the pads
and the component intact; doing it with a plain iron and a spring pump takes much longer and
often lifts a pad.

It is the tool for salvaging parts from old boards, replacing through-hole components, and
cleaning holes before fitting a new part.

## What it is good for

- Removing multi-pin connectors, IC sockets and DIP chips in one piece
- Replacing electrolytic capacitors and other through-hole parts on repairs
- Clearing plated-through holes of old solder
- Salvaging usable components from scrap boards

## Safety

- The tip is at 350 °C or more and the sucked-up solder inside the gun is hot too. Do not touch
  the tip or the collection chamber until it has cooled.
- Put the gun back in its stand every time. Never on the table.
- The pump exhaust carries flux fumes — use the fume extractor or open a window.
- Do not press the tip hard against the pad: heat, wait for the solder to melt, then trigger.

## How to use

1. Switch on and set around 350–380 °C for lead-free solder; a little higher than for
   soldering, because the tip has to melt the joint through the hollow.
2. Pick a tip whose hole is slightly larger than the component lead.
3. Place the tip over the lead, wait two or three seconds for the solder to melt fully, wiggle
   the lead gently so it frees up, and pull the trigger.
4. Move to the next lead. If a joint does not empty, add fresh solder to it first and try again.
5. When done, run the pump for a few seconds with the tip in the air to clear it, clean the tip,
   empty the collection chamber if it is full, and switch off.

## Access

The station is on the electronics bench in the hackspace room, so a plan that includes hackspace
access is required. No induction is needed, but ask someone to show you how to empty the
solder chamber the first time.
