# Wiring Guide

## ESP32 to Motor Driver

| ESP32 | Motor Driver |
|---|---|
| GPIO 18 | IN1 |
| GPIO 19 | IN2 |
| GPIO 23 | ENA |
| GPIO 16 | IN3 |
| GPIO 17 | IN4 |
| GPIO 22 | ENB |
| GND | GND |

## Important Notes

- Connect ESP32 GND to motor driver GND.
- Use a separate battery for motors.
- Do not connect motors directly to ESP32 pins.