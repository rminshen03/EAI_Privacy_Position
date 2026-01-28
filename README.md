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
  - [L1-L4 Privacy Classification Matrix](#l1-l4-privacy-classification-matrix)
  - [Full Lifecycle Governance](#full-lifecycle-governance)
- [👁️ 4. Case Study](#4-case-study)
  - [Simulation Results (Val-Seen/UnSeen)](#simulation-results)
  - [Real-world Physical Deployment](#real-world-deployment)
- [🔮 5. Challenges and Future Directions](#5-challenges-and-future-directions)
- [🔖 Citation](#-citation)

---

## 📖 1. Introduction <a name="1-introduction"></a>

[cite_start]Embodied AI (EAI) is rapidly transitioning from laboratory benchmarks to real-world domestic and occupational environments[cite: 59, 68]. [cite_start]However, existing solutions prioritize task utility at the expense of data privacy, leading to a systemic privacy crisis[cite: 61]. 

[cite_start]We argue that embodied privacy is a **fundamental tradeoff** that cannot be resolved by isolated "patches"; instead, it requires a new architectural paradigm that integrates privacy-utility optimization throughout the entire EAI lifecycle[cite: 73, 141].

---

## 🏗️ 2. Taxonomy <a name="2-taxonomy"></a>

<div align="center">
  <img src="assets/taxonomy.png" width="95%" alt="Taxonomy"/>
  <br>
  <em>Fig. [cite_start]1: The SPINE evaluation framework across four phases: Instruction Understanding, Environment Perception, Action Planning, and Physical Interaction[cite: 63, 172].</em>
</div>

### Privacy Classification Matrix

| Level | Scenario Example | Trade-off Priority | Key Techniques | [cite_start]Legal Basis [cite: 80, 272] |
|:------|:----------|:----------|:---------------------| :--- |
| **L1: Public** | Parks, public streets | Utility First | Public Models, Universal APIs | N/A |
| **L2: Internal** | Office corridors | Balanced | Data Anonymization, FL, TEE | GDPR Recital 26 |
| **L3: Confidential** | Private living rooms | Privacy-Leaning | MPC, Differential Privacy | GDPR Art. 4 |
| **L4: Restricted** | Bathrooms, bedrooms | Privacy First | Zero-Knowledge Proof, FHE | GDPR Art. 9 & 10 |

---

## 💬 3. SPINE Framework Design <a name="3-spine-framework-design"></a>

[cite_start]SPINE embeds privacy as a core primitive throughout the EAI workflow[cite: 62]:
1. [cite_start]**Instruction Understanding**: Local sanitization of sensitive entities (e.g., abstracting specific medication names)[cite: 253, 258].
2. [cite_start]**Environment Perception**: Source-level modality restrictions, triggering hardware-level visual cutoffs in restricted zones[cite: 259, 260].
3. [cite_start]**Action Planning**: Integration of "Privacy Cost Maps" to force trajectories to circumvent sensitive regions[cite: 255].
4. [cite_start]**Physical Interaction**: In-memory-only execution with secure wipe protocols triggered immediately upon task completion[cite: 262, 263].

---

## 👁️ 4. Case Study <a name="4-case-study"></a>

<div align="center">
  <img src="assets/overview.png" width="90%" alt="Case Study Overview"/>
  <br>
  <em>Fig. [cite_start]2: Long-range navigation task definition: Transitioning from Public (L1) to Restricted (L4) zones[cite: 410, 451].</em>
</div>

### Experimental Qualitative Analysis
[cite_start]We formulated and validated two primary research hypotheses[cite: 403, 404]:
* [cite_start]**H1: Semantic Compensation**: High-level intent serves as a semantic anchor, maintaining a baseline Success Rate (SR) even under perceptual degradation[cite: 457, 460].
* [cite_start]**H2: Heuristic Decoupling**: Stringent privacy constraints lead to a logic break between perception and planning, sharply declining navigation efficiency (SPL)[cite: 537]. 
  * [cite_start]*Results*: SR decreased by 30.3%, while SPL plummeted by 43.3% in restricted settings[cite: 540].

### Hardware Configuration
* [cite_start]**Robot**: AgileX SCOUT MINI [cite: 415, 492]
* [cite_start]**Sensing**: Livox Mid-360 LiDAR & RealSense Camera [cite: 415, 466]
* [cite_start]**Computing**: Jetson AGX Orin [cite: 415, 491]

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
