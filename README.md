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
  <b>🔥 这是针对 "具身智能隐私-效用权衡" 立场论文的官方资源汇总。</b>
  <br>
  本研究提出了 <b>SPINE (Secure Privacy Integration in Next-generation Embodied AI)</b> 框架，
  [cite_start]旨在解决具身智能在真实场景部署中面临的系统性隐私危机 [cite: 62, 140]。
  <br>
  我们将持续更新最新的研究动态与实验数据！
</p>

---

## 📢 News

| 日期 | 动态 |
|:-----|:-----|
| 🔥 2026/01 | 论文提交至 **ICML 2026** 并开源相关资源。 |
| 🚀 2026/01 | 仓库 `EAI_Privacy_Position` 正式建立，更新 SPINE 框架说明。 |

---

## 🔍 目录 (Table of Contents)

- [📖 1. 引言 (Introduction)](#1-引言)
- [🏗️ 2. 隐私分类体系 (Taxonomy)](#2-隐私分类体系)
- [💬 3. SPINE 框架设计 (Position)](#3-spine-框架设计)
  - [L1-L4 隐私级别矩阵](#l1-l4-隐私级别矩阵)
  - [全生命周期治理](#全生命周期治理)
- [👁️ 4. 案例研究 (Case Study)](#4-案例研究)
  - [模拟器实验 (Val-Seen/UnSeen)](#模拟器实验)
  - [真实物理平台部署](#真实物理平台部署)
- [🔮 5. 挑战与未来方向](#5-挑战与未来方向)
- [🔖 引用 (Citation)](#-citation)

---

## 📖 1. 引言 (Introduction) <a name="1-引言"></a>

[cite_start]具身智能 (EAI) 正在迅速从实验室模拟环境向真实的家庭和办公环境转变 [cite: 59, 68][cite_start]。然而，现有的 EAI 解决方案在优先考虑任务效用时，往往会牺牲数据隐私，导致系统性的隐私危机 [cite: 61]。

[cite_start]我们认为，具身隐私是一个**权衡问题 (Tradeoff)**，不能仅仅通过局部补丁来解决，而需要一种全新的架构范式 [cite: 73, 141]。

---

## 🏗️ 2. 隐私分类体系 (Taxonomy) <a name="2-隐私分类体系"></a>

<div align="center">
  <img src="assets/taxonomy.png" width="95%" alt="Taxonomy"/>
  <br>
  <em>Fig. [cite_start]1: SPINE 框架评估体系，涵盖：指令理解、环境感知、动作规划及物理交互 [cite: 63, 172]。</em>
</div>

### 隐私分级矩阵 (Privacy Matrix)

| 级别 | 场景示例 | 权衡优先级 | 核心技术 | [cite_start]法律依据 [cite: 80, 272] |
|:------|:----------|:----------|:---------------------| :--- |
| **L1: Public** | 公园、公共街道 | 效用优先 | 通用 API、云端 LLM | N/A |
| **L2: Internal** | 办公走廊 | 平衡模式 | 数据脱敏、FL、TEE | GDPR Recital 26 |
| **L3: Confidential** | 私人客厅 | 隐私倾向 | MPC、差分隐私 | GDPR Art. 4 |
| **L4: Restricted** | 浴室、卧室 | 隐私优先 | 零知识证明、同态加密 | GDPR Art. 9 & 10 |

---

## 💬 3. SPINE 框架设计 (Position) <a name="3-spine-框架设计"></a>

[cite_start]SPINE 将隐私作为核心原语，贯穿 EAI 的整个生命周期 [cite: 62]：
1. [cite_start]**指令理解**：对敏感意图进行本地脱敏（如将特定药物名称抽象化）[cite: 253, 258]。
2. [cite_start]**环境感知**：实施源头限制，在受限区域触发硬件级视觉阻断 [cite: 259, 260]。
3. [cite_start]**动作规划**：引入“隐私成本地图”，使路径自动绕开敏感区域 [cite: 255]。
4. [cite_start]**物理交互**：采用内存即运行模式，任务完成后立即执行安全擦除协议 [cite: 262, 263]。

---

## 👁️ 4. 案例研究 (Case Study) <a name="4-案例研究"></a>

<div align="center">
  <img src="assets/overview.png" width="90%" alt="Case Study Overview"/>
  <br>
  <em>Fig. [cite_start]2: 远距离导航任务定义：从公开区域 (L1) 到受限区域 (L4) [cite: 410, 451]。</em>
</div>

### 实验结果分析
[cite_start]我们提出了两个核心假设并得到了验证 [cite: 403, 404]：
* [cite_start]**H1: 语义补偿 (Semantic Compensation)**：高层意图锚点允许智能体在视觉受损时仍维持基础成功率 (SR) [cite: 457, 460]。
* [cite_start]**H2: 启发式解耦 (Heuristic Decoupling)**：严格的隐私保护会导致路径效率 (SPL) 显著下降（SR 下降 30.3%，而 SPL 下降达 43.3%）[cite: 537, 540]。

### 真实物理平台部署
* [cite_start]**机器人**: AgileX SCOUT MINI [cite: 415, 492]
* [cite_start]**感知**: Livox Mid-360 LiDAR & RealSense Camera [cite: 415, 466]
* [cite_start]**计算**: Jetson AGX Orin [cite: 415, 491]

---

## 🔮 5. 挑战与未来方向 <a name="5-挑战与未来方向"></a>

* [cite_start]**跨阶段隐私一致性**：确保隐私政策从指令到物理执行的一致传播 [cite: 711, 712]。
* [cite_start]**隐私-效用协同优化**：寻找 Pareto 前沿，定量评估隐私成本 [cite: 716, 721]。
* [cite_start]**硬件-软件协同设计**：加速边缘端的加密计算，以保证物理敏捷性 [cite: 727, 730]。

---

## 🔖 引用 (Citation) <a name="-citation"></a>

如果您发现本研究对您有帮助，请考虑引用我们的论文：

```bibtex
@misc{anonymous2026spine,
  title={Embodied AI Requires a Privacy-Utility Tradeoff},
  author={Anonymous Authors},
  year={2026},
  booktitle={Under review by ICML 2026},
  url={[https://github.com/rminshen03/EAI_Privacy_Position](https://github.com/rminshen03/EAI_Privacy_Position)},
}
