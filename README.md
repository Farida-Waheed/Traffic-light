# 🚦 Traffic Light System Project

A simple yet effective electronic simulation of a **traffic light control system** using a 555 Timer IC and a 4017 Decade Counter. This project was developed as part of the Electronics Lab at Benha University, Faculty of Engineering (Shoubra), Communications and Computer Engineering Department.

---

## 📘 Introduction

Traffic lights manage vehicle flow at intersections and enhance safety. This project implements a **sequenced traffic light system** that mimics real-world stop, caution, and go signals using LEDs. It showcases how the **555 timer** and **4017 decade counter** ICs work together to control timing and LED sequencing.

---

## 🏫 Project Information

- **University:** Benha University, Faculty of Engineering (Shoubra)
- **Department:** Communications and Computer Engineering
- **Course:** Electronic Circuits 2

---

## 👩‍💻 Team Members

- Farida Waheed Abdelbary
- Mohamed Ahmed Mohamed Hassan
- Raneem Ahmed Refaat
                 
---

## 📘 Project Overview

This project models a basic yet practical traffic light system that controls signal transitions using simple integrated circuits. It is designed to:
- Emulate **Stop**, **Caution**, and **Go** signals.
- Use **555 Timer IC** for generating clock pulses.
- Use **4017 Decade Counter IC** for sequencing LED lights.

---

## 🧠 Theory of Operation

### 🔁 IC 555 (Timer)
- **Pin 3 (Output)**: Generates clock signals for 4017.
- **Pins 2 & 6**: Connected to a capacitor to determine pulse duration.
- **Pin 7**: Controls charge/discharge rate via a potentiometer.
- **Pins 4 & 8**: Connected to Vcc for power.
- **Pin 4**: Reset (disabled by keeping high).
- **Pin 5**: Not used.

### 🔟 IC 4017 (Decade Counter)
- **Pin 14 (CLK)**: Receives clock pulses from the 555.
- **Pins Q0–Q9**: Sequentially go high on each rising clock edge.
- **Pin 15 (Reset)**: Grounded to allow continuous counting.
- **Pin 13 (Enable)**: Typically grounded.

---

## 🔦 LED & Diode Configuration

| Output Pin | LEDs | Duration | Meaning               |
|------------|------|----------|------------------------|
| Q0–Q3      | Red  | 4 cycles | 🚫 Stop                |
| Q4         | Red + Yellow | 1 cycle  | 🛑 Stop + Caution     |
| Q5–Q8      | Green| 4 cycles | ✅ Go                  |
| Q9         | Yellow | 1 cycle  | ⚠️ Caution            |

**Diodes** are used for:
- Isolation between outputs
- Voltage protection
- Current limiting
- Directing current properly to LEDs

---

## 🛠 Components Used

- **555 Timer IC**
- **4017 Decade Counter IC**
- **Red, Yellow, Green LEDs**
- **Diodes**
- **Capacitors & Potentiometers**
- **Power Supply (5–15V)**

---

## 💻 Implementation

### ✅ Simulation:
Designed and tested using **Proteus** simulation software.

### 🔧 Breadboard:
The design was successfully built and tested on a breadboard.

### 📦 PCB:
Final circuit was fabricated and soldered on a PCB for real-life testing.

---

## 📷 Project Stages

- **Schematic Design (Proteus)**:
  ![image](https://github.com/user-attachments/assets/2dd4dabd-21e6-440a-b082-59b1fdd58c57)
- **Breadboard Implementation**:
  ![image](https://github.com/user-attachments/assets/d940fea6-4a73-4b34-97d4-5c8458f205c7)
- **Final PCB Product**:
  ![image](https://github.com/user-attachments/assets/669eea0f-a52f-4850-92d3-436d055f1b53)
  ![image](https://github.com/user-attachments/assets/ce986d88-4ca6-4974-b25e-2cbcc72a2247)




