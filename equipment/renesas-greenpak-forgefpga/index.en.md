---
title: "Renesas Boards: GreenPAK and ForgeFPGA"
seoDescription: "A container of Renesas boards at the Tallinn hackspace: a GreenPAK Lite Dev Board with a set of DIP-packaged chips, and a ForgeFPGA Evaluation Board with 1120 LUTs."
specs:
  - { label: "GreenPAK",     value: "GreenPAK Lite Dev. Board Rev 1.1 with an extension set: SLG46537V-DIP and others" }
  - { label: "ForgeFPGA",    value: "ForgeFPGA Evaluation Board, SLG47910 device" }
  - { label: "Inside the ForgeFPGA", value: "1120 six-input LUTs, 1120 flip-flops, 32 kbit BRAM, 50 MHz oscillator, PLL, 19 GPIOs" }
  - { label: "Software",     value: "Go Configure Software Hub, free" }
  - { label: "Contents",     value: "change as boards are added; the list is correct as of 19 October 2026" }
---

Two boards about the same idea: getting a handful of small logic off your board by replacing it
with one chip you configured yourself.

## GreenPAK

A GreenPAK is a chip containing logic gates, comparators, counters, timers, a DAC and a little
analogue glue, joined by a programmable matrix. You draw a schematic in the editor, program it
into the chip — and from then on it is an ordinary small IC that works with no processor and no
firmware in the usual sense.

It covers exactly the layer that normally eats board space: a power-on delay, a simple latch, a
couple of gates, a voltage monitor, a pulse shaper. Five packages become one, the size of a SOT.

The **GreenPAK Lite Dev. Board Rev 1.1** is the programmer and the test bed: a chip goes in the
socket, the software loads a configuration into it, and it can emulate the design without
programming it at all. Beside it is an extension set of chips in DIP packages — **SLG46537V-DIP**
and others. The DIP package is there so you can push the chip into a breadboard and build a
circuit around it by hand.

## ForgeFPGA

The **ForgeFPGA Evaluation Board** carries the **SLG47910**, a small and cheap FPGA. Inside are
1120 six-input LUTs, as many flip-flops, 32 kbit of block RAM, a 50 MHz oscillator and a PLL, and
19 GPIOs.

This is not a Xilinx or an Altera: a processor core will not fit. What does fit is what an FPGA is
usually for in a small device: cycle-level signal handling, unusual interfaces, counters and
decoders that a microcontroller either cannot keep up with or spends all its time on.

The board is USB powered.

## Software

Both boards work with **Go Configure Software Hub**, Renesas's free environment. The GreenPAK is
configured with the mouse in a graphical editor; the ForgeFPGA in Verilog.

## What to take them for

- Clearing a scattering of logic and timers off a board, replacing it with one chip
- Building a power monitor, a delay or a latch with no microcontroller
- Trying an FPGA without buying a development board that costs hundreds
- Taking hard-timing work off a microcontroller
- Simply seeing how it all works: both environments are free, and the DIP chips go straight into a
  breadboard

## The contents change

The list is correct **as of 19 October 2026**. Boards get added, and sometimes they go off into
projects. If something is not there, ask us.

And if your project needs a board we do not have, write: we are usually happy to buy one.

## Access

The container is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed.
