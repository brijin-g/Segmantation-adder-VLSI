# Segmentation Adder – FPGA & ASIC Implementation

This project implements a **Segmentation Adder** architecture aimed at improving the speed and power efficiency of arithmetic operations. The design is realized using **Verilog HDL** and validated on both **FPGA (Basys3)** and **ASIC (SkyWater 130nm PDK)** platforms.

---

## 🧠 Abstract

The Segmentation Adder divides operands into smaller segments and processes them in parallel, minimizing carry propagation delay. The project follows a complete digital design flow from **RTL to GDSII**, including FPGA deployment and waveform verification.

---

## 🛠️ Tools & Technologies

- **Languages**: Verilog HDL
- **FPGA Tools**: Xilinx Vivado 2024.2, GTKWave
- **ASIC Tools**: Yosys, OpenLane, KLayout, SkyWater 130nm PDK
- **Simulation**: Icarus Verilog + GTKWave
- **Hardware**: Basys3 FPGA Board

---

## 🧩 Features

- 8-bit and optimized 4-bit Segmentation Adders
- Verilog-based modular design with testbenches
- GTKWave simulation and waveform analysis
- FPGA deployment with I/O mapping via XDC
- ASIC flow including synthesis, placement, routing, and GDSII export

---

## 🔍 Methodology

### FPGA Path:
1. Verilog design coded and tested with testbench.
2. Simulated using Vivado/GTKWave.
3. Deployed on Basys3 FPGA with LED/SW pin mapping.
4. Power and temperature issues mitigated by optimizing to 4-bit design.

### ASIC Path:
1. RTL synthesized with Yosys using Sky130 PDK.
2. Floorplanning, placement, and routing via OpenLane.
3. Layout verified using KLayout and Magic.
4. GDSII generated for fabrication readiness.

---

## 📊 Results

| Metric                | 8-bit Adder      | 4-bit Adder     |
|----------------------|------------------|-----------------|
| Power Consumption     | 47.26 W          | 9.53 W          |
| Junction Temperature | 125°C (Overheat) | 72.7°C (Safe)   |
| Thermal Margin        | –176.3°C         | +12.3°C         |
| Performance           | Functional       | Optimized       |

---

