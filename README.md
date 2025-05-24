# Smart-Alcohol-Dispenser-IoT
A smart IoT-based alcohol dispensing system designed for bars and restaurants. It automatically measures poured volumes, updates inventory in real time, and alerts staff when bottles are low — reducing waste and improving efficiency.

Features

- Accurate alcohol dispensing using load cells
- Real-time inventory updates to the cloud
- WiFi and BLE support (ESP32)
- Tamper detection and usage logging
- Cloud alerts for low stock levels
- Compact PCB design for easy installation

Tech Stack

- Microcontroller: ESP32
- Languages: C, C++, Python (for testing/logging)
- RTOS: FreeRTOS
- Communication:UART, I2C, MQTT
- Cloud: Firebase / AWS IoT
- PCB Tools: KiCad / Eagle
- Debug Tools: Oscilloscope, Logic Analyzer

---

 Architecture

1. Load Cell + HX711 → ESP32
2. ESP32 (FreeRTOS tasks):
   - Task 1: Read sensor
   - Task 2: Control solenoid
   - Task 3: Send data via MQTT
3. MQTT → Firebase dashboard

