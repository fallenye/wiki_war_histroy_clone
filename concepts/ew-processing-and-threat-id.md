---
title: EW 处理与威胁识别（EW Processing & Threat Identification）
type: concept
concept_type: technology
tags: [concept, electronic-warfare, esm, signal-processing, threat-id, operator-interface]
aliases: [EW Processing, 威胁识别, Threat Identification, Deinterleaving, 去交错]
sources: [ew-101-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# EW 处理与威胁识别

技术参考层页面。Adamy《EW 101》Ch5 所述接收机之后的**信号处理链**与**人机界面**，是可跨战争、
跨装备复用的处理框架。本页汇总处理任务、参数测量、去交错（deinterleaving）与人机界面要点，
不作为具体历史事件的史料。

## 1. 处理任务与 RF 威胁识别逻辑

EW 处理的核心是把接收到的脉冲流对照**威胁库**判定“这是什么辐射源”。逻辑流为：提取每个脉冲
的参数 → 与已知威胁参数比对 → 识别类型。需要测定的主要参数：

- **脉宽（Pulse Width）**
- **频率（Frequency）**
- **到达方向（Direction of Arrival, DOA）**
- **脉冲重复间隔（Pulse Repetition Interval, PRI）**
- **天线扫描（Antenna Scan）**特征（扫描型式和速率是威胁识别的重要线索）

## 2. 去交错（Deinterleaving）

真实环境中一部接收机会**同时收到多部辐射源的脉冲交织**，必须先按来源分组：

- **Pulse on pulse**：两脉冲时间上重叠（因不同辐射源独立发脉冲而常见），给分组带来困难。
- **去交错工具**：以 PRI、频率、DOA、脉宽、扫描等参数的**一致性**把脉冲分到各辐射源。DOA 常
  是最有力的区分维度（不同方位即不同辐射源）。
- 数字接收机为去交错提供更强算力支持；处理结果与操作员界面耦合。

## 3. 人机界面（Operator Interface）

- **计算机 vs 人的分工**：自动处理需要更高的 SNR（比训练有素的操作员目视检测/手控跟踪要求更
  高）；自动处理适合高速大量脉冲，人则在模糊/异常情形介入。
- **一体化机载 EW 套件**的界面；现代机载界面形态：
  - **图像式显示（Pictorial Format Displays）**
  - **平视显示器（Head-Up Display, HUD）**：威胁符号按三维观测角摆位（见
    [[ew-link-equation-and-db-math|链路方程页]]的球面三角应用）。
  - **垂直态势显示器（Vertical-Situation Display）**
  - **水平态势显示器（Horizontal-Situation Display）**
  - **多用途显示器（Multiple-Purpose Displays）**
- **操作员职能与三角定位（triangulation）实战**：战术 ESM 系统的操作员依据截获的 DOA 做测向
  交汇定位；地图化现代显示帮助把多站 DOA 合成目标位置。

## 4. 作战意义与研究价值

- “接收→测参→去交错→对照威胁库→告警/记录”的处理链，是理解 RWR/ESM 行为、以及历史上告警
  系统局限（虚警、漏警、密集环境饱和）的通用框架。
- DOA＋PRI＋频率参数组与去交错思想，直接支撑 [[emitter-location|辐射源定位]] 中对同源信号的
  分选与识别需求。
- 人机界面的 HUD 符号摆位与三维观测角计算，连接 [[ew-link-equation-and-db-math|球面三角]]，
  是座舱告警设计的数学基础。

## 关联

- 概念：[[ew-receiver-architecture|EW 接收机]]、[[emitter-location|辐射源定位]]、
  [[ew-link-equation-and-db-math|链路方程与 dB 数学]]、[[ew-simulation|EW 仿真]]
- 应用：[[apr-25-26-rhaw|AN/APR-25/26 RHAW]]、[[ec-121-warning-star|EC-121]]、
  [[rb-66c-elint|RB-66C]]、[[sigint|SIGINT]]
- 来源：[[sources/ew-101-adamy|EW 101]]

## 资料来源

[[sources/ew-101-adamy|Adamy《EW 101》]] Ch5（EW 处理）。技术参考汇总，非史料。
