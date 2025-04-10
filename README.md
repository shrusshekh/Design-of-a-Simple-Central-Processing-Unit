# COE328 Lab 6 – Design of a Simple Central Processing Unit (CPU)

**Toronto Metropolitan University**  
**Department of Electrical, Computer and Biomedical Engineering**  
**Course:** COE 328 – Digital Systems  
**Lab 6 Duration:** 2 Weeks

---

## 📌 Overview

This project involved the design and simulation of a simplified **Central Processing Unit (CPU)** using **VHDL** on **Quartus** for FPGA implementation. The CPU includes an **Arithmetic Logic Unit (ALU)**, **Register Units**, a **Moore Finite State Machine (FSM)**, and a **Decoder**. The final design integrates all these components and is simulated using waveform outputs and tested on an Altera FPGA board.

---

## 🎯 Objectives

- Design and implement all ALU functionalities in VHDL.
- Create a CPU control unit using FSM and decoder components.
- Simulate and test the CPU system using Quartus Prime.
- Display ALU results and control states on 7-segment displays.
- Extend ALU functionality using student ID digits as dynamic input.

---

## 🧩 System Architecture

The system includes the following main modules:

- **Register Units**: Temporary storage for 8-bit input operands A and B.
- **ALU Core**: Performs arithmetic and logic operations based on an 8-bit opcode.
- **FSM (Program Counter)**: Acts as a 3-bit up-counter cycling through 8 states.
- **3x8 Decoder**: Converts FSM states into operation codes for the ALU.
- **7-Segment Displays**: Show ALU results and FSM output (student ID).

---

## ⚙️ ALU Operations

The ALU supports a wide variety of operations, including:

| Function | Opcode     | Operation                  |
|----------|------------|----------------------------|
| 1        | `00000001` | A + B                      |
| 2        | `00000010` | A - B                      |
| 3        | `00000100` | NOT A                      |
| 4        | `00001000` | NAND A, B                  |
| 5        | `00010000` | NOR A, B                   |
| 6        | `00100000` | AND A, B                   |
| 7        | `01000000` | XOR A, B                   |
| 8        | `10000000` | OR A, B                    |

Additional operations were implemented based on TA-assigned modifications for Problems 2 & 3.

---

## 🛠 Technologies & Tools

- **VHDL** – Digital design language for FPGA logic
- **Quartus** – Design and simulation software
- **ModelSim** – Waveform simulation
- **Altera DE-Series FPGA Board** – Hardware implementation

---


