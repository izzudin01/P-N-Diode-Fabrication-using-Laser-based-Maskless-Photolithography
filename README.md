# P-N Diode Fabrication using Laser-Based Maskless Photolithography (Boron P-Type Doping)

This project demonstrates the fabrication of **P–N diode structures** by forming a **p-type region (boron doping)** on an **n-type silicon wafer** using a **laser-based maskless photolithography** approach. The fabricated samples were evaluated using **I–V sweep** and **reverse-bias I–V** characterization.

> Report (full documentation): see `https://github.com/izzudin01/P-N-Diode-Fabrication-using-Laser-based-Maskless-Photolithography/blob/main/Final%20Project%20Report_%20DEL_Izzudin%20Al%20Ayyubi_2006574780%20(Indonesian).pdf`.

---

## Overview
The work implements a maskless lithography workflow to open diffusion windows on silicon (SOI in the experiment context) and perform localized p-type doping using boron-based dopant. The resulting diode samples are characterized to assess fabrication quality and variability across a 3×3 sample matrix.

![](https://github.com/izzudin01/P-N-Diode-Fabrication-using-Laser-based-Maskless-Photolithography/blob/main/Picture/Screenshot%202026-02-12%20223523.png)

## Background
Lithography is a key step in semiconductor microfabrication. Conventional mask-based lithography is efficient for mass production but less flexible for rapid iteration. **Maskless photolithography** enables direct patterning without a physical mask, making it suitable for R&D, low-volume prototyping, and fast design changes.  
In P–N diode fabrication, maskless lithography can support targeted doping region formation with reduced turnaround time and cost.

---

## Objectives
1. Implement **p-type doping** on **n-type silicon** using **laser-based maskless photolithography**.
2. Analyze the resulting P–N diode characteristics through **I–V sweep** and **reverse-bias I–V** measurements.

---

## Methodology (High-Level)
### 1) Diffusion Window Opening (Laser Maskless Process)
- Laser parameters were varied (power and pulse frequency) while maintaining fixed scan speed and loop count.
- The effectiveness of window opening/doping indication was evaluated using resistance measurement.

### 2) Boron Dopant Preparation & Doping Process
- Boron dopant was prepared as a boric-acid-based solution and applied on the wafer surface.
- Doping was performed through patterned exposure/processing on predefined window regions.

### 3) Electrical Characterization
- Nine diode samples were arranged in a **3×3 matrix** (positions (1,1) to (3,3)).
- **I–V sweep** test: 0 to 6 V (step 0.1 V).
- **Reverse I–V** test: -5 to 0 V (step 0.05 V).
- Measurement used a semiconductor parameter analyzer (as documented in the report).

> Detailed procedure, figures, and equipment setup are documented in the full PDF report.

---

## Results
### A) Laser Parameter Sweep (Resistance-Based Evaluation)
Power (W): 10 / 20 / 30  
Frequency (kHz): 25 / 50 / 75  

The study found an optimal parameter combination at **20 W and 75 kHz**, producing the lowest measured resistance (~0.444 MΩ), indicating the most effective window opening/doping condition among tested configurations.

### B) I–V Sweep Characteristics (Forward Bias)
- Samples at **(1,1), (1,3), and (3,1)** showed the closest behavior to an ideal diode: forward current increased with voltage in a more exponential trend, although slower than ideal.
- Samples at **(2,3), (3,2), and (3,3)** showed poor performance with significant fluctuation/instability and larger leakage behavior at low voltage, suggesting issues such as non-uniform doping, contact resistance, or measurement noise.
- Other samples showed intermediate performance.

### C) Reverse-Bias I–V Characteristics
- Samples **(1,1), (1,2), and (3,2)** showed the best reverse-bias behavior with stable current response and no breakdown up to **-5 V**.
- Some samples showed oscillation at higher reverse voltage (above ~-3 V), likely due to measurement instability/contact issues or material inconsistency.
- Several samples showed nearly flat curves (very high reverse resistance), potentially indicating over-wide depletion region or less optimal doping.

---
![](https://github.com/izzudin01/P-N-Diode-Fabrication-using-Laser-based-Maskless-Photolithography/blob/main/Picture/Screenshot%202026-02-12%20223602.png)
![](https://github.com/izzudin01/P-N-Diode-Fabrication-using-Laser-based-Maskless-Photolithography/blob/main/Picture/Screenshot%202026-02-12%20223548.png)


## Conclusion
- Laser power and pulse frequency significantly affect diffusion window results and electrical behavior.
- The **20 W / 75 kHz** configuration provided the most favorable resistance outcome among tested settings.
- Diode performance varied across the 3×3 matrix: a subset of samples approached expected diode-like I–V behavior, while others showed instability, leakage, and inconsistency likely caused by doping non-uniformity, contact quality, and measurement noise.
- Improvements are suggested via tighter process control for doping uniformity, enhanced contact formation to reduce series resistance, and improved measurement setup stability.

---

## Repository Contents
- `report/` : Full project report (PDF)
- `figures/` : Key images (workflow, diffusion window, I–V plots)

---

## Notes
This repository is intended for academic/portfolio documentation. Some proprietary tool files and lab machine configurations are not included.
