<div align="center">

# 🔐 Position: Embodied AI Requires a Privacy-Utility Tradeoff

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/rminshen03/EAI_Privacy_Position/graphs/commit-activity)

<h3 align="center">
  <!-- <strong>⭐ Official Repository for the SPINE Framework ⭐</strong> -->
</h3>

</div>

---

<p align="center">
  <b>🔥 This is the repository for evaluation and case studies of the submission: <br> "Position: Embodied AI Requires a Privacy-Utility Tradeoff".</b>
  <br><br>
  We propose <b>SPINE</b> (Secure Privacy Integration in Next-generation Embodied AI), 
  a unified privacy-aware framework that treats privacy as a dynamic control signal governing cross-stage coupling throughout the entire Embodied AI lifecycle. 
  <br><br>
  <!-- We will continue to <b>UPDATE</b> this repository with new resources and experimental data!  -->
</p>

---

## 🔍 Table of Contents
- [📖 1. Introduction](#1-introduction)
- [🏗️ 2. Taxonomy](#2-taxonomy)
- [💬 3. SPINE Framework Design](#3-spine-framework-design)
- [👁️ 4. Case Study](#4-case-study)
- [🔖 Citation](#-citation)

---

## 📖 1. Introduction <a name="1-introduction"></a>
Embodied AI (EAI) systems are rapidly transitioning from laboratory benchmarks to real-world domestic and occupational environments. However, existing solutions exclusively demonstrate advancements within isolated stages, which may create a systemic privacy crisis when prioritizing task utility at the expense of data privacy. We propose **SPINE**, a unified framework to navigate this fundamental tradeoff by integrating privacy-utility optimization throughout the agent's workflow.

---

## 🏗️ 2. Taxonomy <a name="2-taxonomy"></a>
Our evaluation framework categorizes EAI privacy into four interdependent stages that define the information flow of an embodied agent:
1. **Instruction Understanding**: Focuses on local sanitization of user commands and intent masking.
2. **Environment Perception**: Addresses source-level modality restrictions and anonymization techniques.
3. **Action Planning**: Incorporates privacy cost maps and trajectory privacy to protect user routines.
4. **Physical Interaction**: Ensures data minimality through in-memory execution and secure wipe protocols.

---

## 💬 3. SPINE Framework Design <a name="3-spine-framework-design"></a>
SPINE functions as a dynamic orchestration layer that adjusts the agent's computational behavior based on a detected privacy classification matrix ranging from L1 Public to L4 Restricted. Crucially, this tiered approach ensures that privacy constraints are enforced holistically, preventing systemic leakage caused by treating stages as isolated components.

---

## 👁️ 4. Case Study <a name="4-case-study"></a>

We perform a detailed case study on embodied navigation within the SPINE framework, evaluating a long-range navigation task transitioning from Public (L1) to Restricted (L4) zones.

### 4.1. Task Definition, Hypotheses & Results
<div align="center">
  <img src="assets/fig1.png" width="40%" alt="Task and Analysis"/>
  <br>
  <em>Fig. 1: (a) Task Definition; (b) Research Hypotheses (H1 & H2); (c) Qualitative Analysis & Explanation.</em>
</div>

* **H1: Semantic Compensation**: High-level intent serves as a semantic anchor, allowing the agent to maintain a baseline success rate even when visual data is sanitized.
* **H2: Heuristic Decoupling**: Loss of visual landmarks causes a logic break, forcing the navigation policy to regress from efficient heuristics into stochastic search patterns.
* **Key Findings**: In experimental scenarios, Success Rate (SR) decreased by 30.3%, while Success weighted by Path Length (SPL) plummeted by 43.3% in restricted settings.

### 4.2. Experimental Design（simulator & real-word） 
<div align="center">
  <img src="assets/fig2.png" width="85%" alt="Hardware and Environment"/>
  <br>
  <em>Fig. 2: Hardware platform (AgileX SCOUT MINI) and real-world quadrant deployment.</em>
</div>

* **Hardware Platform**: AgileX SCOUT MINI mobile base.
* **Sensing Suite**: Livox Mid-360 LiDAR for spatial mapping and RealSense Camera for visual input.
* **Computing Unit**: Jetson AGX Orin module for real-time inference and navigation control.
### 4.3. Demonstration Video (coming soon)

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
