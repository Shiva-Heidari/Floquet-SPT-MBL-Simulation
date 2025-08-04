# floquet-spt-mbl-simulation
# Floquet SPT-MBL vs. ETH Simulation in a 6-Qubit Spin Chain

This project explores the contrasting dynamical behavior of **Floquet symmetry-protected topological (SPT) phases stabilized by many-body localization (MBL)** versus **thermalizing (ETH) dynamics**, using a 6-qubit spin chain.

The work includes theoretical background, circuit-level quantum simulation using Qiskit, exact Hamiltonian evolution, and a detailed LaTeX report. This is intended as both a physics education tool and a research-grade benchmark for non-equilibrium quantum dynamics in NISQ systems.

---

## Overview

### What is Simulated?

We compare two driven quantum systems:

| Model              | Description |
|--------------------|-------------|
| **Floquet ETH**    | Thermalizing system with uniform transverse field and nearest-neighbor $$\( ZZ $$\) interactions. |
| **Floquet SPT-MBL**| Non-thermal system protected by disorder and $$\(\mathbb{Z}_2 \times \mathbb{Z}_2$$\) symmetry, exhibiting stable edge modes. |

Both systems are initialized in the same non-entangled product state and evolved stroboscopically.

---

### Key Observables

- \\( \langle Z_0(t) \rangle \\): Edge spin coherence
- \\( \langle Z_2(t) \rangle \\): Bulk spin behavior
- \\( S_0(t) \\): Single-qubit entanglement entropy

---

### Results Highlights

- **ETH system** shows rapid decay of local observables and volume-law entanglement.
- **SPT-MBL system** exhibits robust edge oscillations, suppressed entanglement growth, and localization-induced memory preservation.

---

## Contents

| File | Description |
|------|-------------|
| `floquet_spt_step.py` | Builds one Floquet step for the SPT-MBL circuit |
| `simulate_spt.py`     | Simulates 6-qubit Floquet SPT-MBL evolution using Qiskit |
| `simulate_eth.py`     | Simulates ETH model via exact matrix exponentiation |
| `report.pdf`          | Full LaTeX article comparing theory and simulation |
| `figures/`            | Simulation results and circuit diagrams |
| `README.md`           | This file |

---


