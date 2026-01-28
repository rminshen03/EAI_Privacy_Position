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
  <b>🔥 This is a curated paper list for "Embodied AI Requires a Privacy-Utility Tradeoff".</b>
  <br>
  [cite_start]To the best of our knowledge, this is the <b>first comprehensive study</b> on privacy-utility tradeoffs in Embodied AI systems, covering the entire lifecycle across four critical stages: <b>Instruction Understanding</b>, <b>Environment Perception</b>, <b>Action Planning</b>, and <b>Physical Interaction</b>[cite: 60, 151].
  <br>
  We will continue to <b>UPDATE</b> this repository! 
</p>

---

## 📢 News

| Date | Event |
|:-----|:-----|
| 🔥 2026/01 | Paper submitted to **ICML 2026**; associated resources released. |
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
[cite_start]Embodied AI (EAI) systems are rapidly transitioning from laboratory benchmarks to real-world domestic and occupational environments[cite: 59, 68]. [cite_start]However, existing solutions often prioritize task utility at the expense of data privacy, leading to a systemic privacy crisis[cite: 61]. [cite_start]We propose **SPINE** (Secure Privacy Integration in Next-generation Embodied AI), a unified framework to navigate this fundamental tradeoff[cite: 62, 140].

---

## 🏗️ 2. Taxonomy <a name="2-taxonomy"></a>
Our evaluation framework categorizes EAI privacy into four interdependent stages:
1. **Instruction Understanding**: Privacy-preserving input and semantic masking.
2. **Environment Perception**: Anonymization and source-level modality restrictions.
3. **Action Planning**: Safety-aware navigation and trajectory privacy.
4. **Physical Interaction**: In-memory execution and secure wipe protocols.

---

## 💬 3. SPINE Framework Design <a name="3-spine-framework-design"></a>
[cite_start]SPINE functions as a dynamic orchestration layer that adjusts the agent's behavior based on a detected privacy classification matrix (L1 to L4)[cite: 238]. [cite_start]It ensures that privacy constraints are enforced holistically across the entire lifecycle, preventing systemic leakage from fragmented components[cite: 238].

---

## 👁️ 4. Case Study <a name="4-case-study"></a>

[cite_start]We evaluate the privacy-utility tradeoff through a long-range navigation task transitioning from Public (L1) to Restricted (L4) zones[cite: 401, 410].

### 4.1. Task Definition, Hypotheses & Results
<div align="center">
  <img src="assets/fig1.png" width="40%" alt="Task and Analysis"/>
  <br>
  <em>Fig. 1: (a) Task Definition; (b) Research Hypotheses (H1 & H2); (c) [cite_start]Qualitative Analysis[cite: 344].</em>
</div>

* **H1: Semantic Compensation**: [cite_start]High-level goals from Stage I act as a semantic anchor, maintaining task success rate (SR) even when visual data is sanitized in Stage II[cite: 459, 460].
* **H2: Heuristic Decoupling**: [cite_start]Extreme perceptual loss at high privacy levels fractures the coupling between perception and planning, causing a sharp decline in efficiency (SPL)[cite: 535, 537].

### 4.2. Experimental Design & Hardware Configuration
<div align="center">
  <img src="assets/fig2.png" width="85%" alt="Hardware and Environment"/>
  <br>
  <em>Fig. [cite_start]2: Simulated environment, AgileX SCOUT MINI hardware, and real-world testbed[cite: 533].</em>
</div>

* **Hardware Platform**: [cite_start]AgileX SCOUT MINI equipped with Livox Mid-360 LiDAR, RealSense Camera, and Jetson AGX Orin[cite: 415, 492].
* **Quantitative Findings**: [cite_start]In Val-Seen scenarios, SR decreased by 30.3%, while SPL fell significantly by 43.3%[cite: 540].

---

## 🔮 5. Challenges and Future Directions <a name="5-challenges-and-future-directions"></a>
* [cite_start]**Cross-Stage Consistency**: Transitioning from localized patches to global protocols[cite: 712].
* [cite_start]**Co-optimization**: Mapping the Pareto frontier between performance and the "cost of privacy"[cite: 721].
* [cite_start]**Infrastructure**: Hardware-software co-design for secure, low-latency edge inference[cite: 730].

---

## 🔖 Citation <a name="-citation"></a>
```bibtex
@misc{anonymous2026spine,
  title={Embodied AI Requires a Privacy-Utility Tradeoff},
  author={Anonymous Authors},
  year={2026},
  booktitle={Under review by ICML 2026},
  url={[https://github.com/rminshen03/EAI_Privacy_Position](https://github.com/rminshen03/EAI_Privacy_Position)},
}
