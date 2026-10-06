---
title: "EW 105: Space Electronic Warfare（David L. Adamy, Artech House, 2021）"
type: source
source_type: book
author: David L. Adamy
year: 2021
publisher: Artech House
raw_file: raw/papers/ew-105-adamy.pdf
tags: [source, electronic-warfare, technical-reference, textbook, space, satellite]
sources: [ew-105-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# EW 105: Space Electronic Warfare

David L. Adamy 著，Artech House，2021 年（ISBN 13: 978-1-63081-834-0）。是 EW 100 系列
（[[sources/ew-101-adamy|EW 101]]／[[sources/ew-102-adamy|EW 102]]／[[sources/ew-103-adamy|EW 103]]／
[[sources/ew-104-adamy|EW 104]]）的**第五册**。定位为**电子战与卫星两学科交叉**的技术教材，
面向“懂 EW 不懂卫星 / 懂卫星不懂 EW / 两者皆新”的读者。作者自述 EW 在空间是**真实**的：许多军民用
卫星至关重要，许多正遭电子攻击、其余亦易受攻击。

## 摄入定位（技术参考资料模式）

本书按用户指示作为 **technical reference** 摄入：优先提取具有**长期研究价值、可跨战争复用**的
技术概念、原理、分类、参数关系、公式及作战意义，增量补齐/扩展本库电子战技术概念层（新增
**空间 EW** 方向）。**不**将教材章节机械拆分为大量页面；**不**用其一般性技术说明代替具体历史事件
的史料证据。具体历史事实、装备实际运用和历史时期术语**仅在本书明确提供证据时**摄入——本书提供了
少量史实（如 **1960 年**西方国家开始发射成像与信号情报卫星；**NRO 1994 年**出版、**2016 年**解密
其侦察卫星项目史），已简要摄入于相关页；书中大量算例系**演示用合成数据**（作者反复声明“非真实
系统”），已明确标注。

## 全书结构（10 章 + 3 附录）

1. **Introduction**——卫星的 EW 价值与劣势、轨道关系、**信号情报卫星项目简史**、全书路线图。
2. **Spherical Trigonometry**——平面/球面三角（正弦律、余弦律、直角球面三角形、Napier 规则）。
3. **Orbit Mechanics**——开普勒轨道根数、轨道尺寸-周期（开普勒第三定律）、SVP、地面位置、传播距离、
   地球轨迹（SVP/极轨/同步）、威胁定位（视距角/方位/距离/仰角）、地平线距离（圆周轨道）。
4. **Radio Propagation**——大气内传播（单向链路、LOS/双径/菲涅尔区/刀边/大气/雨衰；与 EW 103 重叠）。
5. **Radio Propagation in Space**——LOS 损耗、大气损耗、天线失配、极化损耗、雨衰（0°C 等温线）。
6. **Satellite Links**——链路几何、上行（指令/拦截）、下行（遥测/数据/用户/干扰）、敌对链路。
7. **Link Vulnerability to EW**——卫星脆弱性（截获/欺骗/干扰）、下行截获、上行截获、下行干扰、
   上行干扰、卫星链路电子防护。
8. **Duration and Frequency of Observations**——地平线距离、目标可用时长（地心视角/地球自转/观测
   时长公式）、星-地链路多普勒频移。
9. **Intercept from Space**——低轨卫星截获雷达信号、地球地平线图、窄波束接收天线截获、静止卫星截获。
10. **Jamming from Space**——从卫星干扰地面信号、干扰通信网、干扰微波数据链、从空间干扰地面雷达
    （充分性/低 RCS 防护/时长/静止轨道劣势）。

附录 A：信号情报与 EW 公式（截获/通信干扰/雷达干扰/EP）；附录 B：空间 EW 重要数值（轨道/地球
常数、轨道半径与周期表）；附录 C：dB 数学。

## 关键可复用公式（索引）

- 开普勒第三定律 `a³ = C·P²`；静止轨道半径 42,165.7 km / 高 35,795 km / 周期 1,436 min。
- 地平线：`C = arccos[R_E/(R_E+H)]`；链路距离 `c = (R_E+H)sin(C)`；地表距离 `40,030 km×(C/360°)`。
- 观测时长 `T_TOTAL = P[2·arccos(R_E/a)][1 + cos(i)·cos(lat)]`；地球东移 0.25068°/min。
- 多普勒 `ΔF = F·V·cos(θ)/c = F·V_R/c`。
- 空间 LOS 损耗 `32.44 + 20log(d) + 20log(F)`；盘天线增益 `−42.2 + 20log(D) + 20log(F)`；
  波束宽度 `antilog[(86.8 − 20logD − 20logF)/20]`；天线失配 `ΔG = 12(θ/α)²`。
- 接收机灵敏度 `S = kTB + NF + RFSNR`；远距雷达干扰
  `J/S = 71 + ERP_J − ERP_S + 40logR_T − 20logR_J + G_S − G_M − 10log(RCS)`。
- 地球大圆周长 40,030 km；地球半径 6,371 km；FDOA/截获见附录 A。

## 注意与局限

- 本书为**入门技术教材**，非史料：书内**大量算例使用任意选定的合成参数**（"非真实系统"），本库引用
  时明确标注为演示数据，不当作现实系统描述或一手史料。
- 与 EW 101/102/103/104 在**传播模型、J/S、球面三角、天线**上有重叠；本书**独有空间 EW 方向**
  （轨道力学、空间传播、卫星链路脆弱性、空间截获/干扰、观测时长）为主要增量。
- 摄入时**优先增量更新既有页**（satellite-communication-links、jamming、ew-link-equation），
  对空间 EW 独有主题建新页。
- PDF 为 zip-deflate 编码；`pdftotext -layout` 提取文本层完整（打印 "Bad annotation destination"/
  "xref num not found" 警告属 PDF 结构噪声，不影响正文），未跑 OCR。

## 关联

- 由本书**新建**的概念页：[[orbit-mechanics-for-ew|轨道力学]]、[[space-radio-propagation|空间无线电传播]]、
  [[satellite-links|卫星链路]]、[[satellite-link-vulnerability|卫星链路脆弱性]]、
  [[satellite-observation-duration|观测时长与多普勒]]、[[intercept-from-space|空间截获]]、
  [[jamming-from-space|空间干扰]]。
- 由本书**增量更新**的既有页：[[satellite-communication-links|通信卫星链路]]（链路几何/类型）。
- 姊妹来源：[[sources/ew-101-adamy|EW 101]]、[[sources/ew-102-adamy|EW 102]]、[[sources/ew-103-adamy|EW 103]]、
  [[sources/ew-104-adamy|EW 104]]；同属专题 [[topics/electronic-warfare-technical-foundations|电子战技术基础]]。
- 与本库历史/侦察卫星线衔接：[[corona-reconnaissance-satellite|CORONA 侦察卫星]]、
  [[u2-aquatone-program|U-2/AQUATONE]]、[[sources/secret-empire-taubman|Secret Empire]]、
  [[sigint|SIGINT]]、[[electronic-support-vs-sigint|ES vs SIGINT]]。

## 原始资料

- `raw/papers/ew-105-adamy.pdf`（原始 PDF，228 页）
- `raw/papers/ew-105-adamy.txt`（本地提取文本，SHA256: 43f626ac996136caeae0491fefe07cf02187b1b6ee3afa0eb4d7c2b53ce34758）
