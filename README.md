# Motogadget Clone (ESP32)

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Platform: ESP32](https://img.shields.io/badge/Platform-ESP32-blue.svg)
![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)

**A fully open-source motorcycle control unit (inspired by Motogadget M-Unit Blue), powered by ESP32.**  
Complete with PCB schematics, 3D models, BOM + Pick & Place, and firmware examples.

---

## 📚 Overview

This project develops an open-source alternative to the **Motogadget M-Unit Blue**, intended for **custom motorcycles and DIY builders**.  

- Handles **all electrical functions** (lights, horn, ignition enable, indicators).  
- Adds **overcurrent/short-circuit protection** strategies.  
- Firmware-driven logic: configurable behavior (auto-cancel indicators, delayed lights, etc.).  
- **ESP32 MCU** enables advanced features (future: Bluetooth app config, CAN bus).  

> ⚠️ Project is in **prototype/experimental** stage. Hardware and firmware are subject to change.

---

## 🛠️ Hardware Details

- **MCU**: ESP32  
- **Power**: fused battery input, protection circuitry, buck regulator  
- **Inputs**: switch/button signals (momentary or latching)  
- **Outputs**: relay or solid-state drivers for lighting + auxiliary loads  
- **Form factor**: compact PCB for mounting under seat/tank  
- **Design priorities**: vibration resistance, easy wiring, serviceability  

📄 **Schematics:**  
[Schematic PDF](./Schematics/Schematic_Canarin_MUX.pdf)  

📦 **3D Model Previews:**  
*(add your `.step` or screenshot images here, e.g. from EasyEDA export)*  

🖼 **PCB Images:**  
*(insert renders or Gerber previews from `/PCB` folder)*  

---

## 📦 Bill of Materials (BOM)

A detailed **BOM + Pick & Place** file is provided in:  
[`/BOM and Pick N Place`](./BOM%20and%20Pick%20N%20Place)  

Key components include:

| Component      | Description                  | Notes                  |
|----------------|------------------------------|------------------------|
| MCU            | ESP32-WROOM Module           | Main controller        |
| Relays/MOSFETs | Automotive-rated drivers     | Output switching       |
| Regulator      | DC-DC buck                   | Stable 3.3V for MCU    |
| Connectors     | Screw terminal / JST options | For I/O wiring         |
| Protection     | Fuse, TVS diode              | Short-circuit safety   |

---

## 📐 PCB Fabrication

All Gerber files are included under [`/PCB`](./PCB).  
Boards are currently being fabricated and tested with the support of **PCBWay**.  

**Manufacturing Sponsor:**  
Huge thanks to **PCBWay** for sponsoring the first prototype batch. Their **high-quality manufacturing, quick turnaround, and helpful service** accelerate development.  

> A full review of PCB quality, assembly, and ordering experience will be published here and on Reddit once boards are tested.

---

## 🚀 Firmware

- **Platform**: Arduino IDE or PlatformIO  
- **Core logic**: input scanning, rules engine, output driving  
- **Planned features**:  
  - Configurable I/O mapping  
  - Short-circuit detection/handling  
  - Bluetooth app configuration  
  - CAN bus integration  

*(Firmware will be pushed as soon as bring-up tests are complete.)*

---

## 🧪 Testing Plan

1. **Bench Power-Up**: check voltage rails, ESP32 boot.  
2. **Input Simulation**: switch/button signals → serial monitor feedback.  
3. **Output Loads**: drive LEDs, then lamps, then full motorcycle circuits.  
4. **Protection**: simulate short-circuit with current-limited supply.  
5. **Environmental**: vibration/shock (bench test), thermal cycling.  
6. **On-Bike**: staged integration — start with indicators/horn, then expand.  

---

## 📅 Roadmap

- **Now**: PCB prototyping, firmware scaffolding.  
- **1–2 months**: Hardware bring-up, protective feature testing.  
- **3–4 months**: Firmware stability, Bluetooth integration.  
- **5–6 months**: Community-ready release with guides and demos.  

---

## 📸 Media

Add your images here once PCBs arrive:  
- PCB top/bottom photos  
- 3D renders  
- Assembly shots  
- On-bike installation  

---

## 🙌 Collaboration

Contributions welcome!  
- Build & test your own prototype.  
- File issues for bugs, improvements, ideas.  
- PRs for firmware, PCB design, docs.  
- Share builds (photos/videos).  

---

## 📜 License

This project is released under the **MIT License**.  
All files (schematics, PCB, firmware, docs) are open for personal and commercial use with attribution.

---

## 🔗 Resources

- [GitHub Repository](https://github.com/jaksatomovic/motogadget-clone)  
- [PCBWay](https://www.pcbway.com/)  
- [ESP32 Documentation](https://docs.espressif.com/)  
- [Arduino IDE](https://www.arduino.cc/en/software)  

---

> _“Open source means everyone can help — collective knowledge is stronger.”_
