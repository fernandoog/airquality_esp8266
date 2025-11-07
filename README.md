# Air Quality ESP8266

PlatformIO project for testing ESP8266 with MQ-135 gas sensor.

## Description

This project demonstrates how to use an MQ-135 gas sensor with ESP8266 using PlatformIO. The MQ-135 sensor can detect various gases including CO2, alcohol, benzene, NH4, and smoke.

## Features

- ESP8266 microcontroller support
- MQ-135 gas sensor integration
- PlatformIO development environment
- Real-time gas detection

## Hardware Requirements

- ESP8266 development board (NodeMCU, Wemos D1, etc.)
- MQ-135 gas sensor
- Jumper wires
- Optional: Display for readings

## Installation

1. Install PlatformIO IDE or PlatformIO Core
2. Clone this repository
3. Open the project in PlatformIO
4. Connect the MQ-135 sensor to ESP8266:
   - VCC to 3.3V or 5V
   - GND to GND
   - A0 to analog pin (A0)

5. Build and upload:
```bash
pio run --target upload
```

## Usage

After uploading, open the serial monitor to see gas readings:

```bash
pio device monitor
```

## Configuration

Adjust sensor calibration and thresholds in the code based on your environment and requirements.

## Project Structure

```
airquality_esp8266/
├── src/
│   └── main.cpp (or main.ino)
├── platformio.ini
└── README.md
```

## MQ-135 Sensor

The MQ-135 sensor can detect:
- CO2 (Carbon Dioxide)
- Alcohol
- Benzene
- NH4 (Ammonia)
- Smoke

## Author

Fernando Ortega Gorrita (@fernandoog)

## License

See LICENSE file for details.
