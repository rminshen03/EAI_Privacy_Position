<div align="center">

# 🔐 EAI_Privacy_Position: Embodied AI Requires a Privacy-Utility Tradeoff

[![arXiv](https://img.shields.io/badge/arXiv-26XX.XXXXX-b31b1b.svg?logo=arxiv)](https://arxiv.org/abs/26XX.XXXXX)
[![GitHub stars](https://img.shields.io/github/stars/rminshen03/EAI_Privacy_Position?style=social)](https://github.com/rminshen03/EAI_Privacy_Position)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/rminshen03/EAI_Privacy_Position/graphs/commit-activity)

<h3 align="center">
  <strong>⭐ Official Repository for the SPINE Framework ⭐</strong>
</h3>

</div>

---

<p align="center">
  <b>🔥 Official resource hub for the position paper: "Embodied AI Requires a Privacy-Utility Tradeoff."</b>
  <br>
  This research introduces <b>SPINE (Secure Privacy Integration in Next-generation Embodied AI)</b>, 
  [cite_start]a unified framework designed to address the systemic privacy crisis in real-world Embodied AI deployments[cite: 62, 140].
  <br>
  We continuously update this repository with the latest research developments and experimental data!
</p>

---

## 📢 News

| Date | Event |
|:-----|:-----|
| 🔥 2026/01 | Paper submitted to **ICML 2026**; associated resources released. |
| 🚀 2026/01 | Repository `EAI_Privacy_Position` officially launched with SPINE framework documentation. |

---

## 🔍 Table of Contents

- [📖 1. Introduction](#1-introduction)
- [🏗️ 2. Taxonomy](#2-taxonomy)
- [💬 3. SPINE Framework Design](#3-spine-framework-design)
- [👁️ 4. Case Study](#4-case-study)
- [🔮 5. Challenges and Future Directions](#5-challenges-and-future-directions)
- [🔖 Citation](#-citation)

---

## 📖 1. Introduction <a name="1-introduction"></a>

[cite_start]Embodied AI (EAI) is rapidly transitioning from laboratory benchmarks to real-world domestic and occupational environments[cite: 59, 68]. [cite_start]However, existing solutions prioritize task utility at the expense of data privacy, leading to a systemic privacy crisis[cite: 61]. 

[cite_start]We argue that embodied privacy is a **fundamental tradeoff** that cannot be resolved by isolated "patches"; instead, it requires a new architectural paradigm that integrates privacy-utility optimization throughout the entire EAI lifecycle[cite: 73, 141].

---

## 🏗️ 2. Taxonomy <a name="2-taxonomy"></a>

Our evaluation framework for privacy-aware Embodied AI spans four critical phases:
1. **Instruction Understanding**: Focuses on privacy-preserving input and instruction safety.
2. **Environment Perception**: Addresses anonymization, adversarial defense, and efficiency.
3. **Action Planning**: Incorporates safety constraints and trajectory privacy.
4. **Physical Interaction**: Ensures reliability and prevents sensor data leakage during deployment.

*(Note: Taxonomy visualization diagram will be updated soon.)*

---

## 💬 3. SPINE Framework Design <a name="3-spine-framework-design"></a>

[cite_start]SPINE embeds privacy as a core primitive throughout the EAI workflow[cite: 62]:
1. [cite_start]**Instruction Understanding**: Local sanitization of sensitive entities (e.g., abstracting specific medication names)[cite: 253, 258].
2. [cite_start]**Environment Perception**: Source-level modality restrictions, triggering hardware-level visual cutoffs in restricted zones[cite: 259, 260].
3. [cite_start]**Action Planning**: Integration of "Privacy Cost Maps" to force trajectories to circumvent sensitive regions[cite: 255].
4. [cite_start]**Physical Interaction**: In-memory-only execution with secure wipe protocols triggered immediately upon task completion[cite: 262, 263].

---

## 👁️ 4. Case Study <a name="4-case-study"></a>

[cite_start]We perform a detailed case study on embodied navigation within the SPINE framework, evaluating a long-range navigation task transitioning from Public (L1) to Restricted (L4) zones[cite: 410, 451].

### 4.1. Task Definition, Hypotheses & Results
<div align="center">
  <img src="assets/fig1.png" width="80%" alt="Task and Analysis"/>
  <br>
  <em>Fig. 1: (a) Task Definition; (b) Research Hypotheses (H1 & H2); (c) [cite_start]Qualitative Analysis & Explanation[cite: 451, 453].</em>
</div>

* [cite_start]**H1: Semantic Compensation**: High-level intent serves as a semantic anchor, maintaining a baseline Success Rate (SR) even under perceptual degradation[cite: 457, 460].
* [cite_start]**H2: Heuristic Decoupling**: Loss of visual landmarks causes a logic break, forcing the agent to regress from efficient heuristics into stochastic search, declining navigation efficiency (SPL)[cite: 537].

### 4.2. Experimental Design & Hardware Configuration
<div align="center">
  <img src="assets/fig2.png" width="85%" alt="Hardware and Scenarios"/>
  <br>
  <em>Fig. [cite_start]2: Hardware platform (AgileX SCOUT MINI) and real-world quadrant deployment[cite: 533].</em>
</div>

* [cite_start]**Robot**: AgileX SCOUT MINI[cite: 415, 492].
* [cite_start]**Sensing Suite**: Livox Mid-360 LiDAR, RealSense Camera, and Jetson AGX Orin module[cite: 415, 466, 491].
* [cite_start]**Quantitative Findings**: In restricted settings, Success Rate (SR) decreased by 30.3%, while Success weighted by Path Length (SPL) plummeted by 43.3%[cite: 540].

---

## 🔮 5. Challenges and Future Directions <a name="5-challenges-and-future-directions"></a>

* [cite_start]**Cross-Stage Privacy Consistency**: Ensuring seamless propagation of privacy policies from instructions to physical actuation[cite: 711, 712].
* [cite_start]**Privacy-Utility Co-optimization**: Mapping the Pareto frontier to rigorously quantify the "cost of privacy"[cite: 716, 721].
* [cite_start]**HW/SW Co-design**: Accelerating edge-native encrypted computation to maintain physical agility[cite: 727, 730].

---

## 🔖 Citation <a name="-citation"></a>

If you find this work helpful, please consider citing our paper:

```bibtex
@misc{anonymous2026spine,
  title={Embodied AI Requires a Privacy-Utility Tradeoff},
  author={Anonymous Authors},
  year={2026},
  booktitle={Under review by ICML 2026},
  url={[https://github.com/rminshen03/EAI_Privacy_Position](https://github.com/rminshen03/EAI_Privacy_Position)},
}
