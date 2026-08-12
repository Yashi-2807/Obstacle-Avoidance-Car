# Obstacle Avoidance Car

An Arduino-based obstacle avoidance car designed to detect obstacles using an ultrasonic sensor and automatically change direction to avoid collisions.

## Overview

This project was developed as a basic embedded-systems project focused on obstacle detection and motor control.

The car uses an ultrasonic sensor to measure the distance to objects in front of it. When an obstacle is detected within a predefined distance, the car stops, checks the available space on the left and right sides, and selects an appropriate direction.

## How It Works

1. The car moves forward.
2. The ultrasonic sensor measures the distance ahead.
3. If the path is clear, the car continues moving forward.
4. When an obstacle is detected, the car stops.
5. The sensor scans the left and right directions using a servo motor.
6. The measured distances are compared.
7. The car turns toward the more suitable direction.
8. If both sides are blocked, the car moves backwards before changing direction.

## Hardware

- Arduino
- HC-SR04 Ultrasonic Sensor
- Servo Motor
- Motor Driver
- Wheels
- Battery Supply

## Software

- Arduino IDE
- C/C++ (Arduino)

## Obstacle Detection Logic

```text
Start
  ↓
Move Forward
  ↓
Measure Distance
  ↓
Obstacle Detected?
  ├── No → Continue Forward
  │
  └── Yes
        ↓
      Stop
        ↓
   Scan Left & Right
        ↓
   Compare Distances
        ↓
    Choose Direction
        ↓
    Continue Moving
```

## Project Outcome

The project provided hands-on experience with ultrasonic sensing, motor control, servo positioning, distance measurement, and basic automatic obstacle avoidance.

Future Improvements
Speed control using PWM
Improved turning decisions
Additional sensors
More accurate distance measurement
Improved navigation logic

## Project Note

This repository documents the obstacle-avoidance car developed as part of a small academic project.
