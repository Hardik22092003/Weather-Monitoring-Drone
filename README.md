# 🛰️ Weather Monitoring Drone with LoRa Communication

A modular drone-based atmospheric sensing system that captures real-time environmental data from the lower atmosphere and transmits it wirelessly using LoRa communication.

---

## 🔧 Project Overview

This project aims to create an efficient and long-range **weather monitoring drone** equipped with:

- Environmental sensors (Temperature, Humidity, Pressure, CO₂)
- Custom-designed PCB for efficient integration
- LoRa transceivers for low-power, long-range data transmission
- ESP32 microcontroller for processing and communication
- Ground station for real-time telemetry display

---

## 📦 Features

✅ Real-time atmospheric data logging  
✅ Long-range wireless transmission using **LoRa SX1278**  
✅ Compact, drone-mounted custom PCB design  
✅ Multi-sensor fusion (BMP180, DHT11, MQ135)  
✅ Power-efficient firmware logic (sleep-wake cycles)  
✅ Ground receiver dashboard using Python serial interface  

---

## 🔬 Technologies & Tools Used

| Category | Tools/Components |
|---------|------------------|
| Microcontroller | ESP32 DevKit V1 |
| Communication | LoRa SX1278 Modules |
| Sensors | BMP180 (Pressure), DHT11 (Temp/Humidity), MQ135 (CO₂) |
| PCB Design | EasyEDA |
| Drone Modeling | Blender |
| Firmware | Embedded C (Arduino Framework) |
| Visualization | Python + Serial Plotting (ground station) |

---

## 🛠️ System Architecture

```
[ Sensors ] --> [ ESP32 ] --> [ LoRa TX ] ))) ---wireless---> ((( [ LoRa RX ] --> [ Python Dashboard ]
              [ Custom PCB ]                                 [ Ground Station ]
```

---

## 🚀 Getting Started

### Hardware Setup

1. **Sensor Integration**: Connect BMP180, DHT11, and MQ135 to ESP32 GPIOs (I2C + analog pins).
2. **PCB Mounting**: Use the provided `.gerber` files to fabricate and assemble the custom PCB.
3. **LoRa Module**: Connect SX1278 LoRa modules to both drone-side and ground station ESP32.

### Firmware Flashing

- Use [Arduino IDE] or PlatformIO to flash the firmware.
- Libraries Required:
  - `Adafruit_BMP085`
  - `DHT`
  - `LoRa`
  - `SoftwareSerial` (for debug, optional)

### Ground Station

- Run `receiver_plot.py` (included) to visualize sensor data in real-time.
- Requires: `pyserial`, `matplotlib`, `pandas`

---

## 📈 Sample Data Output

```
Timestamp       Temp (°C)   Humidity (%)   Pressure (hPa)   CO₂ Level (ppm)
------------------------------------------------------------------------
2025-07-16 08:30  32.5         58.0             987.2            412
2025-07-16 08:31  32.7         59.1             986.9            415
...
```

---

## 📂 Repository Structure

```
├── firmware/
│   ├── drone_firmware.ino
│   └── sensor_readings.cpp
├── hardware/
│   ├── schematic.pdf
│   ├── PCB_layout.png
│   └── gerber/
├── ground_station/
│   └── receiver_plot.py
├── README.md
└── LICENSE
```

---

## 📌 Future Improvements

- GPS-based geotagging of sensor data  
- SD card backup on drone for data redundancy  
- Altitude sensor integration for vertical profiling  
- Drone telemetry over WebSocket/MQTT

---

## 🙋 About the Developer

👤 **Hardik Sahu**  
🎓 B.Tech – Electrical Engineering | MANIT Bhopal  
🔗 [LinkedIn](https://www.linkedin.com/in/hardik-sahu-07296b24b/) | [GitHub](https://github.com/Hardik22092003)  
✉️ hardiksahu02@gmail.com

---

## 📄 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

## 🙋 About the Developer

👤 **Hardik Sahu**  
🎓 B.Tech – Electrical Engineering | MANIT Bhopal  
🔗 [LinkedIn](https://www.linkedin.com/in/hardik-sahu-07296b24b/) | [GitHub](https://github.com/Hardik22092003)  
✉️ hardiksahu02@gmail.com

---
