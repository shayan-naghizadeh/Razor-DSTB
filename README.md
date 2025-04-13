# Razor-DSTB
# Razor-DSTB
# ⚙️ VLSI Sequential Element Design – Latch, Flip-Flop, Razor/DSTB

This repository contains the VLSI design, HSPICE simulation, and timing analysis of key sequential elements: **Latch**, **Flip-Flop**, and **Razor/DSTB error detection circuits**.  
The project is implemented using tri-state inverter logic and includes precise measurements of setup/hold times, delays, and signal correctness.

---

## 📐 Project Summary

The goal of this project is to design sequential memory elements capable of functioning correctly at high frequencies and respond appropriately to timing violations such as late input transitions.  
This includes simulating behavior during **forbidden time windows**, analyzing **VTC curves**, and constructing circuits with robust **error detection**.

---

## 🔧 Components Implemented

### 1️⃣ Latch (Tri-State Based)
- Designed using a **tri-state inverter pair**.
- Tested for:
  - **Setup and hold violations**
  - Internal timing correctness
- Simulated transitions and setup behavior around clock edges.

### 2️⃣ Flip-Flop (Master-Slave)
- Built from cascaded latches (edge-triggered).
- Complete timing characterization:
  - `Tcq`, `Tdq`, `Setup`, `Hold`
- Rise/fall variations included.

### 3️⃣ Razor / DSTB Circuit
- Error detection using XOR of latch and flip-flop outputs.
- Handles setup violations gracefully.
- Differentiates between safe and unsafe timing zones using flag signals.
- Demonstrates metastability-safe response via DSTB mechanism.

---

## 📊 Key Features

- **VTC curve analysis** for inverters
- **Setup/Hold timing visualization**
- Full behavior simulation for edge violations
- XOR-based fault indication logic
- Comparison between Razor and DSTB response
- Gate-level design focused on noise tolerance and high-speed operation

---

## 🧪 Simulation Environment

All components were simulated using **HSPICE**.