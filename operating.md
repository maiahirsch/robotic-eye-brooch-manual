---
layout: page
title: Operating the Brooch
---

# Operating the Brooch

[← Back to Manual](index.md)

This page explains how to use the brooch in the Interactive Configuration.

The Interactive Configuration uses:

- Raspberry Pi 5
- Geekworm X1205 power system
- Interactive Controller
- Camera
- Two servos
- Push button
- Indicator LEDs

---

## Button Controls

| Button Press | Mode | LEDs | Behavior |
|---|---|---|---|
| First press | Random Mode | 1 LED ON | Eye moves and blinks randomly |
| Second press | Tracking Mode | 2 LEDs ON | Camera activates and hand tracking controls the eye |
| Third press | Off | LEDs OFF | Eye system is inactive |

---

## Random Mode

Press the push button once.

In Random Mode:

- One indicator LED turns on.
- The camera is not used.
- The eye looks left and right automatically.
- The eyelid blinks automatically.

This mode is useful when interactive tracking is not required.

---

## Tracking Mode

Press the push button a second time.

In Tracking Mode:

- Two indicator LEDs turn on.
- The camera activates.
- The Raspberry Pi detects hands using OpenCV and MediaPipe.
- A person standing in front of the brooch can influence the eye movement.
- The eye can look left or right based on detected hand position.
- The blinking mechanism can also respond to tracking behavior.

---

## Heat Warning

The Raspberry Pi 5 performs real-time computer vision while in Tracking Mode.

Because the Raspberry Pi is worn inside a blazer pocket, heat can build up quickly.

**Do not use the Interactive Configuration continuously for more than approximately 5 minutes.**

For longer operation, use the [Extended Wear Configuration](extended-wear.md).

---

## Turning the Brooch Off

Press the button until:

- Both indicator LEDs are off.
- The eye is inactive.

After use, power off the Raspberry Pi system properly before disconnecting power.
