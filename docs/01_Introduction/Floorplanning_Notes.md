# Floorplanning

## What is Floorplanning?

Floorplanning is the first physical design stage after synthesis. It defines the physical layout of the chip before placing the standard cells.

Main objectives:
- Define die and core area
- Perform power planning
- Place I/O pins
- Reserve routing space

---

## Floorplan Configuration

The floorplan is controlled using the **floorplan.tcl** configuration file.

Important parameters include:
- Core Utilization
- Aspect Ratio
- Core Margin
- Pin Placement
- Metal Layers

These parameters determine how the chip floorplan is generated.

---

## Floorplanning Output

After floorplanning, OpenLANE generates:

- Floorplan DEF file
- Floorplan reports
- Floorplan logs

These files are stored inside the **runs** directory.

---

## DEF File

DEF (Design Exchange Format) contains the physical information of the design, such as:

- Die dimensions
- Core dimensions
- Placement rows
- Pin locations
- Cell placement information

---

# Placement

## What is Placement?

Placement is the process of assigning each standard cell to a physical location inside the core.

The main objective is to minimize wire length while improving timing and reducing congestion.

---

## Placement Steps

### 1. Bind Netlist with Physical Cells

The synthesized netlist is mapped to the standard cells available in the Sky130 library.

### 2. Initial Placement

Standard cells are placed inside the core based on connectivity.

### 3. Placement Optimization

The placement is optimized to:

- Reduce wire length
- Improve timing
- Reduce congestion
- Improve overall design quality

---

## Viewing the Floorplan

The generated layout can be viewed using **Magic VLSI**.

Magic is used to visualize:
- Standard cells
- Metal layers
- Pins
- Core area
- Die area

---

## Key Points

- Floorplanning is performed before placement.
- Core is the region where standard cells are placed.
- Die is the complete chip area.
- DEF stores physical design information.
- Good placement improves timing and routing.

---

## Summary

- Learned the purpose of floorplanning.
- Studied the floorplan configuration file.
- Understood DEF files.
- Learned the placement process.
- Viewed layouts using Magic VLSI.
