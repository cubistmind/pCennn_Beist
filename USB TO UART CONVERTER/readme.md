# USB-to-Serial UART Converter
<img width="1656" height="928" alt="USB TO SERIAL UART CONVERTERo" src="https://github.com/user-attachments/assets/9857fc18-000d-4242-b912-fa639a4a4a27" />
<img width="1656" height="928" alt="USB TO SERIAL UART CONVERTER" src="https://github.com/user-attachments/assets/3bd7bb03-c0ad-42a9-bd79-b50e2fef676e" />

A custom USB-to-UART converter PCB designed using **KiCad 10**.

This project implements a USB-to-serial communication interface using the FT232RL USB-to-UART bridge IC. The PCB provides a USB Mini-B connection and a dedicated UART output header for interfacing with external embedded systems, microcontrollers, and development boards.

## Project Overview

| Parameter | Specification |
|---|---|
| Project | USB-to-Serial UART Converter |
| Main IC | FT232RL |
| USB Connector | Mini-B |
| Communication | USB to UART |
| PCB Layers | 2-layer |
| EDA Software | KiCad 10 |
| Design Type | Custom PCB |
| PCB Fabrication | Gerber and Excellon outputs included |

## Features

- FT232RL-based USB-to-UART conversion
- USB Mini-B interface
- Dedicated 6-pin UART output connector
- RGB LED indicator
- Through-hole and SMD components
- Four PCB mounting holes
- Two-layer PCB design
- Front and back copper routing
- Manufacturing-ready Gerber and drill outputs

## Hardware Components

| Component | Description |
|---|---|
| U1 | FT232RL USB-to-UART bridge |
| J1 | USB Mini-B connector |
| J2 | 3-pin jumper |
| J3 | 6-pin UART output |
| D1 | RGB LED |
| FB1 | Ferrite bead |
| R1–R3 | Resistors |
| C1–C5 | Capacitors |

Refer to `BOM.csv` for the component list and footprints.

## PCB Design

The PCB was designed and routed in KiCad 10.

The design includes:
- Front copper layer (F.Cu)
- Back copper layer (B.Cu)
- Front and back solder masks
- Front and back silkscreen
- Defined board outline
- Plated and non-plated drill holes

## Design Verification

The design was checked using KiCad's Electrical Rules Checker (ERC) and Design Rules Checker (DRC).

**Reported verification status:**
- ERC: 0 errors, 0 warnings
- DRC: 0 errors, 0 warnings

These results indicate that the configured schematic and PCB design checks passed. Physical hardware operation still requires fabrication and functional testing.

## Repository Structure

```text
USB-to-Serial-UART-Converter/
│
├── USB TO SERIAL UART CONVERTER.kicad_pro
├── USB TO SERIAL UART CONVERTER.kicad_sch
├── USB TO SERIAL UART CONVERTER.kicad_pcb
│
├── BOM.csv
│
├── GERBER/
│   ├── F_Cu.gtl
│   ├── B_Cu.gbl
│   ├── F_Mask.gts
│   ├── B_Mask.gbs
│   ├── F_Silkscreen.gto
│   ├── B_Silkscreen.gbo
│   ├── Edge_Cuts.gm1
│   ├── PTH.drl
│   ├── NPTH.drl
│   └── Gerber job file
│
└── README.md
```

## Manufacturing

The repository includes Gerber fabrication files and Excellon drill files for a two-layer PCB.

For PCB fabrication, provide the manufacturer with the complete Gerber and drill file set.

For PCBA, additionally prepare:
- Verified BOM with manufacturer part numbers
- Component Placement List (CPL)
- Solder-paste stencil files, where required

## Getting Started

1. Clone or download this repository.
2. Open the `.kicad_pro` file using KiCad 10.
3. Inspect the schematic and PCB layout.
4. Review the BOM and manufacturing outputs.
5. Generate updated Gerber files if the design is modified.

## Project Status

**PCB Design: Completed**

**ERC/DRC: Passed according to the latest project checks**

**Physical Hardware Testing: Pending**

## License

Add your preferred open-source hardware license before distributing or manufacturing derivative designs.

---

Designed with KiCad 10.

**USB-to-Serial UART Converter | Electronics & PCB Design Project**
