# Proactive Mission-Time-Efficient Coverage Path Planning Using Hierarchical Heuristics

---

## 🔎 **Overview**
**Overall Framework**  
<img width="2916" height="538" alt="overall_structure5" src="https://github.com/user-attachments/assets/bc1bfbcf-906d-4f15-9132-9cfb7c87f10c" />


*Figure 1. Flowchart of the proposed energy-aware CPP framework. The process starts with map generation and ACO-based path planning. Redundant nodes are inserted to reflect energy constraints, and a GA schedules recharging stops to minimize mission time.*

This repository provides a **summary and visual materials** of our work:  
**"Proactive Mission-Time-Efficient Coverage Path Planning Using Hierarchical Heuristics"**  
(*Under Review, 2025*)  

The proposed framework combines:  
- **Ant Colony Optimization (ACO)** for coverage path generation  
- **Genetic Algorithm (GA)** for proactive charging scheduling  

By integrating charging decisions in advance, the method achieves up to **24.66% mission time reduction**, especially in sparse charging environments.

---

## 🚀 **Key Contributions**
- **Proactive Planning**: Plans charging stops before the battery reaches critical levels.  
- **Hierarchical Heuristic**: ACO ensures efficient path ordering, GA refines charging schedules.  
- **Efficiency Gains**: Demonstrated significant mission-time reduction in synthetic, real-world, and Antarctica-based environments.  

---

## ⚡ **Problem Description**
<img width="1054" height="337" alt="problem" src="https://github.com/user-attachments/assets/7f0227bc-1641-4ade-90a8-f736a925bfa5" />

*Figure 2. Comparison between reactive and proactive (GER) energy-aware planning. Black circles: coverage nodes (N); green circles: charging stations (C); dotted circles: sensing range (Rs). Unlike reactive methods that recharge only at low battery, GER proactively integrates charging stops into path planning.*

---

## 📊 **Results**

### 🔹 **Simulation Comparisons**
Comparison of four methods in a synthetic coverage environment:  
- **NCPP**: Ignores charging, fails due to battery depletion.  
- **ER**: Charges only when nearly depleted, leading to late detours.  
- **EVTSP**: Minimizes travel time but still charges reactively.  
- **GER (Proposed)**: Proactively schedules charging, avoiding long detours and reducing mission time.  

<img width="514" height="585" alt="sim-results" src="https://github.com/user-attachments/assets/3115ab32-519d-425c-b4df-687d1833ae6b" />

---

### 🔹 **Battery Profiles**
GER maintains safer margins by recharging earlier, avoiding critical depletion and reducing mission time.  

<img width="525" height="128" alt="battery" src="https://github.com/user-attachments/assets/b567a4d0-4898-487c-9d1f-f5ae162ac519" />

---

### 🔹 **Mission Time Comparison**
Total mission time (*T(Q\*)*) for NCPP, ER, EVTSP, and GER in a real-world-acquired environment.  
GER shows the shortest mission times across all charging station densities.  

<img width="537" height="87" alt="mission-time" src="https://github.com/user-attachments/assets/3a9992ea-5cdc-4abe-b494-92213fbb9e5d" />

---

## 🎥 Demonstration
Short demo GIF (simulation-based):

![Demo GIF](videos/demo.gif)

---

## 📂 Repository Structure
