# Introduction to Digital VLSI SoC Design

## Objective

This section introduces the fundamentals of digital ASIC design, the RTL-to-GDSII flow, OpenLANE, and the Sky130 PDK.

---

## Key Concepts

### What is VLSI?

**VLSI (Very Large Scale Integration)** is the process of integrating millions or billions of transistors onto a single Integrated Circuit (IC).

Examples:
- Processors
- Memory Chips
- Microcontrollers

---

### What is SoC?

**SoC (System on Chip)** integrates multiple hardware components on a single chip.

Typical components include:
- CPU
- Memory
- Communication Interfaces
- Peripherals

Advantages:
- Compact size
- High performance
- Low power consumption

---

### Software to Hardware Overview

A program reaches the hardware through several layers.

```
Application Software
        ↓
Operating System
        ↓
Compiler
        ↓
Instruction Set Architecture (ISA)
        ↓
Hardware
```

- Applications are written by programmers.
- The Operating System manages hardware resources.
- The Compiler converts programs into machine instructions.
- The ISA acts as the interface between software and hardware.
- The Hardware executes the instructions.

---

## RTL to GDSII Flow

OpenLANE converts an RTL design into a manufacturable chip layout.

```
RTL
 ↓
Synthesis
 ↓
Floorplanning
 ↓
Placement
 ↓
Clock Tree Synthesis (CTS)
 ↓
Routing
 ↓
Sign-off
 ↓
GDSII
```

### Flow Overview

- **Synthesis** – Converts RTL into a gate-level netlist.
- **Floorplanning** – Defines chip size and placement regions.
- **Placement** – Places standard cells inside the chip.
- **Clock Tree Synthesis (CTS)** – Distributes the clock signal.
- **Routing** – Connects all components using metal layers.
- **Sign-off** – Performs final verification before fabrication.
- **GDSII** – Final layout file sent for chip manufacturing.

---

## What is OpenLANE?

OpenLANE is an open-source ASIC implementation flow.

It automates:
- Logic Synthesis
- Floorplanning
- Placement
- Clock Tree Synthesis
- Routing
- Physical Verification
- GDSII Generation

---

## Sky130 PDK

The **Sky130 Process Design Kit (PDK)** provides the technology files required for designing chips in the SkyWater 130 nm process.

It includes:
- Standard Cell Libraries
- Design Rules
- Technology Files
- Device Models

---

## OpenLANE Flow

The OpenLANE flow integrates multiple open-source tools to perform the complete ASIC design process from RTL to GDSII.

Major stages:
- RTL Synthesis
- Static Timing Analysis (STA)
- Floorplanning
- Placement
- CTS
- Routing
- Physical Verification
- GDSII Generation

---

## RISC-V (Introduction)

RISC-V is an **open-source Instruction Set Architecture (ISA)**.

It defines the instructions that a processor understands and executes. Many open-source processor designs use the RISC-V ISA.

---

## Key Terms

| Term | Meaning |
|------|---------|
| VLSI | Very Large Scale Integration |
| SoC | System on Chip |
| RTL | Register Transfer Level |
| PDK | Process Design Kit |
| ISA | Instruction Set Architecture |
| CTS | Clock Tree Synthesis |
| GDSII | Final chip layout file |

---

## Key Takeaways

- Learned the basic VLSI design terminology.
- Understood the software-to-hardware stack.
- Introduced to the RTL-to-GDSII ASIC flow.
- Learned the role of OpenLANE and Sky130 PDK.
- Understood the importance of RISC-V in open-source processor design.

---

## Screenshots to Include

Save the following screenshots in the `screenshots` folder:

- Software to Hardware Overview
- RTL to GDSII Flow
- OpenLANE ASIC Flow
- SoC Design using OpenLANE
