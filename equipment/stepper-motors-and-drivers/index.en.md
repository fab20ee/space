---
title: "Stepper Motors and Drivers"
seoDescription: "A container of stepper motors, servos and drivers at the Tallinn hackspace: for mechanisms, feeds, rotary axes and home-built machines."
specs:
  - { label: "Steppers",     value: "various frame sizes, in bags" }
  - { label: "Servos",       value: "compact ones, including MG90S and SG90" }
  - { label: "Drivers",      value: "stepper driver boards" }
  - { label: "Mechanics",    value: "timing belts and small hardware" }
  - { label: "Contents",     value: "change; types rather than part numbers" }
---

The box of everything that moves on command. Stepper motors for precise positioning, servos for
turning to an angle, drivers for the steppers and a little mechanical hardware to go with them.

## Stepper or servo

The difference is fundamental, and the choice shapes the whole design:

- **A stepper motor** turns exactly the number of steps you command and holds its position while
  current flows. It does not know where it is: if a step is missed, nobody finds out until you run
  into an endstop. It needs a driver and usually its own supply, higher than logic voltage.
- **A servo** is given an angle and reaches it with its own internal feedback. No driver needed —
  three wires, one of them control. The travel is usually limited, though, and the accuracy
  depends on how cheap the gearbox inside is.

For a feed, a machine axis, a rotary table — a stepper. For "turn this flap thirty degrees" — a
servo.

## About drivers and current

A stepper driver is set up for the particular motor, and the main parameter is the **current
limit**. Setting it higher than the winding can take means heating the motor until it smells, and
possibly burning the driver.

- Look up the rated current on the motor itself or on its bag.
- Drivers get hot in use, properly hot. The heatsink on a driver chip is not decoration.
- **Do not disconnect a motor from a running driver.** Breaking a winding under current kills the
  output stage: it is the most common cause of death for cheap drivers.

## Power

A motor does not run off your board. A microcontroller's 5 V rail is good for an unloaded servo at
best, and even that will sag the supply enough to reset the controller. Use a separate source: the
[power supplies](/en/equipment/power-supply-owon-spe3102) are on the same bench.

## How to use

1. Take the motor together with its bag: the connector for it is usually in there.
2. Find the rated current and voltage and set the driver to them **before** first power-up.
3. Test it on the bench, with no mechanics attached, before building it into anything.
4. Put everything back in the box and in the same bag.

## Access

The container is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed.
