---
title: "Motors and Pumps"
seoDescription: "A container of small motors and pumps at the Tallinn hackspace: brushed motors, gearmotors, diaphragm and peristaltic pumps, and a solenoid valve."
specs:
  - { label: "Motors",       value: "small brushed ones, some with gearboxes" }
  - { label: "Pumps",        value: "diaphragm and peristaltic, low power" }
  - { label: "Also",         value: "a solenoid valve, tubing, small fittings" }
  - { label: "Power",        value: "mostly low-voltage DC, from a few volts to 12–24 V" }
  - { label: "Contents",     value: "change; types rather than part numbers" }
---

The box of things that spin and pump. Unlike the
[steppers](/en/equipment/stepper-motors-and-drivers), the motors here are simple: apply voltage
and it turns, remove it and it stops. There is no position control, but one transistor is enough
to drive them.

The pumps are low power, for water and other non-aggressive liquids: watering plants, moving
liquid between containers, feeding coolant in home-built setups.

## Worth knowing

- **The voltage is written on the motor** or on its bag. More than that buys you more revolutions
  and noticeably less life.
- **Starting current is several times the running current.** A motor that draws half an amp
  running will take two at start-up. Size the driver and the supply for the start.
- **A flyback diode is mandatory.** Any winding produces a voltage spike when switched off, and
  that spike kills a transistor or a microcontroller pin. Without the diode the circuit works
  right up until the first time you turn it off.
- **Some pumps are self-priming and some are not.** A diaphragm pump will lift water by itself, a
  peristaltic one doses neatly, and neither likes running dry.
- **Check whether a pump may sit energised** with no flow. Some models overheat in minutes.

## How to use

1. Take a motor or a pump out of the box and read its markings.
2. Test it on the [bench power supply](/en/equipment/power-supply-owon-spe3102) with a current
   limit: that shows you both the running and the starting current straight away.
3. To drive it, take a transistor or a ready driver module from the [module
   box](/en/equipment/electronic-modules), and do not forget the diode.
4. Test a pump over a sink or a basin, not over a bench full of instruments.
5. Put everything back in the box and coil the tubing.

## Access

The container is in the hackspace room, so a plan that includes hackspace access is required. No
induction is needed.
