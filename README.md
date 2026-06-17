# ESP32 Bluetooth Controlled Car

A simple Bluetooth-controlled robot car project using ESP32, Arduino IDE, and a motor driver module such as L298N.

## Overview

This project allows you to control a small robot car using Bluetooth commands sent from a mobile phone. The ESP32 receives Bluetooth serial commands and controls two DC motors through a motor driver.

## Features

* Bluetooth control using ESP32
* Forward, backward, left, right, and stop commands
* Simple Arduino IDE code
* Suitable for beginner robotics projects
* Easy to modify and expand

## Hardware Requirements

* ESP32 development board
* L298N motor driver module or similar motor driver
* 2 DC motors
* Robot car chassis
* Battery pack
* Jumper wires
* Android phone with a Bluetooth serial controller app

## Pin Configuration

| ESP32 Pin | Motor Driver Pin | Description       |
| --------- | ---------------- | ----------------- |
| GPIO 18   | IN1              | Motor A direction |
| GPIO 19   | IN2              | Motor A direction |
| GPIO 23   | ENA              | Motor A enable    |
| GPIO 16   | IN3              | Motor B direction |
| GPIO 17   | IN4              | Motor B direction |
| GPIO 22   | ENB              | Motor B enable    |

## Bluetooth Device Name

After uploading the code, the ESP32 Bluetooth name will be:

```text
ESP32_Car
```

Pair your phone with this device name.

## Bluetooth Commands

| Command | Action        |
| ------- | ------------- |
| F       | Move forward  |
| B       | Move backward |
| L       | Turn left     |
| R       | Turn right    |
| S       | Stop          |

## How to Use

1. Open the project in Arduino IDE.
2. Select your ESP32 board from the Boards menu.
3. Connect the ESP32 to your computer.
4. Upload the code.
5. Open a Bluetooth serial controller app on your phone.
6. Pair with `ESP32_Car`.
7. Send commands such as `F`, `B`, `L`, `R`, or `S`.

## Project Structure

```text
esp32-bluetooth-car/
│
├── ESP32_Bluetooth_Car/
│   └── ESP32_Bluetooth_Car.ino
│
├── docs/
│   ├── wiring.md
│   └── bluetooth-commands.md
│
├── images/
│   └── circuit-diagram.png
│
├── README.md
├── LICENSE
└── .gitignore
```

## Notes

* This project is designed for ESP32 boards.
* The `BluetoothSerial.h` library is used for Bluetooth serial communication.
* Make sure your motor driver and ESP32 share a common GND.
* Do not power motors directly from the ESP32 board.

## License

This project is licensed under the MIT License.
