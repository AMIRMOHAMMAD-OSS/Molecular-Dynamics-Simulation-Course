# Molecular Dynamics Study of Doxorubicin Interaction with a Functionalized Carbon Nanotube

## Overview

This repository contains molecular dynamics simulation files and analysis
outputs for studying the interaction between **doxorubicin (DOX)** and a
**functionalized carbon nanotube (CNT)** using **GROMACS**.

The project investigates the structural behavior and interaction properties of
a CNT–DOX system in aqueous solution using atomistic molecular dynamics
simulations.

---

## Research Question

**How does doxorubicin interact with a functionalized carbon nanotube surface
under molecular dynamics simulation conditions?**

The study focuses on:

- CNT–DOX interaction energy
- Electrostatic and van der Waals contributions
- Hydrogen-bond interactions
- Enhanced sampling using umbrella sampling

---

## System Description

The simulated system consists of:

- Functionalized carbon nanotube (CNT)
- Doxorubicin molecule (DOX)
- Explicit water solvent
- Sodium counterions

Simulation conditions:

| Parameter | Value |
|---|---|
| Software | GROMACS |
| Force field | GROMOS54a7 |
| Temperature | 310 K |
| Pressure | 1 bar |
| Solvent | Explicit water |
| Ensemble | NVT / NPT / Production MD |

---

# Simulation Workflow

```
System preparation
        |
        ↓
Energy minimization
        |
        ↓
NVT equilibration
        |
        ↓
NPT equilibration
        |
        ↓
Production molecular dynamics
        |
        ↓
Interaction analysis
        |
        ↓
Umbrella sampling (exploratory)
        |
        ↓
WHAM analysis
```

---

# Molecular Dynamics Simulation

The production simulation was performed using GROMACS with:

- Leap-frog molecular dynamics integrator
- Particle Mesh Ewald (PME) electrostatics
- V-rescale thermostat
- Pressure coupling at 1 bar

The production trajectory was analyzed to characterize CNT–DOX interactions.

---

# Analysis Performed

## CNT–DOX Interaction Energy

The interaction between the nanotube and doxorubicin was evaluated through:

- Lennard-Jones interactions
- Coulombic interactions

The analysis provides information about the energetic contributions
stabilizing the CNT–DOX system.

---

## Hydrogen Bond Analysis

Hydrogen-bond contacts between CNT and DOX were evaluated during the
simulation to characterize specific intermolecular interactions.

---

## Umbrella Sampling

Umbrella sampling was performed as an enhanced-sampling extension.

The workflow included:

- Steered molecular dynamics
- Multiple umbrella windows
- WHAM analysis

The sampling quality was evaluated by examining histogram overlap between
neighboring umbrella windows.

---

# Repository Structure

```
.
├── analysis/
│   ├── Interaction energy outputs
│   ├── Hydrogen-bond analysis
│   └── WHAM outputs
│
├── simulation/
│   ├── Production MD parameters
│   ├── Pulling parameters
│   └── Umbrella sampling parameters
│
├── topology/
│   ├── CNT/DOX topology files
│   └── Molecular index files
│
└── figures/
    └── Analysis plots and visualizations
```

---

# Results Summary

## CNT–DOX Interaction

The production MD trajectory shows favorable CNT–DOX interactions,
dominated by van der Waals contributions.

The interaction analysis indicates stabilization of the drug molecule near the
functionalized CNT surface during the simulation.

---

# Umbrella Sampling Note

The umbrella sampling calculation was evaluated through histogram overlap
analysis.

Several neighboring windows showed limited overlap, therefore the resulting
PMF is considered **exploratory** and is not interpreted as a final quantitative
binding free-energy estimate.

This assessment highlights the importance of validating sampling convergence
before extracting thermodynamic quantities.

---

# Software and Tools

- **GROMACS** — Molecular dynamics simulation
- **WHAM** — Free-energy analysis
- **VMD** — Molecular visualization
- **Python** — Data processing and visualization

---

# Reproducibility

The repository contains:

- GROMACS parameter files (`.mdp`)
- Molecular topology files
- Index files
- Analysis outputs

Large trajectory files are excluded because of repository size limitations.

---

# Author

**AMIRMOHAMMAD-OSS**

Computational Molecular Dynamics Project
