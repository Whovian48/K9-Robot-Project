# K9 Robot Dog Build

![K9 Robot Image](link-to-your-image)

## Overview
This repository contains the 2024 version of the **K9 Robot Dog Software**, updated for Raspberry Pi 5 with improved capabilities in speech recognition, navigation, and 3D vision.

The K9 robot features:
- Real-time speech interactions with GPT-3/3.5 and offline fallback.
- LIDAR-based navigation and collision avoidance.
- OAK-D stereo camera for 3D vision and object detection.
- Chess-playing functionality via Lichess API.

## Core Features
- **Speech Recognition:** Offline STT with Mozilla DeepSpeech or Coqui STT, and online GPT-powered interactions.
- **Navigation:** Redis and MQTT used for state sharing and pub/sub communication between modules.
- **Vision Pipeline:** OAK-D Lite for real-time object detection, depth sensing, and collision avoidance.
- **Modular Design:** Key modules include motors, lights, ears, and memory, each running independently but integrated through Redis/MQTT.

## Hardware Requirements
- Raspberry Pi 5 (2GB or more recommended)
- Adafruit I2C PCA9685 Servo controller
- Espruino Pico for LIDAR ears
- USB microphone
- RoboClaw PID motor controller
- OAK-D camera

## Software Requirements
- Python 3.10+
- Redis for shared memory
- MQTT for pub/sub communication
- DepthAI SDK for OAK-D integration

## Installation

### Prerequisites
1. Install system dependencies:
   ```bash
   

