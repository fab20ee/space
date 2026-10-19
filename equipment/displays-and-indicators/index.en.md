---
title: "Displays and Indicators"
seoDescription: "A container of displays at the Tallinn hackspace: TFT, OLED, 1602 character LCDs, LED matrices and seven-segment indicators for Arduino and STM32 prototypes."
specs:
  - { label: "TFT",          value: "a colour screen of about 3.5 inches, with a ribbon" }
  - { label: "OLED",         value: "several monochrome modules around an inch, on breakouts and bare" }
  - { label: "Character",    value: "1602 LCD — two lines of sixteen characters" }
  - { label: "Matrices",     value: "8 × 8 LED" }
  - { label: "Seven-segment", value: "four-digit and single digits, plus a bar graph" }
  - { label: "Contents",     value: "change; the card describes types rather than exact part numbers" }
---

A box of screens for prototypes. Every project eventually runs into "how do I see what is going on
in there", and then the choice begins: show a number, draw a graph, or make do with a blinking
LED.

Everything here is what you try that on, before ordering a display for your own board.

## What is here and what for

- **A TFT of about 3.5 inches** — colour, backlit, connected by a ribbon. For an interface with
  pictures, graphs and buttons. It wants noticeably more pins and more memory than the rest.
- **OLED modules around an inch** — monochrome, over I²C or SPI, two to four wires. The usual
  choice for a small instrument: high contrast, no backlight needed, easy to wire. Some are on
  breakout boards, some are bare with an FPC tail — the latter for people laying out their own
  board.
- **A 1602 character LCD** — two lines of sixteen characters, parallel interface or an I²C
  backpack if one turns up. An old, simple and very predictable thing.
- **8 × 8 LED matrices** — scrolling text, icons, simple animation.
- **Seven-segment indicators** — four-digit and single digits. For when you need to show a number
  and nothing else: a clock, a counter, a temperature.
- **A bar graph** — a column of segments for a level or a progress indication.

## Worth knowing before you wire it up

- **Voltage.** Some modules are 3.3 V, some tolerate 5 V. Putting five volts on a three-volt OLED
  happens once. If there is no clear marking on the board, measure and read the datasheet.
- **Interface.** I²C is two wires and slow, SPI is more wires and fast, parallel is a lot of
  wires. For animation on a TFT the difference matters.
- **The FPC tails on the bare displays are fragile.** They must not be creased and must not be
  tugged: the traces inside break invisibly and the display simply stops working.
- **Libraries.** Almost everything here has a ready library for Arduino and STM32. Start with the
  library's example rather than your own code: that way you find out at once whether the module is
  alive.

## How to use

1. Take a module and read the controller marking on the board — that is what you search for both
   the library and the datasheet with.
2. Wire it on a breadboard and check it with the library example.
3. Put the module back in the box, not in your pocket and not in your own desk drawer.
4. If a module does not work, put it aside separately and tell us, so the next person does not
   lose an evening to it.

The parts for building it up — jumpers, breadboards, wire — are in the [component
boxes](/en/equipment/electronics-components-and-consumables).

## Access

The container is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed.
