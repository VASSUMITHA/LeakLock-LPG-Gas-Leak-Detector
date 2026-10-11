# 🔥 LeakLock: LPG Gas Leak Detector with Escalating Alarm

Arduino-based LPG gas leak detector with 4-level escalating alerts (Safe, Medium, High, Critical) using LEDs and a buzzer. Built during my Embedded IoT System Design internship at Sans Innovations, Salem.

## Features
- Reads gas level (0-1023) on pin A0
- 4 alert levels with matching LED + buzzer pattern
- Serial Monitor logs every reading and status
- MQ-6 gas sensor simulated with a potentiometer

## Alert levels
| Level | Reading | LED | Buzzer |
|---|---|---|---|
| Safe | below 256 | Green | Silent |
| Medium | 256-511 | Yellow | Slow beep |
| High | 512-767 | Orange | Fast beep |
| Critical | 768 and above | Red | Siren |

## Components
Arduino Uno, potentiometer, buzzer, 4 LEDs, 4 x 220 ohm resistors

## Pin connections
| Component | Pin |
|---|---|
| Potentiometer middle | A0 |
| Buzzer + | 3 |
| Green LED | 8 |
| Yellow LED | 9 |
| Orange LED | 10 |
| Red LED | 11 |

## Demo
Video: (https://drive.google.com/file/d/1lWOGm4KvTehPNDjsx7Urzd2llMPNQ5cH/view)
Tinkercad: (https://www.tinkercad.com/things/bnCKdXq4aTc-fantabulous-tumelo-stantia?sharecode=P8kiPDrDVXD1cafkpYApq-O5XFHzf1USxLxCG4A3x9s)

## Future scope
Wi-Fi alerts using ESP8266/ESP32
