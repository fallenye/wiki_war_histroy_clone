---
title: 电子战技术基础（跨战争专题）
type: topic
tags: [topic, electronic-warfare, technical-reference, ew-theory, concepts]
aliases: [EW Technical Foundations, 电子战技术基础, EW 理论层]
sources: [ew-101-adamy, ew-102-adamy, ew-103-adamy, ew-104-adamy, ew-105-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# 电子战技术基础（跨战争专题）

本专题页是知识库的**电子战技术概念层入口**：把不依附于任何单一战争、可跨战争与跨装备复用的
电子战**原理、分类、参数关系与公式**组织成一张网。它与本库既有的**历史叙事/装备线**
（[[electronic-warfare-in-ww2|二战电子战]]、[[electronic-warfare-cold-war-1946-64|电子战·冷战早期]]、
[[sead|SEAD/DEAD]] 等）互补：历史线回答“谁在何时何地用何装备做了什么”，本专题回答“电子战作为
技术体系如何运作、参数如何定量关联”。

主要技术参考来源：[[sources/ew-101-adamy|David Adamy《EW 101: A First Course in Electronic
Warfare》(Artech House, 2001)]]、[[sources/ew-102-adamy|《EW 102: A Second Course in Electronic
Warfare》(Artech House, 2004)]]、[[sources/ew-103-adamy|《EW 103: Tactical Battlefield
Communications EW》(Artech House, 2009)]] 与 [[sources/ew-104-adamy|《EW 104: EW Against a New
Generation of Threats》(Artech House, 2015)]]、[[sources/ew-105-adamy|《EW 105: Space Electronic
Warfare》(Artech House, 2021)]]（EW 100 系列五册；均按**技术参考资料模式**摄入，仅取技术概念/分类/
公式，不取史料）。

## 概念/条令层

- [[spectrum-warfare-ems|频谱战（Spectrum Warfare / EMS Warfare）]]——EMS 作为第五作战域、连通性、
  网络中心战、传输安全 vs 消息安全、赛博战 vs EW、隐写术、链路干扰与抗干扰。
- [[electronic-support-vs-sigint|电子支援 vs 信号情报（ES vs SIGINT）]]——ES/SIGINT 定位差异、
  COMINT/ELINT、天线/距离/接收机/搜索/处理技术差异。

## 分析底座

- [[ew-link-equation-and-db-math|电子战链路方程与 dB 数学基础]]——dB 运算、单向链路方程、扩散/
  大气损耗、接收灵敏度与有效距离、雷达距离方程的“链路化”、干扰信号差、球面三角与多普勒/观测角。
  这是其余各页的数学底座。

## 威胁与信号源

- [[ew-threats-and-guidance|EW 威胁与制导方式]]——威胁类型、四类制导方式（主动/半主动/指令/被动）、
  频段体系（科学/元件/雷达三套划分）、威胁雷达扫描与调制特征、通信信号威胁。
- [[radar-characteristics|雷达特征]]——雷达功能与分类、雷达距离方程三形式+dB 形式、脉冲调制与
  脉冲压缩、CW/脉冲多普勒/MTI/SAR。
- [[lpi-radar|低截获概率雷达（LPI 雷达）]]——LPI 三途径与三层级、LPID/安静/随机信号雷达、图数。
- [[radar-electronic-protection|雷达电子防护（EP）]]——新一代威胁雷达的 EP 技术（超低旁瓣、旁瓣
  对消/匿隐、单脉冲、抗交叉极化、脉冲压缩、PD 雷达 EP、频率捷变、PRF 抖动、寻的干扰）及各能力的
  EW 影响；威胁系统升级（据开放源）。
- [[infrared-electro-optical-ew|红外与光电 EW]]——IR 频谱/黑体辐射、IR 制导导弹与导引头/调制盘、
  IRLS、FLIR/IRST、夜视、激光指示/告警、IRCM（含照明弹战术、跟踪器、激光干扰机）。

## 系统链（从天线到处理）

- [[ew-antenna-parameters|EW 天线参数与选型]]——波束定义、增益-波束-面积关系、极化技巧、
  天线类型选型、抛物面权衡、相控阵。
- [[ew-receiver-architecture|EW 接收机体制分类]]——九类接收机及能力矩阵、宽带瞬时 vs 窄带选择。
- [[ew-processing-and-threat-id|EW 处理与威胁识别]]——威胁识别逻辑、参数测量、去交错、人机界面。
- [[emitter-location|辐射源定位与测向]]——定位目的与精度、精度预算、测向/定位技术（幅度、
  Watson-Watt、干涉仪、多普勒、TOA/TDOA）。
- [[emitter-location-accuracy|辐射源定位系统精度]]——RMS/CEP/EEP 度量、误差预算与合成、
  TDOA/FDOA 精确定位。

## 对抗（ECM）与反制

- [[jamming|干扰（J/S 与烧穿）]]——干扰四分类、J/S 方程、烧穿距离、覆盖/欺骗干扰、对单脉冲雷达
  的欺骗手法；雷达干扰技术分类（阻塞/点/扫频点/欺骗）。
- [[digital-rf-memory|数字射频存储（DRFM）]]——DRFM 原理与宽带/窄带体制、相干干扰、对脉冲压缩/
  频率捷变/前沿跟踪的对抗、复杂假目标、时延问题——新一代干扰的核心技术。
- [[radar-decoys|雷达诱饵]]——诱饵类型与三任务、RCS 与反射功率、被动/主动诱饵、交战中的有效 RCS。
- [[lpi-signals|低截获概率信号（LPI，通信侧）]]——LPI 基本手段、跳频/chirp/直接序列扩频及攻防。
- [[ew-against-communications|对通信信号的电子战]]——HF/VHF/UHF 传播模型（自由空间/双径/刀边）、
  背景噪声、数字通信（调制/BER/带宽）、通信干扰、对扩频信号的干扰与定位。

## 通信 EW 专项（据 EW 103）

- [[communications-search-and-poi|通信辐射源搜索与截获概率（POI）]]——POI 定义、三类搜索策略、
  能量检测接收机（积分-倾倒/相关/码片/滑动窗）、信号环境、无线电视距、LPI 搜索、look-through、
  自相残杀。
- [[communications-intercept|通信信号截获]]——截获链路方程、定向/非定向截获、机载/非视线截获、
  强信号环境中截获弱信号、LPI 信号截获。
- [[communications-emitter-location|通信辐射源定位]]——三角定位、单站定位（SSL/HF）、精度定义与
  CEP 近似、站点/北向基准、干涉仪测向、TDOA/FDOA 精确定位、扩频辐射源定位。

## 平台链路

- [[satellite-communication-links|通信卫星链路]]——EIRP/G/T/Q 术语、噪声温度体系、链路损耗、
  链路性能、与 EW 链路方程的关系、卫星链路干扰。

## 空间 EW（据 EW 105）

- [[orbit-mechanics-for-ew|电子战轨道力学]]——开普勒轨道根数、轨道尺寸-周期、SVP、威胁定位、地平线距离。
- [[space-radio-propagation|空间无线电传播]]——空间 LOS 损耗、大气损耗（随仰角）、天线失配、极化损耗、雨衰。
- [[satellite-links|卫星链路（空间 EW 视角）]]——链路几何、上行（指令/拦截）、下行（遥测/数据/用户/干扰）、敌对链路。
- [[satellite-link-vulnerability|卫星链路对 EW 的脆弱性]]——截获/欺骗/干扰（上/下行）、卫星链路电子防护。
- [[satellite-observation-duration|卫星观测时长与多普勒频移]]——地平线距离、目标可用时长、地球自转、多普勒。
- [[intercept-from-space|空间截获]]——低轨/静止轨道截获雷达与通信、灵敏度/链路余量/地平线判据。
- [[jamming-from-space|空间干扰]]——从卫星干扰通信网/数据链/地面雷达、J/S、低 RCS 杠杆、时长、静止轨道劣势。

## 方法学

- [[ew-simulation|EW 仿真]]——建模/仿真/仿真注入、注入点分级、威胁与天线方向图仿真、保真度。

## 与历史/装备线的接口

- 历史叙事：[[electronic-warfare-in-ww2|二战电子战]]、[[electronic-warfare-cold-war-1946-64|电子战·冷战早期]]
- 对抗行动/装备：[[sead|SEAD/DEAD]]、[[agm-45-shrike|Shrike]]、[[agm-78-standard-arm|Standard ARM]]、
  [[agm-88-harm|HARM]]、[[sa-2-guideline|SA-2]]、[[sa-10-s300|SA-10/S-300]]、[[window-chaff|Window/Chaff]]、
  [[qrc-160-pod-family|QRC-160 吊舱族]]、[[alq-119-jammer-pod|ALQ-119]]、[[alq-165-aspj|ALQ-165 ASPJ]]
- 情报侧：[[sigint|SIGINT]]、[[nsa|NSA]]、[[gchq|GCHQ]]、[[ec-121-warning-star|EC-121]]、
  [[rb-66c-elint|RB-66C]]、[[rc-135-signals-family|RC-135 家族]]、[[ru-21-electric-warrior|RU-21]]

## 使用说明

- 本专题各页为**技术参考汇总**，公式与分类可复用；涉及具体历史战果/日期/装备运用时，须回到
  相应历史来源页与 raw，不据教材断言历史事实。
- 教材未机械分章建页：仅按“可长期研究、可跨战争复用”的**主题单元**整合为上述页面。
