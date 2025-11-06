# 🚁 Arduino-Dual-Drone Project

> **A lightweight two-motor drone system with Bluetooth control via HC-05. Modular, expandable, and student-built with love 💖.**

---

## 📖 Overview

This project is a micro drone built on **Arduino Uno** featuring:
- **2 Brushless Motors + ESCs**
- **HC-05 Bluetooth module** for remote control via custom Android app
- Modular software structure using **PlatformIO** and C++

---

## 🎯 Features

- 🛠️ **Manual control via Bluetooth (WASD control scheme)**
- ✨ **Clean modular code split into multiple `.cpp` and `.h` files**
- 📡 **HC-05 Bluetooth receiver with dedicated communication module**
- 🔄 **ESC control using Servo library (PWM-based)**
- ⚙️ **Custom speed and threshold configuration**

---

## 🧩 Folder Structure

```bash
Arduino-Dual-Drone/
├── include
│   ├── comm.h
│   └── drone.h
├── lib
├── platformio.ini
├── src
│   ├── comm.cpp
│   ├── drone.cpp
│   └── main.cpp
└── test
```

---

## 🔧 Hardware Structure

**Components:**
- Arduino Uno (CH340)
- 2x A2212 1000KV Brushless Motor
- 2x 30A ESC with BEC
- 2x Pairs of 1045L/R Propellers for brushless motors (CW & CCW)
- HC-05 Bluetooth Module
- Li-Po 7.4V 1500mAh 2S Battery (You can upgrade to Li-Po 3S (11.1V) Battery
- Jumper Cables
- Custom Impraboard Frame
  
---

## ⚡ Wiring Layout

| Component              | Arduino Pin | Note                                             |
| :--------------------- | :---------- | :----------------------------------------------- |
| Motor Left ESC Signal  | D6          | Controlled via Servo PWM                         |
| Motor Right ESC Signal | D5          | Controlled via Servo PWM                         |
| HC-05 TX               | RX (D0)     | Bluetooth serial receive                         |
| HC-05 RX               | TX (D1)     | Bluetooth serial transmit                        |
| Li-Po Battery          | ESC T-plug  | ESC powers motors and BEC provides 5V to Arduino |

⚠️ Note:
- Motors connected directly to ESCs
- ESC’s BEC powers Arduino via 5V and GND
- Ensure to calibrate ESC before first flight

📊 Optional ASCII/Diagram:
```
[HC-05]
   |
 TX/RX
   |            
  [Arduino UNO CH340]
    |       |       |
  D6 ESC  D5 ESC    5V/GND (from ESC BEC)
    |       |
  Motor1  Motor2
```

---
## ⚙️ Dependencies

- Servo (by Arduino)

---

## 👨‍💻 Contributors
| Name                   | Role                                   |
| :--------------------- | :------------------------------------- |
| Bernardus (me 😎)      | Project Lead / Programmer / Repo Owner |
| Hugo | Hardware Builder / Hardware Wiring |
| Isaac | Hardware Builder / Hardware Wiring |
| Matthew | Donor |
| Austin | Donor |
| Mr. Tito Vicente Maia, S.T. | Teacher and Main Advisor |

---

## 📈 Goals
- Build a polished, working student drone
- Learn modular embedded system programming
- Leave behind a clean, reusable codebase for future students
- Earn big teacher respect points 😤

---

## 📸 Demo (To be added after testing)

> Documentation photos, test footage, and performance stats coming soon.

---
## 📔 Summary
> We failed at making a flying drone due to insufficient funding and lack of research; however, from this failed project, we gained a lot of experience dealing with hardware, embedded quirks, and integration with Bluetooth software.

> TLDR: We failed but gained so much experience 🐧✨
---

## 🚀 Big Projects Start Small

*Remember ! Big Projects Start From Small Dreams ! ✨🌠"*


