# Motogadget Clone

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Platform: ESP32](https://img.shields.io/badge/Platform-ESP32-blue.svg)
![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)

**DIY prototype of a Motogadget-like unit (inspired by Motogadget M-Unit Blue) using ESP32**

---

## 📖 Table of Contents

- [Project Description](#-project-description)  
- [Repository Structure](#-repository-structure)  
- [Requirements](#-requirements)  
- [Getting Started](#-getting-started)  
- [Status & Roadmap](#-status--roadmap)  
- [How to Contribute](#-how-to-contribute)  
- [License](#-license)  

---

## 🛠 Project Description

This project is my DIY prototype of a Motogadget control unit (e.g. *M-Unit Blue*).  
The goal is to provide a more affordable, open version with essential features:

- Handle inputs from switches/signals  
- Manage power and protection  
- Ready-to-build PCB and schematics  

⚠️ The project is **not finished** — currently in **experimental stage** and open for community contributions.

---

## 📂 Repository Structure

```text
├── Schematics/              ← electronic schematics  
├── PCB/                     ← PCB board files (Gerber, top/bottom view, images)  
├── BOM and Pick N Place     ← bill of materials + placement files  
├── EasyEDA Source Files     ← EasyEDA project sources  
├── How to Order.txt         ← instructions for PCB ordering  
├── License                  ← project license (MIT)  
└── … other docs and resources  
```

---

## ⚡ Requirements

- ESP32 microcontroller  
- Components from the BOM  
- Soldering tools / prototyping equipment  
- Software: Arduino IDE or PlatformIO, EasyEDA (for PCB design)  
- Stable power supply (with protection recommended)  

---

## 🚀 Getting Started

1. Clone the repository:  
   ```bash
   git clone https://github.com/jaksatomovic/motogadget-clone.git
   ```
2. Review the schematics and PCB files.  
3. Assemble or order the PCB using the Gerber files.  
4. Solder and connect components according to the BOM.  
5. Upload firmware / test code to the ESP32.  
6. Verify basic functionality (switches, LEDs, power protection).  

---

## 📌 Status & Roadmap

**Current status:**  
- PCB design drafted, basic schematics available  
- Firmware in early stage  
- Used mainly as **prototype / proof of concept**

**Planned improvements:**  
- Develop stable firmware with configuration support  
- Test robustness under real-world conditions (vibration, temperature, moisture)  
- Add protective features (current limits, fuses)  
- Explore CAN communication and additional modules  

---

## 🤝 How to Contribute

The community is welcome to participate! You can:  
- Try out the project and build your own prototype  
- Report bugs or ideas via *Issues*  
- Submit *Pull Requests* for firmware, PCB, or documentation improvements  
- Share photos/videos of your prototype  

If you create improvements (e.g. a better PCB version), I’d be glad to merge them into the repo.  

---

## 📜 License

This project is released under the **MIT License**.  
See the [`LICENSE`](LICENSE) file for details.  

---

> _“Open source means everyone can help — collective knowledge is stronger.”_  
