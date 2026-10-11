# IoT-Based-Water-Pipeline-Leakage-Monitoring-System
An ESP32-based IoT water pipeline leakage monitoring system using flow sensors and relay control, with Blynk IoT and Node-RED dashboards, MQTT communication, and Telegram and email notifications.
IoT-Based Water Pipeline Leakage Monitoring System

Project Overview

This project is an IoT-based water pipeline leakage monitoring system developed using an ESP32, two flow sensors, and a water pump.

The system compares the inlet and outlet flow rates to identify possible water leakage. When the flow difference exceeds a predefined threshold for three consecutive measurement intervals, the system detects a potential leak, switches off the pump, activates a buzzer, and sends a Telegram notification through Node-RED.

Objectives

- Monitor inlet and outlet water flow rates.
- Calculate the difference between the two flow measurements.
- Detect possible pipeline leakage.
- Automatically switch off the pump when leakage is detected.
- Display sensor readings and system status on a Node-RED dashboard.
- Send Telegram notifications when a leak is detected.
- Allow the user to reset the system after addressing the leakage.

Components Used

- ESP32 Dev Module
- Two water flow sensors
- Relay module
- Water pump
- Buzzer
- Wi-Fi connection
- HiveMQ public MQTT broker
- Node-RED dashboard
- Telegram bot

Technologies Used

- Embedded C++ / Arduino IDE
- MQTT communication
- Node-RED
- Telegram Bot API
- IoT-based monitoring

Working Principle

1. Flow Sensor 1 measures the inlet water flow.
2. Flow Sensor 2 measures the outlet water flow.
3. The ESP32 calculates the difference between the two flow rates.
4. If the difference exceeds the configured threshold for three consecutive measurement intervals, the system declares a potential leakage.
5. The ESP32 switches off the pump and activates the buzzer.
6. The leakage status and pump status are published through MQTT.
7. Node-RED displays the readings and sends a Telegram notification.
8. After the leakage has been addressed, the user can reset the system through the dashboard.

System Features

- Real-time flow monitoring
- Automatic leakage detection
- Automatic pump shutdown
- Buzzer-based warning
- MQTT communication
- Node-RED dashboard
- Telegram notifications
- User-controlled system reset

Project Demonstration

Project photographs, source code, dashboard screenshots, and the demonstration video link will be provided in this repository.

Team Members

- Sudhishma S.
- Meera Sankar S

Future Improvements

- Improve flow sensor calibration and leakage detection accuracy.
- Add historical flow data and graphical analysis.
- Introduce secure MQTT communication and authentication.
- Improve dashboard visualization and system diagnostics.
