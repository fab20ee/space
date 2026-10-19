---
title: "TI and NXP Development Boards"
seoDescription: "Texas Instruments and NXP development boards at the Tallinn hackspace: a LaunchPad with the MSPM0L1117 and the FRDM-MCXN947. For trying something other than STM32."
specs:
  - { label: "Texas Instruments", value: "LaunchPad with the MSPM0L1117, Arm Cortex-M0+ core" }
  - { label: "NXP",          value: "FRDM-MCXN947, the MCX N family with two Cortex-M33 cores and an NPU" }
  - { label: "Condition",    value: "both boards still in their factory boxes, with cables and documentation" }
  - { label: "Contents",     value: "these two so far; the set is meant to grow" }
---

A container for anyone who needs to try something that is not an STM32.

Microcontroller vendors are incompatible with each other at every level: peripherals, development
environment, debugger, the way you set up a clock tree. Choosing a vendor for a project is a
decision you live with for years, and making it from a datasheet without ever holding the board is
an odd way to go about it. So boards from different vendors sit side by side.

## What is here

- **A TI LaunchPad with the MSPM0L1117.** MSPM0 is Texas Instruments' inexpensive Cortex-M0+
  family, aimed at simple and cheap devices. The environment is Code Composer Studio; the debugger
  is on the board.
- **An NXP FRDM-MCXN947.** The other end: the MCX N family, with two Cortex-M33 cores and a neural
  network accelerator on board. The environment is MCUXpresso.

Both are still in their factory boxes, with their cables and paperwork.

## What it is good for

- Comparing development environments before you pick a vendor for your own project
- Trying what STM32 does not have: an NPU on the NXP side, a price point on the TI side
- Reproducing a vendor's example without buying the board
- Finding out how painful porting your code between architectures is — normally you learn that too
  late

If you already work with STM32, the [STM32 board container](/en/equipment/stm32-development-boards)
with its probes is next to this one.

## The set is meant to grow

This is everything from TI and NXP so far: one board each. The list is correct **as of 19 October
2026**.

**If your project needs a particular development board, write to us.** We are usually happy to buy
one, and more often than not you will not be the only one who wants it.

## How to use

1. Take the board out of the container with its box — the cable and the documentation are in
   there.
2. Install the vendor's environment: Code Composer Studio for TI, MCUXpresso for NXP. Both are
   free.
3. Both boards have the debugger on board, so no separate probe is needed — USB is enough.
4. Put the board back in its box and the box back in the container. The cable too.

## Access

The container is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed.
