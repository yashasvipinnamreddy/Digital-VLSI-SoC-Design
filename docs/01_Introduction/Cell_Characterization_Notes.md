---

# Cell Design Flow

## What is Cell Design?

Cell design is the process of creating standard cells that are used during physical design.

The cell design flow includes:
- Circuit Design
- Layout Design
- Characterization

The inputs required are:
- Process Design Kit (PDK)
- Design Rules (DRC/LVS)
- SPICE Models
- Standard Cell Library Specifications

---

# Cell Characterization

Characterization is the process of measuring the electrical behavior of a standard cell.

It helps determine:
- Propagation Delay
- Rise Time
- Fall Time
- Power Consumption
- Timing Information

These values are stored in the standard cell library and are used during synthesis and timing analysis.

---

# Timing Characterization

Timing characterization defines the timing thresholds used to measure circuit performance.

Important timing parameters include:
- Input Rise Threshold
- Input Fall Threshold
- Output Rise Threshold
- Output Fall Threshold
- Rise Delay
- Fall Delay

Propagation delay is calculated between the input and output threshold points.

---

# SPICE Deck

A SPICE deck is a text file used to simulate electronic circuits.

It contains:
- Component connectivity
- Component values
- Circuit nodes
- Simulation commands

SPICE simulations help verify the behavior of the designed circuit before fabrication.

---

# VTC (Voltage Transfer Characteristic)

The Voltage Transfer Characteristic (VTC) curve shows the relationship between input voltage (Vin) and output voltage (Vout) of a CMOS inverter.

The VTC is used to determine:
- Switching Threshold (Vm)
- Noise Margin
- Switching Behavior

Changing transistor sizes affects the switching threshold and inverter performance.

---

# SPICE Simulation

The designed circuit can be simulated using **ngspice**.

Simulation helps verify:
- Output waveform
- Delay
- Voltage levels
- Circuit functionality

Simulation results are compared with the expected behavior before moving to fabrication.

---

## Summary

- Learned the standard cell design flow.
- Understood the purpose of characterization.
- Studied timing characterization parameters.
- Learned the structure of a SPICE deck.
- Performed SPICE simulation using ngspice.
- Understood Voltage Transfer Characteristics (VTC) of a CMOS inverter.
