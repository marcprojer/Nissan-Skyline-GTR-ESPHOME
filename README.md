# Nissan Skyline GTR ESPHome Project

> **Note**: This README was generated with AI assistance.

This project controls lighting for a Nissan Skyline GTR model car using ESPHome and ESP32.

## Hardware Setup

### ESP32 Configuration
- **Board**: ESP32 Dev Kit
- **Framework**: Arduino

### GPIO Pin Assignments
- **GPIO 18**: Underbody lighting (via relay - LOW active)
- **GPIO 19**: Turn signals/blinkers (via relay - LOW active) --> WIP!
- **GPIO 21**: Headlights (direct LED control - HIGH active) --> WIP!

### Components
- **2x Relays**: For underbody lighting and blinkers (LOW-active)
- **SMD LEDs**: Direct connection to GPIO 21 for headlights
- **ESP32**: Main controller

## Lighting Features

### Home Assistant Integration
The following entities are exposed to Home Assistant:

#### Lights
- **Underbody Beleuchtung** - Simple on/off control
- **Blinker** - Automatic strobe effect (500ms on/off cycle)

#### Switches  
- **Scheinwerfer** - Direct LED headlight control

## Files

- `wip.yaml` - Main ESPHome configuration file

## Usage

1. Flash the `wip.yaml` configuration to your ESP32
2. Connect hardware according to GPIO pin assignments
3. Control lights through Home Assistant interface

## Project Image

![Nissan Skyline GTR Model](IMG_1475.jpg)