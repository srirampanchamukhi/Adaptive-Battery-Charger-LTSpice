# 🔋 Adaptive Battery Charging Circuit — LTSpice Simulation

**🏆 2nd Prize Winner — ElectroQuad'25 Hackathon**  
Team PV | February 2025

This project simulates an **adaptive battery charging circuit** designed to charge a 12V battery while dynamically adjusting the charging current based on load conditions. It includes safety mechanisms and ripple suppression, designed under strict component and time constraints.

---

## 🎯 Problem Statement

As part of the ElectroQuad'25 Hackathon, the challenge was to design and simulate a battery charging circuit that:

1. Maintains a **constant 12V charging voltage**
2. Dynamically adjusts current based on battery state (0.5A to 2A)
3. Includes **overvoltage, overcurrent, and thermal protection**
4. Limits ripple to **<100mV peak-to-peak** ✅ *(Achieved)*

📄 [View Full Problem Statement](docs/ElectroQuad_Problem_Statement.pdf)

---

## ⚙️ What I Built

- Designed and simulated in **LTSpice**
- Implemented a **MOSFET-based Buck-Boost Converter** for dynamic voltage regulation
- Implemented current control and ripple suppression
- Built under a 3-hour time limit using only permitted components

Despite constraints, the design met the **ripple requirement**, although the output voltage remained below 12V due to circuit limitations.

---

## 🧩 System Overview

| Component          | Purpose                                         |
|--------------------|-------------------------------------------------|
| Linear Regulator   | For maintaining a constant voltage (target: 12V)|
| BJT + R-C Network  | Used for current control and soft switching     |
| Filters            | Capacitors for ripple smoothing                 |
| Safety Mechanisms  | Passive thermal and current protection logic    |
| Buck-Boost Converter | Main voltage regulation block using switching MOSFET topology |

---

## 🧪 Simulation Results

- ⚡ Ripple under 100mV ✅
- ❌ Output voltage: Microvolt level (target was 12V)

![Simulation Waveform](results/Simulation%20Waveform.png)  
![Circuit Diagram](results/Circuit%20Diagram.png)

---

## 📁 Files

| File                                | Description                                      |
|-------------------------------------|--------------------------------------------------|
| [`Team PV Circuit.asc`](circuit/Team%20PV%20Circuit.asc)        | LTSpice schematic file                           |
| [`Simulation Waveform.png`](results/Simulation%20Waveform.png)  | Screenshot of simulation output                  |
| [`Circuit Diagram.png`](results/Circuit%20Diagram.png)          | Full circuit layout (image)                      |
| [`Team PV Report.docx`](docs/Team%20PV%20Report.docx)           | Project explanation and design choices           |
| [`ElectroQuad_Problem_Statement.pdf`](docs/ElectroQuad_Problem_Statement.pdf) | Original problem statement                      |
| [`Runner-up Certificate.png`](docs/Runner-up%20Certificate.png) | 2nd prize certificate 🏆                         |

---

## 🏆 Award

🥈 **2nd Prize Winner** out of 150 teams across 4 NITs (Trichy, Calicut, Surathkal, Warangal)  
ElectroQuad'25 — National Inter-NIT Hardware Hackathon

I participated as a solo team (**Team PV**) and secured the runner-up position among highly competitive multidisciplinary teams.

![Runner-up Certificate](docs/Runner-up%20Certificate.png)

---

> *This project reflects real-world design constraints and engineering trade-offs — built entirely under pressure in a 3-hour competitive hackathon setting.*
