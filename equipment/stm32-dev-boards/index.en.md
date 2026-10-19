---
title: "STM32 Development Boards"
seoDescription: "A container of STM32 development boards at the Tallinn hackspace: Nucleo H7, G4, U0 and U5, ST-LINK V3 probes including the V3-PWR with power measurement."
specs:
  - { label: "Nucleo boards", value: "NUCLEO-H7S3L8, NUCLEO-U031R8 (two), NUCLEO-G431RB, NUCLEO-U545RE-Q" }
  - { label: "Probes",       value: "ST-LINK V3-PWR and several compact ST-LINK V3" }
  - { label: "Cables",       value: "ribbon cables for the ST-LINKs" }
  - { label: "Adapters",     value: "STDC14 → CatCon, the connector on RW boards" }
  - { label: "Contents",     value: "change as boards are added; the list is correct as of 19 October 2026" }
---

A container of boards you can start an STM32 project on without soldering or laying out anything.
Each Nucleo is a microcontroller broken out to headers with a programmer already on board: plug in
USB and write code.

The boards are deliberately different — STM32 has several families and they are for different
things:

- **NUCLEO-H7S3L8** — Cortex-M7, up to 600 MHz. The fastest in the box: graphics, signal
  processing, anything an ordinary microcontroller runs out of steam on.
- **NUCLEO-G431RB** — Cortex-M4 with a maths accelerator. The family for motor control and digital
  power.
- **NUCLEO-U031R8** — Cortex-M0+, ultra-low power. For things that live on a cell for years.
  There are two of these — handy when you need to bring up a link between two devices.
- **NUCLEO-U545RE-Q** — Cortex-M33 with TrustZone. Also low power, but with hardware security.

The others are one of each.

## The probes

There are several compact **ST-LINK V3** units in the box — ordinary debug probes, for boards that
do not have one of their own.

Separately there is the **ST-LINK V3-PWR**. It is a probe and a power measurement unit in one: it
supplies the board at 1.6–3.6 V and at the same time measures current from 100 nA to 550 mA, at up
to a hundred thousand samples a second, synchronised with code execution. So you see not just "how
much it eats" but what each part of the firmware costs.

If you need a wider range, or the device is not an STM32, the
[Nordic Power Profiler Kit II](/en/equipment/power-profiler-kit-ii-nordic-ppk2) is nearby: up to
1 A, 0.8–5 V and eight logic inputs, though with no debugger attached to it.

## The CatCon adapters

The box holds adapters from **STDC14** — the standard 14-pin ST-LINK connector — to **CatCon**, the
connector used on KIISU and other RW boards. Without one you simply cannot attach a probe to those
boards, so if you are working on RW hardware, start with that adapter.

## The contents change

The list above is correct **as of 19 October 2026**. The box is a living thing: boards get added,
and sometimes they go off into projects. If something on the list is not there, that happens — ask
us.

And the other way round: **if your project needs a development board we do not have, write to
us.** We are usually happy to buy one — it costs less than you would think, and the next person
will want it too.

## How to use

1. Take a board, and a probe with a cable if you need one, from the container.
2. Install STM32CubeIDE, or whatever environment you are used to.
3. Nucleo boards need no separate probe — it is on the board, so connect over USB.
4. For your own board take an ST-LINK V3 and the right cable; for RW boards, the CatCon adapter.
5. Put everything back in the container, cables included. Cables are what goes missing first.

## Access

The container is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed.
