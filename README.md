# SIM - Smart Industrial Mesh

Distributed IoT monitoring system for industrial applications using ESP32 mesh network.

## Overview

Real-time monitoring and anomaly detection for industrial equipment using wireless sensor nodes with edge processing capabilities.

## Hardware

- 2x ESP32-WROOM-32 microcontrollers
- 1x MPU-6050 accelerometer (vibration monitoring)
- 1x DS18B20 temperature sensor
- Breadboards and wiring

## System Architecture
```
[Node A: Sensor] <--ESP-NOW--> [Node B: Gateway] <--USB--> [Supervisor PC]
```

## Current Status

**Initial Development Phase**
- Project structure established
- Core libraries in development
- Hardware integration pending

## Project Structure
```
SIM/
├── lib/               Shared libraries
├── node-vibration/    Vibration monitoring node
├── node-gateway/      Gateway node
├── docs/              Technical documentation
└── tests/             Test suites
```

## Development

Built with PlatformIO for embedded development.
```bash
# Build
pio run -e node-vibration

# Upload (with hardware connected)
pio run -e node-vibration -t upload -t monitor
```

## License

MIT
