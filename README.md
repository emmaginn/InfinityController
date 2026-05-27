# InfinityController
Joola Infinity Robot Controller

An unofficial Android controller app for the JOOLA Infinity table tennis robot.

This project was created to keep the Kickstarter-only JOOLA Infinity robot usable after the original app functionality was retired. The app connects directly to the robot over Bluetooth Low Energy and provides shot control, landing-point selection, sequence playback, random drills, saved sequences, and calibration tools.

> This project is not affiliated with, endorsed by, or supported by JOOLA. JOOLA and JOOLA Infinity are trademarks of their respective owners.

---

## Features

- Bluetooth LE connection to the JOOLA Infinity robot
- Basic shot builder with:
  - Ball type: Normal, Serve, Lob
  - Spin: Float, Topspin, Backspin, Max Topspin, Max Backspin, Sidespin Right/Left
  - Power: Light, Medium, Strong, Extreme
  - Landing-point grid
- One-ball test shots
- Sequence mode
  - Tap landing points in order
  - Each sequence step stores its own Ball / Spin / Power settings
  - Repeat sequence control
  - Ball interval control
- Random mode
  - Select multiple landing points
  - Randomized shot selection
  - Number-of-balls and interval controls
- Saved sequences
  - Save current sequence
  - Load saved sequence
  - Rename saved sequence
  - Delete saved sequence
  - Play saved sequence
- Per-landing-point fine tuning
  - Left/right correction
  - Short/long correction
  - Height correction
- Robot-wide calibration
- Advanced manual shot creator
  - Direct M1/M2 motor speed control
  - X/Y/Z axis control
  - Raw command testing/debug tools
- Emergency stop controls

---

## Current Status

The app is functional and actively being calibrated.

Confirmed working areas include:

- Bluetooth connection
- Basic shot firing
- One-shot mode
- Sequence mode
- Random mode
- Saved sequences
- Normal shot calibration in progress
- Lob shot calibration in progress
- Per-point fine tuning
- Neutral Z head rotation for non-sidespin shots
- Intentional Z head rotation only for sidespin shots

The shot table is based on recovered app behavior, community testing, and manual calibration. Some shot combinations may still need tuning depending on robot placement, table setup, ball type, and individual robot variation.

---

## Important Safety Notice

This app controls a physical table tennis robot.

Before testing:

- Point the robot safely.
- Keep people, pets, and breakable objects away from the firing path.
- Start with low speed / low power shots.
- Use one-ball test mode before running full sequences.
- Be ready to press Stop if something behaves unexpectedly.

Use at your own risk.

---

## Requirements

- Android phone or tablet
- JOOLA Infinity robot
- Bluetooth enabled
- Location/Bluetooth permissions granted when prompted

Android Bluetooth permissions vary by version:

- Android 12 and newer require Bluetooth Scan / Connect permissions.
- Android 11 and older may require Location permission for BLE scanning.

---

## Building the App

1. Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
