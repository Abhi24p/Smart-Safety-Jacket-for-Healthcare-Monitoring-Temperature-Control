# Smart-Safety-Jacket-for-Healthcare-Monitoring-Temperature-Control

An IoT-based wearable system built using ESP32 to monitor vital body parameters and environmental conditions in real time.
The jacket integrates multiple sensors to measure body temperature, heart rate, SpO₂, gas levels, and atmospheric pressure, while offering automatic temperature regulation and emergency alert features using GSM + GPS.

🚀 Features

Body Temperature Monitoring using DS18B20
Heart Rate & SpO₂ Measurement using MAX30102 sensor
Gas Detection (CO₂, NH₃, NOx) via MQ135
Environmental Pressure using BMP180
GPS Tracking with NEO-6M
GSM SMS Alerts through SIM800L
Automatic Temperature Control using Relay-driven Peltier module
16×2 LCD Display (I²C) for live data
SOS Emergency Button
Buzzer Alert System
Continuous monitoring with real-time notifications

🧰 Hardware Components

| Component              | Description                     |
| ---------------------- | ------------------------------- |
| **ESP32 DevKit V1**    | Main microcontroller            |
| **DS18B20**            | Body temperature sensor         |
| **MAX30102**           | Pulse rate & SpO₂ sensor        |
| **MQ135**              | Gas detection sensor            |
| **BMP180**             | Pressure & temperature sensor   |
| **NEO-6M GPS**         | Location tracking               |
| **SIM800L GSM Module** | Sends emergency SMS alerts      |
| **Relay Module**       | Controls Peltier / heating unit |
| **Peltier Plate**      | Temperature regulation          |
| **I²C LCD 16×2**       | Displays live readings          |
| **SOS Button**         | Manual emergency alert          |
| **Buzzer**             | Audible alarm                   |

🛠️ Installation & Setup

Install Arduino IDE
Install ESP32 board support from:
Install required libraries from Arduino Library Manager
Select:
Tools → Board → ESP32 Dev Module
Connect ESP32 via USB and upload the code
Power GSM module separately
Assemble sensors on jacket or test bench

🧪 How It Works

Sensors capture vital and environmental data
ESP32 reads sensor data via I²C, ADC, UART, and OneWire
LCD shows live monitoring values
GPS provides location coordinate
GSM sends SMS alerts if:
Temperature is abnormal
SpO₂ or heart rate is risky
Gas value exceeds safe limit
SOS button is pressed
Relay controls a Peltier module to regulate body temperature

EMERGENCY ALERT!
Temp: 39.2°C
Heart Rate: 120 bpm
SpO2: 88%
Gas Value: HIGH
Location: 17.4123, 78.4312

🧠 Future Improvements

Mobile app for real-time data
Wi-Fi cloud integration (Blynk/Thingspeak)
Rechargeable battery with solar option
Jacket design with flexible PCB
Fall detection using accelerometer
