---
title: EW 仿真（EW Simulation）——建模、仿真与仿真注入
type: concept
concept_type: technology
tags: [concept, electronic-warfare, simulation, modeling, emulation, training, t-and-e]
aliases: [EW Simulation, EW 仿真, Modeling, Emulation, 建模仿真]
sources: [ew-101-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# EW 仿真（EW Simulation）

技术参考层页面。Adamy《EW 101》Ch11 关于 EW 仿真的**三种方法、仿真注入点、威胁信号仿真与保真度**
是可跨战争、跨装备复用的技术框架。本页汇总仿真方法学与工程要点，不作为具体历史事件的史料。

## 1. 定义与目的

仿真（simulation）＝**制造人为情形或激励，使操作员或 EW 设备以为存在一个或多个威胁信号、并
按其作战时的行为做出反应**。仿真常用于：**省钱**，以及评估**尚不存在的环境、装备与技术**。
通常包含随操作员/设备响应对仿真威胁的**交互式更新**。

## 2. 三种仿真方法（Simulation Approaches）

仿真分为三个子类；任何仿真或仿真注入都必须**基于 EW 系统与威胁环境相互作用的模型**：

1. **计算机仿真／建模（Computer Simulation / Modeling）**：在计算机中用数学模型让对象相互
   作用。**不产生信号或战术态势的“表示”**，适合**评估策略与战术**（比较不同方案）。比较评估
   必须在同一模型下进行。
2. **操作员界面仿真（Operator Interface Simulation，常简称“仿真”）**：生成**操作员显示**与
   控制交互。可由仿真计算机驱动系统显示器、读取开关量，从而让操作员面对模拟态势。
3. **仿真注入／仿真（Emulation）**：**实际系统的一部分在场**时使用。Emulation 以信号在
   **注入点处应有的形式**生成信号。注入点位置会影响到达注入点的信号，故须谨慎选择。

## 3. 仿真用途

- **训练仿真（Simulation for Training）**：让学员在安全环境（无需真飞）中体验真实作战情形；
  常与其他类型仿真合并（如“飞过敌电子环境”）。
- **装备测试与评估仿真（Simulation for T&E）**：使**被测试设备**以为它正在做真实工作，
  以考核系统。与训练仿真之别在于面向**被测系统**而非学员。
- **概念评估**：用建模比较策略/战术/技术方案。

## 4. 仿真注入点（Emulation Injection Points）

按注入位置由外到内一般有：**RF 注入 → IF 或视频注入 → 数字注入 → 数字显示数据注入**。
不同注入点各有**优缺点**（越靠外越真实但成本/复杂度越高；越靠内越易实现但丢失前端效应）。

## 5. 保真度（Fidelity）

保真度是选型/设计 EW 仿真的重要考量：所需保真度取决于**用途**（训练、T&E、概念评估对保真度
要求不同）；必须权衡成本/复杂度与所需真实程度。

## 6. 威胁仿真与天线方向图仿真

- **威胁仿真的类型**：脉冲雷达信号、通信信号等；**脉冲信号仿真**、**高保真脉冲仿真器**
  （parallel generators 并行发生器 / time-shared generators 时分发生器，含**脉冲丢失
  （pulse dropout）**问题，需**)主/备仿真器**）。
- **威胁天线方向图仿真**：仿真各类扫描型式——**圆周（circular）、扇扫（sector）、螺旋
  （helical）、光栅（raster）、圆锥（conical）、螺旋线（spiral）、Palmer、Palmer-raster、
  波瓣切换（lobe switching）、仅收波瓣（lobe-on receive only）、相控阵（phased array）、
  电子俯仰扫描＋机械方位扫描**等。
- **接收机仿真**：接收机功能、信号流、仿真器、信号强度仿真、处理器仿真。
- **天线仿真**：天线特性、抛物线天线示例、RWR 天线示例等。

## 7. 操作员界面仿真的工程考量

- **游戏区（gaming areas）**与**游戏区索引（gaming area indexing）**。
- **硬件异常（hardware anomalies）**、**处理时延（process latency）**。
- “够好即可吗（Is it good enough?）”——保真度与成本的判断。

## 8. 作战意义与研究价值

- 建模仿真方法论是 EW 训练、装备测试、战术评估的通用工具，跨战争与代际复用。
- 注入点分级与保真度权衡，为理解历史 EW 训练/试验体系（如埃格林电测-取证中心一类设施）提供
  框架。
- 与 [[ew-link-equation-and-db-math|球面三角]]（三维几何建模）、[[jamming|干扰]]（舰船防护仿真
  示例）互参。

## 关联

- 概念：[[ew-link-equation-and-db-math|链路方程与球面三角]]、[[jamming|干扰]]、[[radar-decoys|诱饵]]、
  [[ew-processing-and-threat-id|EW 处理]]
- 应用：[[redcap-ew-sim|REDCAP EW 仿真]]（库中既有）
- 来源：[[sources/ew-101-adamy|EW 101]]

## 资料来源

[[sources/ew-101-adamy|Adamy《EW 101》]] Ch11（仿真）。技术参考汇总，非史料。
