# Industrial IO Controller

A general-purpose industrial I/O controller board built around the **RP2040** microcontroller. Designed for rapid prototyping, hardware validation, and testing across a wide range of sensors, actuators, and communication protocols — all from a single PCB.

![Board Status](https://img.shields.io/badge/status-fabricated-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![EDA](https://img.shields.io/badge/EDA-KiCad-orange)

## Features

### Digital I/O
- **20+ configurable digital inputs** — connect buttons, proximity sensors, limit switches, photoelectric sensors, or any industrial-standard digital signal
- **20+ configurable digital outputs** — drive stepper motors, solenoid valves, relays, indicators, and more

### Analog
- **Multi-channel ADC inputs** — for vacuum sensors, pressure transducers, temperature probes, or any 0–3.3V analog signal
- **Current sensing channels** — monitor current draw and detect spikes for motor protection or diagnostics

### Lighting
- **NeoPixel (WS2812B) output** — addressable RGB LED support for status indication, tower lights, or visual feedback

### Storage
- **FRAM (Ferroelectric RAM)** — non-volatile, high-endurance storage for configuration data, counters, or logs that survive power cycles without wear concerns

### Communication Protocols
Designed to test and validate nearly every common protocol from a single board:
- **SPI**
- **I2C**
- **UART**
- **And more** — exposed headers and test points for easy hookup

## Specifications

| Parameter | Value |
|---|---|
| Microcontroller | RP2040 (Dual-core Arm Cortex-M0+, 133 MHz) |
| Digital Inputs | 20+ channels |
| Digital Outputs | 20+ channels |
| Analog Inputs | Multi-channel ADC |
| Current Sensing | Dedicated channels |
| LED Output | NeoPixel (WS2812B) compatible |
| Non-volatile Storage | FRAM |
| Communication | SPI, I2C, UART |
| EDA Tool | KiCad |

## Getting Started

### Viewing the Design
1. Install [KiCad](https://www.kicad.org/) (v7+ recommended)
2. Clone this repository:
   ```bash
   git clone https://github.com/Poornimakulkarni26/Industrial-io-controller.git
   ```
3. Open the `.kicad_pro` project file in KiCad

### Ordering the Board
1. Export Gerber files from KiCad (**File → Fabrication Outputs → Gerbers**)
2. Upload to your preferred PCB manufacturer (JLCPCB, PCBWay etc.)

## Design Highlights

- **Industrial-grade I/O count** — enough channels to prototype full machine control without daisy-chaining expanders
- **Protocol-agnostic test platform** — validate SPI, I2C, UART peripherals without rewiring
- **Mixed-signal capability** — digital I/O, analog sensing, and current monitoring on one board
- **NeoPixel integration** — visual feedback built in, no separate LED driver board needed
- **FRAM over EEPROM** — virtually unlimited write cycles for high-frequency data logging

## Use Cases

- Sensor and actuator validation benches
- Stepper motor driver testing
- Communication protocol bring-up and debugging
- Industrial automation prototyping
- Embedded firmware development and testing

## Author

**Poornima Kulkarni**
Embedded Systems & Industrial Automation Engineer

- GitHub: [@Poornimakulkarni26](https://github.com/Poornimakulkarni26)
https://www.linkedin.com/in/poornima-kulkarni-35ba682a3?utm_source=share_via&utm_content=profile&utm_medium=member_android

## License
This project is open-source under the [MIT License](LICENSE).
