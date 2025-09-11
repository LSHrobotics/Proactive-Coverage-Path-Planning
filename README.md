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
This paper addresses the challenge of energy-aware multi-robot coverage path planning. Traditional reactive methods only trigger recharging when the battery level drops critically low, which often leads to inefficient routes or mission failure in sparse charging environments.
The proposed Globally Extended Routing (GER) method proactively integrates recharging decisions into the path generation process. By embedding charging stops within the coverage sequence, GER minimizes the overall mission time while ensuring that energy constraints are satisfied.

The following Figure illustrates the difference:
Black circles (N): coverage nodes, 
Green circles (C): charging stations, 
Dotted circles (Rs): sensing ranges, 

Reactive planning recharges late, whereas GER proactively plans recharging actions during route construction.

<img width="1054" height="337" alt="problem" src="https://github.com/user-attachments/assets/7f0227bc-1641-4ade-90a8-f736a925bfa5" />



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
In the demonstration video, the coverage mission time is accelerated by approximately 24× so that the mission completes within about one minute for visual clarity. 
In contrast, our paper reports the normalized mission times obtained from simulation. Especially, in the sparse charging-station case, our proposed GER achieves 1164.42 s, compared to 1431.33 s for ER and 1331.86 s for EVTSP, as described in Table 4. 

▶ Watch here: [YouTube Link](https://youtu.be/FFeNO_RdM2w)

---

```bibtex
@unpublished{Lee2025,
  author = {{Junghwan Gong, Moses O. Oluma, and Seunghwan Lee},
  title  = {Proactive Mission-Time-Efficient Coverage Path Planning Using Hierarchical Heuristics},
  note   = {Manuscript under review, 2025}
}

