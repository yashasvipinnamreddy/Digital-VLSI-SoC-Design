# OpenLANE Basics

## OpenLANE Directory Structure

The OpenLANE working directory contains important folders:

- `pdks/` – Process Design Kits (Sky130 PDK)
- `openlane/` – OpenLANE flow
- `designs/` – User designs
- `scripts/` – Automation scripts
- `configuration/` – Configuration files

---

## Sky130 PDK

The Sky130 PDK contains:

- libs.ref
- libs.tech
- Standard Cell Libraries
- Technology Files

The two main folders are:

- `libs.ref` – Library files
- `libs.tech` – Technology files used by EDA tools

---

## Design Directory

Inside the `designs` folder, every design has its own directory.

Example:

```
designs/
   picorv32a/
```

Important files:

- `config.tcl`
- `src/`
- `runs/`

---

## Run Directory

Whenever OpenLANE executes a design, a new run folder is created.

Example:

```
runs/
   12-08_10-49/
```

This folder stores all generated outputs.

---

## Important Run Folders

```
results/
reports/
logs/
tmp/
```

- **results/** → Final outputs of each stage
- **reports/** → Timing and synthesis reports
- **logs/** → Execution logs
- **tmp/** → Temporary files

---

## Synthesis Statistics

After synthesis, OpenLANE generates:

- Number of cells
- Number of wires
- Number of ports
- Number of nets
- Cell utilization

These statistics help analyze the synthesized design.

---

# Floorplanning

Floorplanning defines the chip dimensions before placement.

Two important terms:

### Core

Area where standard cells are placed.

### Die

Complete chip area including the core and boundary.

---

## Utilization Factor

```
Utilization Factor =
Area Occupied by Cells
----------------------
Total Core Area
```

Higher utilization means less empty space inside the core.

---

## Aspect Ratio

```
Aspect Ratio =
Height
------
Width
```

It defines the shape of the core.

---

# Power Planning

Power planning distributes VDD and GND across the chip.

Purpose:

- Stable power supply
- Reduce voltage drop
- Reduce IR drop

Power rails are created before placement.

---

# Pin Placement

Pins are placed around the boundary of the chip.

Good pin placement:

- Reduces routing congestion.
- Improves signal routing.
- Improves overall chip performance.

---

## Summary

- Explored the OpenLANE directory structure.
- Learned the Sky130 PDK hierarchy.
- Understood design and run folders.
- Studied synthesis reports.
- Learned floorplanning concepts.
- Understood utilization factor and aspect ratio.
- Learned the basics of power planning and pin placement.
