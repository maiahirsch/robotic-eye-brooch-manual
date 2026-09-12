---
layout: page
title: System Overview
---

# System Overview

[← Back to Manual](index.md)

The Robotic Eye Brooch combines 3D printed mechanical parts, servo actuation, embedded electronics, and computer vision.

---

## Interactive Configuration

The main signal flow is:

```text
Camera
  ↓
Raspberry Pi 5
  ↓
Interactive Controller
  ↓
Servos + LEDs + Button
```

The Raspberry Pi handles computer vision.

The Interactive Controller handles the physical input/output system.

---

## Vision System

The tracking system uses:

- OpenCV
- MediaPipe
- Raspberry Pi 5
- Camera input

The camera detects hands in front of the brooch.

The detected hand position is used to determine eye movement.

---

## Servo System

The brooch uses two servo motors.

### Eye Movement Servo

Controls:

- Left movement
- Right movement

### Eyelid Servo

Controls:

- Blinking
- Opening the eyelid
- Closing the eyelid

---

## Indicator System

The LEDs show the current operating mode.

- **1 LED** = Random Mode
- **2 LEDs** = Tracking Mode
- **No LEDs** = Off

---

## System Diagram

![System Overview](assets/images/system-overview.png)

---

## Internal Layout

![Servo Layout](assets/images/servo-layout.png)
