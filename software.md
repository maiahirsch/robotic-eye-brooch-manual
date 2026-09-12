---
layout: page
title: Software
---

# Software

[← Back to Manual](index.md)

The Interactive Configuration uses software running on the Raspberry Pi 5 and firmware running on the Interactive Controller.

---

## Raspberry Pi

The Raspberry Pi handles:

- Camera input
- OpenCV
- MediaPipe
- Hand detection
- Tracking logic
- Communication with the controller

The main project directory is:

```text
~/robotic_brooch/

The main tracking program is:

```text
brooch_tracking.py
```

---

## Starting the Program Manually

```bash
cd ~/robotic_brooch
source brooch-env/bin/activate
python brooch_tracking.py
```

---

## Interactive Controller

The Interactive Controller manages:

- Push button input
- Indicator LEDs
- Servo commands
- Communication with the Raspberry Pi

---

## Standalone Controller

The Standalone Controller contains a separate program that:

- Moves the eye randomly
- Blinks automatically
- Does not require the Raspberry Pi
- Does not use the camera

---

## Software Backups

Keep backup copies of:

- Raspberry Pi project folder
- Interactive Controller code
- Standalone Controller code
- Configuration files

A full backup of the Raspberry Pi SD card is also recommended.
