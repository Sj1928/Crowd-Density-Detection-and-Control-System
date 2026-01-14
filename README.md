# Crowd-Density-Detection-and-Control-System
An IoT + Computer Vision based smart safety system that detects crowd density in real-time using a Raspberry Pi camera feed, performs head/person detection, and automatically triggers alerts + gate control actions when the crowd exceeds a configured threshold.

This helps prevent overcrowding, congestion, and stampede-like situations by enabling an automated response instead of manual monitoring.
#📌 Problem Statement
Traditional surveillance systems face major limitations:
- Manual monitoring is not scalable for large crowds.
- No automatic alert mechanism exists when crowd thresholds are crossed.
- Authorities often react late because action depends on human observation.

# 🎯 Objective
To build a low-cost automated crowd alert & control system using:
- Raspberry Pi + Pi Camera for live monitoring
- ML-based head/person detection
- Threshold-based alerts
- Automatic activation of safety mechanisms:
- Emergency gate opening
- Red LED warning
- Buzzer alarm

# 🧠 System Overview (Workflow)
- Pi Camera captures live crowd video.
- Raspberry Pi Zero 2 W streams video to a client laptop (server-client architecture).
- Client runs ML/OpenCV detection frame-by-frame and counts persons/heads.
- Count is compared with a predefined crowd threshold.
- If threshold exceeded:
- Alert is sent to Raspberry Pi
- Raspberry Pi signals ESP8266
- ESP8266 triggers:
- Emergency exit gate (servo motor)
- Red LED
- Buzzer alarm

# 👨‍💻 Authors
- Sibshish Bhoi
- Department: Electronics & Instrumentation
- Project: Final Year IoT + CV based Smart Surveillance
Red LED

Buzzer alarm
