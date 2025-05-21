# 🏢 ISMBMS – Integrated Smart Monitoring and Building Management System

## 📘 Project Overview:

**ISMBMS (Integrated Smart Monitoring and Building Management System)** is a complete IoT-based solution designed for real-time monitoring and automation of building environments. It combines various sensors and actuators to create a smart infrastructure that enhances safety, energy efficiency, and intelligent control.

This system uses the **ESP32 microcontroller**, various environmental sensors, output modules, and a display to perform integrated monitoring and management tasks.

---

## 🔧 Features:

- 🌡️ **Temperature and Humidity Monitoring** using the DHT22 sensor.
- 🚶 **Motion Detection** with a PIR sensor for intruder alert.
- 🔊 **Buzzer and LED Alerts** based on motion detection.
- 💡 **Light Intensity Detection** using an LDR and control of lighting via relays.
- 🔩 **Vibration Monitoring** for safety alert using analog sensor.
- 🔁 **Servo Motor Control** to simulate physical movement in response to vibration.
- 🖥️ **OLED Display** for local sensor data visualization.
- 🔌 **Dual Relay Control** for devices like fans and lights.
- 🌍 **GPS Mock Support** (optional for simulations; can be activated using NMEA strings).

---

## 🧰 Components Used:

| Component             | Description                                  |
|----------------------|----------------------------------------------|
| ESP32                | Main microcontroller unit                    |
| DHT22                | Temperature and Humidity sensor              |
| PIR Sensor           | Motion detection                             |
| Buzzer + LED         | Alerts                                       |
| LDR Module           | Light sensor with AO pin                     |
| Vibration Sensor     | Analog vibration detection                   |
| Servo Motor          | For automation response                      |
| 2-Channel Relay      | Fan and light control                        |
| OLED SSD1306         | 128x64 I2C display                           |
| GPS Module (Mock)    | Optional for location tracking               |

---

## 🔌 Circuit Connections:

| Module           | ESP32 GPIO Pin |
|------------------|----------------|
| DHT22            | GPIO 4         |
| PIR              | GPIO 5         |
| LED              | GPIO 2         |
| Buzzer           | GPIO 19        |
| LDR (AO)         | GPIO 35        |
| Vibration Sensor | GPIO 34        |
| Relay 1          | GPIO 18        |
| Relay 2          | GPIO 25        |
| Servo Motor      | GPIO 23        |
| OLED SDA         | GPIO 21        |
| OLED SCL         | GPIO 22        |
| GPS TX (Mock)    | GPIO 17        |
| GPS RX (Mock)    | GPIO 16        |

> 🔎 **Note:** In Wokwi, the GPS module is simulated using fake NMEA data. For real hardware, connect a Neo-6M GPS module via UART.

---

## 📷 Wokwi Simulation:

You can simulate the entire setup using [Wokwi IoT Simulator](https://wokwi.com/). The diagram includes:

- All sensors and actuators
- OLED display
- Mock GPS module (optional)
- Real-time sensor reading simulation

---

## 📂 File Structure:

📁 ISMBMS/
├── README.md
├── diagram.json # Wokwi circuit diagram
├── ISMBMS.ino # Main Arduino code
├── images/ # Screenshots or diagrams
└── LICENSE

---

## ▶️ How to Use:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ISMBMS.git
Open ISMBMS.ino in Arduino IDE.

Install required libraries:

Adafruit_SSD1306

DHT sensor library

Adafruit GFX

Servo

Upload to ESP32 or run on Wokwi.

📜 License:
This project is licensed under the MIT License.

👨‍💻 Author:
Developed by [SUBHIKSHA S] – for smart infrastructure automation and IoT learning.

🌐 Acknowledgments:
Wokwi

Adafruit Libraries

Arduino Project Hub
