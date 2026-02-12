# Bluetooth Controlled RC Car

A mobile controlled robotic car built using Arduino Nano, L298N motor driver and HC-05 Bluetooth module.  
The car receives serial commands from an Android application and drives accordingly.

## Features
- Forward, backward, left and right movement  
- Real-time Bluetooth control  
- Simple serial command protocol  
- Works with any generic Bluetooth controller app  
- Powered by Li-Po battery

## Hardware Components
- Arduino Nano  
- L298N 2A Dual Motor Driver  
- HC-05 Bluetooth Module  
- 2 DC Gear Motors  
- 7.4V Li-Po Battery  
- Chassis and wheels  
- Jumper wires and switch

## Pin Connections

### Motor Driver → Arduino Nano
| L298N Pin | Arduino Pin |
|-----------|-------------|
| IN1 | D11 |
| IN2 | D10 |
| IN3 | D9  |
| IN4 | D8  |

### HC-05 → Arduino
| HC-05 | Arduino |
|------|---------|
| TX   | RX      |
| RX   | TX      |
| VCC  | 5V      |
| GND  | GND     |

## Control Commands

| Command | Action |
|--------|--------|
| F | Move Forward |
| B | Move Backward |
| L | Turn Left |
| R | Turn Right |
| S | Stop |

## How to Use

1. Upload `src/rc_car.ino` to Arduino Nano  
2. Pair HC-05 with mobile (default PIN: 1234)  
3. Open Bluetooth controller app  
4. Send commands F, B, L, R, S to control the car

## Future Scope
- PWM speed control  
- Obstacle avoidance  
- Custom Android app  
- ESP32 upgrade

## Author
Het Patel  
College Project – Robotics Competition
