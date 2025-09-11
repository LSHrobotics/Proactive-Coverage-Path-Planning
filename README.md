# **Proactive Mission-Time-Efficient Coverage Path Planning Using Hierarchical Heuristics**

---

## 🔎 Overall Framework
<img width="2916" height="538" alt="overall_structure5" src="https://github.com/user-attachments/assets/bc1bfbcf-906d-4f15-9132-9cfb7c87f10c" />

*Figure 1. Flowchart of the proposed energy-aware CPP framework. The process begins with map generation and ACO-based path planning. Redundant nodes are then inserted to account for energy constraints, and a GA refines the solution by scheduling proactive recharging stops to minimize total mission time.*

This repository provides supplementary materials and visualizations for our study:  
**"Proactive Mission-Time-Efficient Coverage Path Planning Using Hierarchical Heuristics"**  
(*Under Review, 2025*)  

The proposed framework integrates:  
- **Ant Colony Optimization (ACO)** for initial coverage path construction  
- **Genetic Algorithm (GA)** for proactive recharging optimization  

By embedding charging decisions into the planning stage, the method achieves up to **24.66% mission-time reduction**, particularly in sparse charging environments.

---

## 🚀 Key Contributions
- **Proactive Charging Strategy**: Incorporates recharge stops before the battery reaches critical levels.  
- **Hierarchical Heuristic Framework**: ACO ensures effective path ordering; GA optimizes the recharging schedule.  
- **Robust Efficiency Gains**: Validated across synthetic layouts, real-world-acquired environments, and an Antarctica-based case study.  

---

## ⚡ Problem Description
<img width="1054" height="337" alt="problem" src="https://github.com/user-attachments/assets/7f0227bc-1641-4ade-90a8-f736a925bfa5" />

*Figure 2. Reactive vs. proactive (GER) energy-aware planning. Black circles: coverage nodes (N); green circles: charging stations (C); dotted circles: sensing range (Rs). Unlike reactive methods that recharge only at low battery levels, GER proactively integrates recharging decisions into the coverage path.*

---

## 📊 Results

### 🔹 Simulation Comparisons
Evaluation of four methods in a synthetic coverage environment:  
- **NCPP**: No charging consideration, fails due to depletion.  
- **ER**: Reactive charging when nearly empty, causing detours.  
- **EVTSP**: Improves travel efficiency but still reactive in charging.  
- **GER (Proposed)**: Proactive charging integration, avoiding unnecessary detours and reducing mission time.  

<img width="514" height="585" alt="sim-results" src="https://github.com/user-attachments/assets/3115ab32-519d-425c-b4df-687d1833ae6b" />

---

### 🔹 Battery Profiles
GER sustains safer energy margins by scheduling earlier recharges, avoiding critical depletion and reducing mission delays.  

<img width="525" height="128" alt="battery" src="https://github.com/user-attachments/assets/b567a4d0-4898-487c-9d1f-f5ae162ac519" />

---

### 🔹 Mission Time Comparison
Total mission time (*T(Q\*)*) of NCPP, ER, EVTSP, and GER in real-world-acquired environments.  
GER consistently achieves the **lowest mission times across charging station densities**.  

<img width="537" height="87" alt="mission-time" src="https://github.com/user-attachments/assets/3a9992ea-5cdc-4abe-b494-92213fbb9e5d" />

---

## 🎥 Demo Video
For demonstration, the coverage mission time is accelerated by ~23× to fit within one minute.  
In the paper, actual mission times align with **Table 4** results.  

▶ Watch here: [YouTube Link](https://youtu.be/FFeNO_RdM2w)

---

@unpublished{Lee2025,
  author = {Junghwan Gong, Moses O. Oluma, and Seunghwan Lee},
  title  = {Proactive Mission-Time-Efficient Coverage Path Planning Using Hierarchical Heuristics},
  note   = {Manuscript under review, 2025}
}

## 📖 How to Cite
If you find this work useful, please cite it as:

```bibtex
@unpublished{Lee2025,
  author = {Seunghwan Lee and Coauthors},
  title  = {Proactive Mission-Time-Efficient Coverage Path Planning Using Hierarchical Heuristics},
  note   = {Manuscript under review, 2025}
}

