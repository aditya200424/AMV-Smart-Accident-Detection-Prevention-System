🚗 AMV – Smart Accident Detection & Prevention System (Blackbox AI) 
📌 Overview

AMV (Advanced Mobility Vision) is a Smart Accident Detection & Prevention System designed to act as a vehicle blackbox with AI intelligence.
The system continuously monitors driver behavior, vehicle motion, audio-visual data, and location to prevent accidents, detect collisions, and automatically trigger emergency alerts.

This project integrates Artificial Intelligence, Embedded Systems, IoT, and Computer Vision to enhance road safety and post-accident accountability.

📅 Project Duration: March 2025
🧠 Category: AI + IoT + Embedded Systems
📜 Status: Working Prototype | Patent Filed

🎯 Problem Statement

Road accidents caused by drunk driving, driver drowsiness, and delayed emergency response lead to severe injuries and fatalities.
Traditional vehicle safety systems:

Do not monitor driver behavior intelligently

Lack blackbox-style data logging

Fail to provide real-time alerts and accountability

✅ Solution

AMV solves these problems by:

Using AI-based vision to detect drowsy or drunk driving

Detecting accidents using motion sensors

Recording video, audio, and sensor data continuously

Sending real-time GPS-based alerts to emergency contacts

Acting as a vehicle blackbox for post-accident analysis

⭐ Key Features

😴 Drowsiness Detection using AI (eye closure & head pose)

🍺 Drunk Driving Detection using MQ-3 alcohol sensor

💥 Accident Detection via MPU6050 (sudden impact / tilt)

📍 Real-Time GPS Tracking (NEO-6M)

📲 Automatic SMS / Call Alerts using SIM800L

📹 Multi-Camera Recording (x3) – driver, road, cabin

🎙 Audio Recording using MEMS microphone

💾 Blackbox Storage on MicroSD card

🔒 Evidence Preservation for insurance & legal use

🧩 System Architecture

The system is built around an ESP32 SoC acting as the main controller and data coordinator.

Main Modules:

ESP32 SoC (central controller)

ESP32-CAM (AI vision input)

MPU6050 (motion & accident detection)

MQ-3 (alcohol detection)

GPS NEO-6M (location tracking)

SIM800L (GSM communication)

MEMS Microphone (audio)

MicroSD Card (blackbox storage)

📷 Architecture diagram is available in /hardware/circuit-diagram/
🛠 Hardware Components
| Component       | Description                         |
| --------------- | ----------------------------------- |
| ESP32           | Main microcontroller                |
| ESP32-CAM (x3)  | Driver face, road, cabin monitoring |
| MPU6050         | Accelerometer + gyroscope           |
| MQ-3            | Alcohol detection sensor            |
| GPS NEO-6M      | Location tracking                   |
| SIM800L         | GSM SMS/call alerts                 |
| MEMS Microphone | Audio capture                       |
| MicroSD Module  | Data logging                        |
| Power Supply    | Battery / vehicle power             |

💻 Software & Technologies
🔹 Embedded Systems

Arduino IDE / ESP-IDF

UART, I2C, SPI protocols

GSM AT commands

🔹 Artificial Intelligence

Python

OpenCV

TensorFlow / TensorFlow Lite

CNN-based driver monitoring

🔹 Computer Vision

Face detection

Eye aspect ratio analysis

Head pose estimation

🔹 Data Storage

CSV / binary logs on MicroSD

Timestamped sensor records

🧠 AI Model Description

The AI model processes real-time camera input to:

Detect eyes closed beyond threshold

Identify abnormal head movement

Trigger alerts when drowsiness is detected

Pipeline:

Camera input (ESP32-CAM)

Frame preprocessing

Feature extraction

CNN inference

Alert generation

🚨 Working Logic (Simplified)

System powers ON

Sensors & cameras initialize

Continuous monitoring starts

If:

Alcohol detected → Alert

Drowsiness detected → Alert

Sudden impact detected → Emergency mode

GPS coordinates fetched

SMS sent to emergency contacts

Data stored on SD card

🚀 Applications

Smart vehicles

Fleet monitoring systems

Insurance claim verification

Accident investigation

Emergency response systems

🔮 Future Enhancements

Cloud dashboard & mobile app

LTE / 5G connectivity

Driver identity recognition

Vehicle-to-vehicle (V2V) alerts

Automotive-grade PCB

Contributions

Contributions, suggestions, and improvements are welcome.
