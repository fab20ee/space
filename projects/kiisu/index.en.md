---
title: "KIISU — a pocket tool for radio and NFC"
seoDescription: "KIISU is a credit-card-sized board compatible with Flipper Zero firmware: Sub-GHz, NFC, RFID, IR, BLE, iButton, GPIO. Developed by RainWalker in Tallinn; prototypes are built in the FAB20 workshop."
---

KIISU is a device the size of a bank card that does what a Flipper Zero does and runs its
firmware: Sub-GHz radio, NFC and RFID, an infrared port, Bluetooth Low Energy, iButton and
exposed GPIO. It is made by RainWalker — the same team behind FAB20 — and the workshop became the
project's home lab: prototypes are soldered and debugged here, and the radio side is tested here
too.

## What is inside

Two microcontrollers — an STM32WB55 (radio and BLE) and an STM32G431 (170 MHz, main logic). A
CC1101 transceiver for Sub-GHz, an ST25R3916 for NFC, an IR receiver and transmitter, an
accelerometer with a compass, temperature, humidity and ambient light sensors; optionally a gas
sensor and a rangefinder. Powered by a LIR2032 cell or USB Type-C.

## Two versions

KIISU V4BR — the main card-format board. KIISU SMOL — a modular variant for those who want a kit
rather than a finished device.

## Open

Schematics and firmware are on GitHub, in a public repository. The device is sold through the
official store and partners in the USA, Europe, Poland and India.

## How the workshop helped

The hot-air soldering station and the BGA rework station for assembling and reworking
prototypes, the microscope for inspecting fine-pitch soldering, the oscilloscope and the spectrum
analyzer for debugging power and RF. All of it stands in the hackspace and is available to any
member on a plan.
