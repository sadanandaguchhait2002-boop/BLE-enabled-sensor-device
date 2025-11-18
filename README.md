[README_GITHUB_STYLE.md](https://github.com/user-attachments/files/23609670/README_GITHUB_STYLE.md)
# ESP32-C3 Mini Sensor Board 🚀  
A compact, low‑power BLE sensor board featuring the **ESP32‑C3‑MINI‑1**, **SHT30**, and **AMS1117‑3.3** with USB programming support.

---

## 📛 Badges  
![Status](https://img.shields.io/badge/Project-Active-brightgreen)
![Board](https://img.shields.io/badge/MCU-ESP32--C3-blue)
![Sensor](https://img.shields.io/badge/Sensor-SHT30-purple)
![License](https://img.shields.io/badge/License-Free-lightgrey)

---

## 📘 Overview  
This project is a custom PCB designed for environmental sensing and BLE communication using the **ESP32‑C3 Mini**.  
It supports:
- Temperature & humidity sensing  
- BLE 5.0 communication  
- USB‑based programming  
- 9V external power input  

---

## ✨ Features  
- 🔹 Low‑power BLE (ESP32‑C3‑MINI‑1)  
- 🔹 High‑accuracy SHT30 sensor  
- 🔹 9V → 3.3V power regulation using AMS1117  
- 🔹 Auto‑reset & boot‑mode transistors  
- 🔹 Reverse polarity protection  
- 🔹 Compact PCB with RF antenna keep‑out  
- 🔹 USB interface for easy flashing  

---

## 📦 Project Structure  
```
├── PCB1.PcbDoc               # PCB layout file
├── Sheet1.SchDoc             # Schematic file
├── BOM.xlsx                  # Bill of Materials
├── README.md                 # Project documentation
└── Reports/                  # Design briefs & power analysis
```

---

## 🔧 Components Used  
| Component | Reason |
|----------|--------|
| **ESP32‑C3‑MINI‑1** | BLE 5.0 + low power, compact size |
| **AMS1117‑3.3 LDO** | Simple, stable 3.3V regulation |
| **SHT30 Sensor** | High‑accuracy humidity & temperature |
| **Q1 & Q2 Transistors** | Auto-reset and boot mode entry |
| **DC Jack (9V)** | External power input |
| **USB Micro Port** | Programming and 5V input |
| **LED Indicators** | Status and power indication |
| **Protection Diode** | Reverse polarity safety |

---

## ⚡ Power Summary  
| Mode | Current | Notes |
|------|---------|-------|
| **Partial Mode** | ~6.9 µA | Deep sleep + 1 reading/min |
| **Continuous Mode** | ~50.6 mA | ESP32 BLE active + sensor active |

---

## 🛠 How to Use  
1. Open **SchDoc** and **PcbDoc** in **Altium Designer**  
2. Flash ESP32‑C3 via USB  
3. Power the board using 9V DC jack or USB  
4. Monitor BLE broadcasts or integrate with your application  

---

## 📚 Included Reports  
- Design Brief  
- Power Consumption Analysis  
- Runtime Estimation  
- One‑Page Summary  

---

## 📝 Notes  
- Keep the antenna area unobstructed  
- AMS1117 may heat up if heavily loaded (use copper pour)  
- Place SHT30 away from heat sources for accurate readings  

---

## 🤝 Contributing  
Feel free to fork and enhance the design! PRs welcome.  

---

## 📄 License  
This project is open for academic and personal use.

---

## ⭐ If you find this useful, give it a star on GitHub!
