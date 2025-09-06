
# 🧺 FSM-Based Washing Machine

## 📌 Project Overview

This project implements a **Finite State Machine (FSM) based Washing Machine** using **HDL (Verilog)**.
The design models a real washing machine controller with multiple states, transitions, and operations such as washing, rinsing, and drying.

The FSM ensures **sequential operation**, **predictable behavior**, and **modular design** for hardware implementation on FPGA/ASIC platforms.

---

## 🚀 Features

* ✅ FSM-based design with clear **state transitions**
* ✅ Supports **Idle, Fill, Wash, Rinse, Spin/Dry, and Done states**
* ✅ User-controlled **start/stop/reset** inputs
* ✅ Can be synthesized and tested on FPGA boards
* ✅ Testbench provided for **simulation and verification**

---

## 🔄 FSM States

The washing machine follows these states:

1. **Idle** → Waiting for start signal
2. **Fill** → Water filling process
3. **Wash** → Washing with detergent
4. **Rinse** → Rinsing with clean water
5. **Spin/Dry** → Spinning clothes to remove water
6. **Done** → Cycle complete

### Example FSM Diagram:

```
      ┌───────┐
      │  Idle │
      └───┬───┘
          │ Start
          ▼
       ┌───────┐
       │  Fill │
       └───┬───┘
           ▼
       ┌───────┐
       │  Wash │
       └───┬───┘
           ▼
       ┌───────┐
       │ Rinse │
       └───┬───┘
           ▼
       ┌───────┐
       │  Spin │
       └───┬───┘
           ▼
       ┌───────┐
       │  Done │
       └───────┘
```

---

## ⚙️ Project Structure

```
📂 FSM_Washing_Machine
 ┣ 📜 washing_machine.v   # FSM Design (Verilog)
 ┣ 📜 tb_washing_machine.v # Testbench
 ┣ 📜 README.md             # Project Documentation
 ┗ 📂 docs                  # State diagram, reports
```

---

## 🛠️ How to Run

1. Clone the repo:

   ```bash
   git clone https://github.com/Hirdesh04vlsi/FSM_Washing_Machine.git
   ```
2. Open in **Xilinx Vivado / ModelSim / Quartus**
3. Compile design and testbench files
4. Run simulation to verify state transitions
5. (Optional) Implement on FPGA board

---

## 📊 Simulation

* Testbench verifies **all state transitions**.
* Outputs include **state signals** and **control flags** for motor, water inlet, and dryer.

---

## 👨‍💻 Author

**Hirdesh Pamnani**
ECE Student | VLSI & Digital Design Enthusiast

---

Do you want me to also make a **GitHub-ready version** with emojis, badges (like "Made with VHDL" / "Simulation Passed"), and images of the FSM diagram for better presentation?
