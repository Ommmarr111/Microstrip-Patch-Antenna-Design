# 📡 5GHz Microstrip Patch Antenna Design

[![CST Studio Suite](https://img.shields.io/badge/Tools-CST_Studio_Suite-blue?style=flat-square&logo=dasher)](https://www.3ds.com/products-services/simulia/products/cst-studio-suite/)
[![Field](https://img.shields.io/badge/Field-RF_%26_Antennas-orange?style=flat-square)](https://en.wikipedia.org/wiki/Microstrip_antenna)

An optimized design and simulation of a **Microstrip Patch Antenna** operating at the **5 GHz** frequency band. This project focuses on achieving high return loss and efficient power transmission through precise impedance matching using the **Inset Feed** technique.

---

## 🎯 Project Overview
This project was developed as part of the **Electronics and Communication Engineering (ECE)** curriculum. The goal was to design a Microstrip patch antenna targeting a resonant frequency of 5 GHz with a characteristic line impedance of 50 $\Omega$.

### ✨ Key Features
* **Impedance Matching:** Implemented an **Inset Feed** to reach the 50 $\Omega$ locus on the patch, eliminating the need for external matching circuits.
* **High Performance:** Achieved a Return Loss ($S_{11}$) of **-22.46 dB** and a VSWR of **1.16 : 1**, indicating near-perfect matching and minimal power reflection.
* **Parametric Modeling:** The design is fully parameterized, allowing for rapid frequency tuning and optimization.

---

## 📊 Technical Specifications

| Parameter | Value | Description |
| :--- | :--- | :--- |
| **Center Frequency** | 5.0 GHz | Target Resonant Frequency |
| **Return Loss ($S_{11}$)** | -22.46 dB | Magnitude at 4.97 GHz |
| **VSWR** | 1.16 : 1 | Voltage Standing Wave Ratio |
| **Gain** | 7.01 dBi | Peak Directivity (Broadside) |
| **Substrate** | FR-4 (lossy) | $\epsilon_r = 4.3$, $h = 1.6$ mm |
| **Efficiency** | ~44% | Radiation Efficiency (Dielectric loss expected) |
| **Feeding Method** | Inset Feed | Optimized for 50 $\Omega$ SMA Edge Connector |

---

## 📐 Dimensions & Parameters
The following fully optimized parameters were used in the CST model:

* **L (Patch Length):** 13.90 mm
* **W (Patch Width):** 18.40 mm
* **W_f (Feed Width):** 3.00 mm
* **Fi (Inset Depth):** 4.00 mm
* **G (Feed Gap):** 1.00 mm
* **h (Substrate Height):** 1.60 mm
* **t (Copper Thickness):** 0.035 mm
* **Lsub / Wsub (Ground Dimensions):** 40.00 mm x 40.00 mm

---

## 📈 Simulation Results

### 1. S-Parameters ($S_{11}$) & VSWR
The simulation shows a sharp resonance at **4.97 GHz** with a <1% error margin from the design target. The VSWR graph confirms optimal power transmission, safely below the 2.0 threshold.

> *(Optional: Upload `s11_plot.png` and `vswr_plot.png` to your repo and link them here)*
> 
> <img width="1581" height="516" alt="Screenshot 2026-05-11 223152" src="https://github.com/user-attachments/assets/398822c2-a315-496f-b733-a0743e77b460" />
> <img width="1562" height="517" alt="Screenshot 2026-05-11 223436" src="https://github.com/user-attachments/assets/08d05a50-f214-4b12-a00e-379e43f80013" />


### 2. Radiation Pattern
The antenna exhibits a clear **Broadside Radiation Pattern**, typical for patch antennas, with maximum directivity along the Z-axis.

> *(Optional: Upload `farfield.png` to your repo and link it here)*
> 
> <img width="1266" height="525" alt="Screenshot 2026-05-11 223640" src="https://github.com/user-attachments/assets/3d6ad19e-4da6-4391-beb6-7723f355d24f" />


---

## 💻 How to Run
1.  Clone this repository:
    ```bash
    git clone [https://github.com/Ommmarr111/Microstrip-Patch-Antenna.git](https://github.com/Ommmarr111/Microstrip-Patch-Antenna.git)
    ```
2.  Open `Microstrip Antenna Project.cst` in **CST Studio Suite**.
3.  If results are missing, go to **Home > Parametric Update (F7)** to rebuild the model.
4.  Run the **Transient Solver** to regenerate the 1D and Farfield results.

---

## 👥 Project Team
* **Omar Ahmed Othman**
* **Abdelrahman Mahmoud Rady**
* **Mohamed Ahmed Mohamed Kassem**

**Supervised By:** Dr. Ahmed Hamdy
