# Haptic Control Application

A BLDC motor position/angle control application using SimpleFOC library for Arduino Uno.

![Haptic Control Demo](.graphics/haptic_control_cut.gif)

## Overview

This project implements Field Oriented Control (FOC) for precise angle positioning of a BLDC motor with magnetic sensor feedback. It enables haptic feedback applications by allowing smooth and accurate motor positioning via serial commands.

## Hardware Requirements

- **Microcontroller:** Arduino Uno
- **Motor:** BLDC Motor (11 pole pairs)
- **Driver:** 3-PWM BLDC Driver (pins 9, 5, 6 with enable on pin 8)
- **Sensor:** AS5600 Magnetic Sensor (I2C)
- **Power Supply:** 12V DC

## Wiring

| Component | Pin |
|-----------|-----|
| PWM A     | 9   |
| PWM B     | 5   |
| PWM C     | 6   |
| Enable    | 8   |
| Sensor    | I2C (SDA/SCL) |

## Software Requirements

- [PlatformIO](https://platformio.org/) (VS Code extension recommended)
- SimpleFOC Library v2.3.4 (installed automatically)

## Installation & Launch

### 1. Clone the Repository

```bash
git clone <repository-url>
cd haptic_control
```

### 2. Open in VS Code with PlatformIO

Open the project folder in VS Code with the PlatformIO extension installed.

### 3. Build the Project

```bash
pio run
```

Or use the PlatformIO toolbar: click the **checkmark icon** (✓) to build.

### 4. Upload to Arduino

```bash
pio run --target upload
```

Or click the **right arrow icon** (→) in PlatformIO toolbar.

