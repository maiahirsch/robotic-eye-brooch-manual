---
layout: default
title: Robotic Eye Brooch Manual
---

# Robotic Eye Brooch

**Designed and built by Maia Hirsch**

Welcome to the user, maintenance, and repair manual for the Robotic Eye Brooch.

This guide explains how to operate the brooch, charge it, troubleshoot common issues, and replace components if necessary.

---

## Quick Start

1. Turn on the power system.
2. Wait for the Raspberry Pi to boot.
3. Use the control button to cycle between operating modes.

### Mode 1 — Random Mode

The eye moves and blinks randomly.

- 1 LED ON
- Camera tracking OFF

### Mode 2 — Tracking Mode

The camera detects a hand and moves the eye to follow it.

- 2 LEDs ON
- Camera tracking ON

### Mode 3 — Off

The eye and tracking system are inactive.

- LEDs OFF

---

## Components

The brooch contains:

- Raspberry Pi 5
- Arduino
- Arducam IMX519 camera
- SG90 eye movement servo
- SG90 eyelid servo
- Power system
- Push button
- Indicator LEDs
- Custom 3D printed housing

---

## Internal Layout

![Internal layout of the brooch](assets/images/internal-layout.jpg)

---

## Charging

### Raspberry Pi Power System

Add your charging instructions here.

### Servo Power System

Add your charging instructions here.

---

## How It Works

The Raspberry Pi processes the camera feed and detects the location of a hand.

When Tracking Mode is active, the hand position is sent to the Arduino, which controls the servo responsible for moving the eye.

When Random Mode is active, the eye moves and blinks automatically without using the camera.

---

# Troubleshooting

## Brooch Does Not Turn On

Check:

1. The battery is charged.
2. The power switch is ON.
3. The Raspberry Pi power connection is secure.
4. The Arduino is connected.

---

## Eye Does Not Move

Check:

- Servo wiring
- Arduino connection
- Servo power
- Mechanical obstruction around the eye

---

## Eye Moves but Does Not Track

The tracking software may not be running.

Restart the brooch.

If necessary, manually start the software using the instructions below.

---

# Software

The Raspberry Pi project is located at:

```text
~/robotic_brooch/
