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



## 🙋 About the Developer

👤 **Hardik Sahu**  
🎓 B.Tech – Electrical Engineering | MANIT Bhopal  
🔗 [LinkedIn](https://www.linkedin.com/in/hardik-sahu-07296b24b/) | [GitHub](https://github.com/Hardik22092003)  
✉️ hardiksahu02@gmail.com

---

