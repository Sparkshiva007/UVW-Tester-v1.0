# 🔧 UVW Tester – Custom PCB Design (ATmega8A Based)

A custom-designed **UVW Phase Tester** built from scratch using:

- ATmega8A microcontroller  
- TP4057 Li-ion charging  
- DW01A + FDG1024NZ battery protection  
- MT3608 boost converter (3.7V → 5V)  
- CH340G USB-to-UART for programming  
- 3-position mode selector (OFF / ON / PROGRAM)  
- 16×2 LCD interface  
- UVW indicator LEDs and test button  

Designed and routed entirely in **KiCad 7/8**.

---

## 🚀 Project Overview

This project is a compact, battery-powered **UVW phase testing tool** implemented as a single integrated PCB. It includes:

- Safe Li-ion charging and protection  
- Boosted 5V power delivery  
- USB-based programming  
- Microcontroller logic and UI  
- Button and LED-driven test interface  

This project was built to explore full-cycle embedded product development — from schematic design and power electronics to PCB layout and interfacing.

---

## 🧩 System Architecture

### 🔋 Power System
- TP4057 for Li-ion charging  
- DW01A + FDG1024NZ for battery protection  
- MT3608 boost converter for regulated 5V output  

### 🔀 Power Mode Selector
Three modes via a DPDT slide switch:
- **OFF** – complete shutdown  
- **ON** – powered by boosted battery output  
- **PROGRAM** – USB-powered mode with CH340G active and battery isolated  

### 💾 Programming Interface
- CH340G USB-UART  
- Auto-reset: DTR → capacitor → RESET  
- Standard TX/RX bootloading via USB-C  

### 🖥️ User Interface
- 16×2 LCD in 4-bit mode  
- Test button  
- UVW indicator LEDs  
- Charging/standby status LEDs  

---

## 📐 PCB Design

Created entirely in **KiCad**, with emphasis on:

- Clean functional block separation  
- Proper decoupling and grounding  
- Logical component placement  
- Clear silkscreen labels  
- LCD mounting hole alignment  
- Safe routing for power paths  


---

## 🛠️ Component Summary

| Block | Components |
|-------|------------|
| Charging | TP4057 + LEDs |
| Battery Protection | DW01A + FDG1024NZ |
| Boost Converter | MT3608 + inductor + diode + feedback resistors |
| Microcontroller | ATmega8A + crystal + decoupling |
| Programming | CH340G + USB-C |
| User Interface | 16×2 LCD + test button + UVW LEDs |
| Mode Switching | DPDT 3-position selector |

---

## 🧪 Features

- Compact standalone UVW tester  
- Rechargeable Li-ion battery power  
- USB-programmable via CH340G  
- LCD menu and display  
- Safe battery handling and boosting  
- Single-board integrated solution  

---

## 💡 Future Improvements

- Enclosure design (3D printed case)  
- Enhanced ground optimization  
- Optional buzzer feedback  
- Battery percentage sensing via ADC  
- UVW input sensing (advanced version)  

---

## 📄 License

This project is shared under the **MIT License**.  
You’re free to use, modify, or build upon it.  
If this work helps you, a small acknowledgment to **Shiva Projects** and this repository is always appreciated.

---

## 📬 Contact

**Shivashankar P**  
https://in.linkedin.com/in/shiva-shankar-p-66868b329
