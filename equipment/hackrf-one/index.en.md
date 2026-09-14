---
title: "HackRF One SDR Transceiver"
seoDescription: "HackRF One software defined radio in a Tallinn hackspace: receive and transmit from 1 MHz to 6 GHz, 20 MHz of bandwidth, GNU Radio and SDRangel. Open 24/7."
specs:
  - { label: "Frequency range", value: "1 MHz – 6 GHz" }
  - { label: "Mode",            value: "half duplex — receive or transmit, not both at once" }
  - { label: "Bandwidth",       value: "up to 20 Msps, 8-bit I/Q samples" }
  - { label: "Antenna port",    value: "SMA female, 50 Ω, whip antenna included" }
  - { label: "Clocking",        value: "CLKIN and CLKOUT, 10 MHz, for an external reference or syncing units" }
  - { label: "Connection",      value: "micro-USB 2.0, bus powered" }
  - { label: "Software",        value: "GNU Radio, SDRangel, GQRX, SDR#, the hackrf command line tools" }
  - { label: "Licence",         value: "open source hardware — schematics and firmware are public" }
---

A receiver and transmitter that leaves almost all of the signal processing to software on your
computer. The hardware only shifts a slice of the spectrum down to baseband and streams samples
over USB — what happens to them is up to the program you run. The same box is an air band
receiver today, a decoder for your own sensor's telemetry tomorrow, and a rough wideband scanner
up to 6 GHz after that. The range covers most of what you are likely to meet: long wave, VHF,
433 and 868 MHz, 2.4 GHz.

This is a tool for learning radio and debugging your own devices, not a measuring instrument. The
signal path is not calibrated and power readings are approximate. When you need real numbers, the
Rigol RSA3030N spectrum analyser stands next to it.

## What you can do

- Listen to the spectrum and watch the waterfall: broadcast, aviation, amateur bands.
- Capture and decode packets from your own 433 or 868 MHz device — a sensor, a remote, a LoRa module.
- Pick up ADS-B from aircraft, NOAA weather satellites, packets from weather stations.
- Record a signal to a file and take it apart in GNU Radio later, away from the hardware.
- Sweep a band quickly with `hackrf_sweep` to find out where anything is happening at all.
- Build and test your own receiver or transmitter in GNU Radio without laying out a board.

## How to use

1. Screw the antenna onto the **ANT** connector by hand, no spanner. Never transmit without an
   antenna or a dummy load attached.
2. Plug the micro-USB cable into your computer. The cable powers the device; there is no separate
   supply.
3. Check that it is there: `hackrf_info`. It prints the serial number and firmware version.
4. Start SDRangel, GQRX or your own GNU Radio flowgraph, and set frequency and bandwidth.
5. Raise the gain gradually. Copies of a signal appearing at several frequencies in the waterfall
   mean the front end is overloaded — turn the gain down, not up.
6. When you are done, close the software, unplug the cable, and put the antenna and the red
   connector caps back.

The front panel LEDs: **3V3** and **1V8** are power rails, **USB** is the link to the computer,
**RF** means the radio section is on, **RX** and **TX** show receive or transmit. **RESET**
restarts the device; **DFU** is only for firmware flashing — leave it alone otherwise.

## Important

- **Transmitting is not just another feature.** You may only go on air in licence-free bands,
  within their power and duty-cycle limits, or under an amateur radio licence. In Estonia this is
  regulated by the Consumer Protection and Technical Regulatory Authority (TTJA). Responsibility
  sits with whoever pressed transmit.
- **The output is unfiltered.** The transmit path is wideband with no output filtering, so
  harmonics are strong. Even with the carrier inside a permitted band, energy lands outside it.
  Use a dummy load for transmit experiments rather than the whip antenna.
- **Do not jam other people's devices.** Wi-Fi, mobile networks, car keys, emergency services and
  GPS are not a playground. Interfering with them is a criminal matter, not a house-rules matter.
- **The input is fragile.** Do not feed more than −5 dBm into the antenna port, and never connect
  it straight to a transmitter output — use an attenuator. It does not tolerate DC on the input
  either.
- **The antenna port can supply power** (a software-enabled bias tee). Before connecting someone
  else's active antenna or amplifier, make sure it is switched off.
- The device gets warm during long transmissions. That is normal, but do not cover it.

## Access

It lives on the RF bench in the hackspace, so you need a plan that opens the hackspace room. A
short briefing comes before first use: what you may listen to (anything) and what you may transmit
(very little without preparation). It does not leave the space.
