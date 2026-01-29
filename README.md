<div align="center">

# 🔐 Position: Embodied AI Requires a Privacy-Utility Tradeoff

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
  <b>🔥 This is a curated paper list for "Position: Embodied AI Requires a Privacy-Utility Tradeoff."</b>
  <br>
  [cite_start]To the best of our knowledge, this is the <b>first comprehensive study</b> on privacy-utility tradeoffs in Embodied AI (EAI) systems [cite: 61, 73][cite_start], covering the entire lifecycle across four critical stages: <b>Instruction Understanding</b>, <b>Environment Perception</b>, <b>Action Planning</b>, and <b>Physical Interaction</b>[cite: 60, 63, 151].
  <br>
  We will continue to <b>UPDATE</b> this repository! 
</p>

---

## 📢 News

| Date | Event |
|:-----|:-----|
| 🚀 2026/01 | Repository officially launched with **SPINE** framework documentation. |

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
[cite_start]Embodied AI (EAI) systems are rapidly transitioning from laboratory benchmarks to real-world domestic and occupational environments[cite: 59, 68]. [cite_start]However, existing solutions exclusively demonstrate advancements within isolated stages, which may create a systemic privacy crisis when prioritizing task utility at the expense of data privacy[cite: 60, 61]. [cite_start]We propose **SPINE** (Secure Privacy Integration in Next-generation Embodied AI), a unified framework to navigate this fundamental tradeoff[cite: 62, 140].

---

## 🏗️ 2. Taxonomy <a name="2-taxonomy"></a>
[cite_start]Our evaluation framework categorizes EAI privacy into four interdependent stages[cite: 63, 172]:
1. [cite_start]**Instruction Understanding**: Privacy-preserving input and semantic masking[cite: 253, 258].
2. [cite_start]**Environment Perception**: Anonymization and source-level modality restrictions[cite: 259, 260].
3. [cite_start]**Action Planning**: Safety-aware navigation and trajectory privacy[cite: 255].
4. [cite_start]**Physical Interaction**: In-memory execution and secure wipe protocols[cite: 262, 263].

---

## 👁️ 4. Case Study <a name="4-case-study"></a>

[cite_start]We perform a detailed case study on embodied navigation within the SPINE framework, evaluating a long-range navigation task transitioning from Public (L1) to Restricted (L4) zones[cite: 343, 401, 410].

### 4.1. Task Definition, Hypotheses & Results
<div align="center">
  <img src="assets/fig1.png" width="40%" alt="Task and Analysis"/>
  <br>
  <em>Fig. 1: (a) Task Definition; (b) Research Hypotheses (H1 & H2); (c) [cite_start]Qualitative Analysis & Explanation[cite: 344, 451, 453].</em>
</div>

* [cite_start]**H1: Semantic Compensation**: High-level intent serves as a semantic anchor, allowing the agent to maintain a baseline success rate even with limited visual input[cite: 457, 460].
* [cite_start]**H2: Heuristic Decoupling**: Loss of visual landmarks causes a logic break, forcing the agent to regress from efficient heuristics into stochastic search patterns[cite: 536, 537].
* [cite_start]**Key Findings**: In experimental scenarios, Success Rate (SR) decreased by 30.3%, while Success weighted by Path Length (SPL) plummeted by 43.3%[cite: 540].

### 4.2. Experimental Design & Hardware Configuration
<div align="center">
  <img src="assets/fig2.png" width="85%" alt="Hardware and Environment"/>
  <br>
  <em>Fig. [cite_start]2: Hardware platform (AgileX SCOUT MINI) and real-world quadrant deployment[cite: 415, 533].</em>
</div>

* [cite_start]**Hardware Platform**: AgileX SCOUT MINI[cite: 415, 492].
* [cite_start]**Sensing Suite**: Livox Mid-360 LiDAR [cite: 415, 466][cite_start], RealSense Camera [cite: 415, 470][cite_start], and Jetson AGX Orin module[cite: 415, 491].

---

## 🔖 Citation <a name="-citation"></a>
```bibtex
@misc{anonymous2026spine,
  title={Position: Embodied AI Requires a Privacy-Utility Tradeoff},
  author={Anonymous Authors},
  year={2026},
  booktitle={Under Review},
  url={[https://github.com/rminshen03/EAI_Privacy_Position](https://github.com/rminshen03/EAI_Privacy_Position)},
}
