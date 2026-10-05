# Molecular Dynamics Simulation Course

This repository contains molecular dynamics simulations and practical exercises completed as part of the **Advanced Molecular Dynamics and Protein Simulation with GROMACS** course by **FaraDars**, which I completed in June 2025.

The projects were carried out primarily using **GROMACS** for molecular dynamics simulations and **VMD** for molecular visualization and trajectory rendering.

## Course

**Advanced Molecular Dynamics and Protein Simulation with GROMACS**  
Instructor: **Dr. Azadeh Kordzadeh**  
Completed: **June 20, 2025**

- [Course page](https://faradars.org/courses/simulation-of-molecular-dynamics-and-proteins-with-gromacs-supplementary-fvch0101)
- [Certificate verification](https://faradars.org/verify/C89CA8ED)

---

## Repository Contents

### S03 — Lysozyme Molecular Dynamics

Molecular dynamics simulation of **lysozyme in explicit solvent**.

The system was prepared, energy-minimized, equilibrated under NVT and NPT conditions, and followed by a production MD simulation.

### MD Trajectory

![Lysozyme MD Simulation](S03/lyzozyme/lysozyme_md.gif)

---

### S04 — Carbon Nanotube and Doxorubicin

Molecular dynamics simulation of **doxorubicin (DOX)** interacting with a **carbon nanotube (CNT)** in aqueous solution.

The system includes:

- Carbon nanotube
- Multiple doxorubicin molecules
- Explicit water
- Production molecular dynamics trajectory

The trajectory shows the motion and interaction of DOX molecules around the nanotube surface.

![CNT–DOX MD](S04/cnt/s04_final.gif)

---

### S05 — DPPC Membrane Simulation

Preparation and molecular dynamics simulation of a **DPPC lipid bilayer** in explicit solvent.

This section includes membrane system construction, energy minimization, equilibration, and production MD.

---

### S06 — Doxorubicin Pulling Through a Carbon Nanotube

Steered molecular dynamics and umbrella-sampling setup for pulling a **DOX molecule along the axis of a carbon nanotube**.

The trajectory shows the molecule moving from one side of the CNT, through its interior, and toward the opposite side.

![DOX Pulling Through CNT](S06/umbrella1/umbrella/vmd_output_s06_final/s06_final.gif)

---

## Tools

- **GROMACS** — molecular dynamics simulations
- **VMD** — molecular visualization and trajectory rendering
- **ImageMagick** — GIF generation and image conversion

---

## Author

**AmirMohammad MohammadHosseini**  
GitHub: [AMIRMOHAMMAD-OSS](https://github.com/AMIRMOHAMMAD-OSS)
