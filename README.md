# 📡 5GHz Microstrip Patch Antenna Design

[![CST Studio Suite](https://img.shields.io/badge/Tools-CST_Studio_Suite-blue?style=flat-square&logo=dasher)](https://www.3ds.com/products-services/simulia/products/cst-studio-suite/)
[![Field](https://img.shields.io/badge/Field-RF_%26_Antennas-orange?style=flat-square)](https://en.wikipedia.org/wiki/Microstrip_antenna)

An optimized design and simulation of a **Microstrip Patch Antenna** operating at the **5 GHz** frequency band. This project focuses on achieving high return loss and efficient radiation through precise impedance matching using the **Inset Feed** technique.

---

## 🎯 Project Overview
This project was developed as part of the **Electronics and Communication Engineering (ECE)** curriculum. The goal was to design a Microstrip patch antenna, targeting a resonant frequency of 5 GHz with a characteristic impedance of 50 $\Omega$.

### ✨ Key Features
* **Impedance Matching:** Implemented an **Inset Feed** to reach the 50 $\Omega$ point on the patch, eliminating the need for external matching circuits.
* **High Performance:** Achieved a Return Loss ($S_{11}$) of **-22.4 dB**, indicating minimal power reflection.
* **Parametric Modeling:** The design is fully parameterized, allowing for easy frequency tuning and optimization.

---

## 📊 Technical Specifications

| Parameter | Value | Description |
| :--- | :--- | :--- |
| **Center Frequency** | 5 GHz | Target Resonant Frequency |
| **Return Loss ($S_{11}$)** | -22.4 dB | Magnitude at 4.97 GHz |
| **Gain** | 7.012 dBi | Peak Directivity |
| **Substrate** | FR-4 (lossy) | $\epsilon_r = 4.3$, $h = 1.6$ mm |
| **Efficiency** | ~44% | Radiation Efficiency (Rad. Effic.) |
| **Feeding Method** | Inset Feed | Optimized for 50 $\Omega$ SMA Connector |

---

## 📐 Dimensions & Parameters
The following parameters were used in the CST model to achieve the results:

* **L (Length):** 13.9 mm
* **W (Width):** 18.4 mm
* **W_f (Feed Width):** 3.0 mm
* **Fi (Inset Depth):** 4.0 mm
* **G (Gap):** 1.0 mm

---

## 📈 Simulation Results

### 1. S-Parameters ($S_{11}$)
The simulation shows a sharp resonance at **4.97 GHz**, which is within <1% error of the design target.
> *Refer to the `S-Parameters` plot in the Results folder.*

### 2. Radiation Pattern
The antenna exhibits a clear **Broadside Radiation Pattern**, typical for patch antennas, with maximum directivity along the Z-axis.

---

## 💻 How to Run
1.  Clone this repository:
    ```bash
    git clone [https://github.com/Ommmarr111/Microstrip-Patch-Antenna.git](https://github.com/Ommmarr111/Microstrip-Patch-Antenna.git)
    ```
2.  Open `Microstrip Antenna Project.cst` in **CST Studio Suite**.
3.  If results are missing, go to **Home > Parametric Update (F7)**.
4.  Run the **Transient Solver** to regenerate results.

---

## 👤 Author
**Omar Ahmed**
