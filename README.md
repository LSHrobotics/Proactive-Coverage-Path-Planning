# Proactive-Coverage-Path-Planning
A hierarchical heuristic framework (ACO + GA) for proactive, mission-time-efficient coverage path planning under battery constraints. Includes results, figures, and demo videos.
# Proactive Mission-Time-Efficient Coverage Path Planning Using Hierarchical Heuristics

[![Paper](https://img.shields.io/badge/Paper-PDF-blue)](링크-추가)
[![Video Demo](https://img.shields.io/badge/Video-Demo-red)](링크-추가)

---

## 🔎 Overview
This repository introduces the paper:

**"Proactive Mission-Time-Efficient Coverage Path Planning Using Hierarchical Heuristics"**  
*Junghwan Gong, Moses O. Oluma, Seunghwan Lee (Kumoh National Institute of Technology)*  

The study presents a **hierarchical heuristic framework** for coverage path planning (CPP) under energy constraints.  
Unlike conventional reactive methods, our approach proactively schedules charging actions, reducing mission time by up to **24.66%** in sparse charging environments.

---

## 🚀 Key Contributions
- **Proactive Planning**: Charging actions are scheduled in advance to avoid mission failure.  
- **Hierarchical ACO + GA**: Combines Ant Colony Optimization (ACO) for path generation and a Genetic Algorithm (GA) for charging scheduling.  
- **Validated Efficiency**: Consistent mission-time reduction across synthetic, real-world, and Antarctica-inspired environments.  

---

## 📊 Results
### Mission Time Reduction
<img src="figures/result_comparison.png" width="600">

- Up to **24.66% shorter mission time** compared to reactive methods.  
- Significant improvements in environments with sparse charging stations.  

### Battery Profile
<img src="figures/battery_profile.png" width="600">

- GER maintains safer energy margins by recharging earlier.  
- Avoids late detours and ensures mission reliability.  

---

## 🎥 Demonstration
Here is a short demo video comparing **Reactive vs GER (Proposed Method):**

![Demo GIF](videos/demo.gif)

👉 [Full Demo on YouTube](https://youtube.com/링크-추가)

---

## 📂 Repository Structure
