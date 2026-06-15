# Ultrasonic Distance Monitor with Relay-Controlled LED

Java-Arduino serial communication project for smart distance monitoring.

## Features
- Real-time distance measurement (HC-SR04 ultrasonic sensor)
- Auto/Manual mode control via GUI and physical switch
- Relay-controlled LED warning light
- LCD display showing distance and status
- Java Swing GUI with serial communication

## Hardware Requirements
- Arduino UNO R3
- HC-SR04 Ultrasonic Sensor
- LCD 1602 (4-bit mode, no I2C)
- 10kΩ Potentiometer
- Push Button
- Slide Switch (SPDT)
- 5V Relay Module
- Red LED + 1kΩ Resistor
- Jumper wires & Breadboard

## Pin Connections
| Pin | Component |
|-----|-----------|
| 2   | LCD RS |
| 3   | LCD E |
| 4   | LCD D4 |
| 5   | LCD D5 |
| 6   | LCD D6 |
| 7   | LCD D7 |
| 8   | Ultrasonic TRIG |
| 9   | Ultrasonic ECHO |
| 10  | Push Button |
| 11  | Slide Switch |
| 12  | Relay Control |
| A0  | Potentiometer |

## Serial Protocol
Arduino → Java: `DIST:45.2`, `LED:ON`, `MODE:AUTO`
Java → Arduino: `THRESH:15`, `LED:ON`, `MODE:MANUAL`

## Author
[Your Name] - Course Project

## License
MIT