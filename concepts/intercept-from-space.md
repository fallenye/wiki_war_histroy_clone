---
title: 空间截获（Intercept from Space）
type: concept
concept_type: electronic-warfare
tags: [concept, electronic-warfare, space, satellite, intercept, elint, link-margin]
aliases: [Intercept from Space, 空间截获, Satellite Intercept, Space ELINT]
sources: [ew-105-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# 空间截获（Intercept from Space）

技术参考层页面。Adamy《EW 105》Ch9 汇总的**从卫星截获敌方地面信号**（雷达与通信）的方法与算例：
低轨与静止轨道两种情形、链路损耗/灵敏度/链路余量/地平线判据/可观时长。作为技术参考，不作为
具体历史事件的史料。

> 卫星 EW 两大任务是**截获**与**干扰**。本书算例使用**任意选定**（合理但**非真实**）的卫星构型、
> 轨道参数与目标能力——目的是演示方程应用，非描述现实系统。分析实际问题时代入现实值即可。

## 1. 从低轨卫星截获雷达信号（Ch9.1）

**算例**：卫星圆轨道高 300 km（a = 6,671 km）、倾角 60°、SVP 在 100°E/45°N；载荷接收机带宽
10 MHz、噪声系数 3 dB、宽波束圆极化天线增益 3 dB。威胁为 6 GHz 雷达、ERP 120 dBm、视轴增益
30 dBi、平均旁瓣低于主瓣 20 dB，位于 95°E/35°N。

- **链路损耗（9.1.1）**：由北极-SVP-雷达位置的球面三角形，用**球面余弦律**
  `cos(a) = sin(lat_SVP)sin(lat_threat) + cos(lat_SVP)cos(lat_threat)cos(ΔLong)` 求地心角
  （例：= 10.58°）；再由卫星-雷达-地心平面三角形求链路距离。
- **LOS 损耗（9.1.2）**：`32.44 + 20log(F) + 20log(d)`。
- **大气与雨衰（9.1.3）**：按频率与仰角取大气损耗（例：6 GHz、0° 仰角 ≈ 2.2 dB）；雨衰按 0°C
  等温线高度估穿雨路径（须质疑“整段穿大雨”是否合理，常假设雨胞覆盖一定比例）。
- **卫星载荷能否收到（9.1.4）**、**接收机灵敏度（9.1.5）**：`S = kTB + NF + RFSNR`
  （算例：kTB = −104 dBm、S = −104+3+15 = **−86 dBm**）。
- **链路余量（9.1.6）**：`P_R − S`（算例 13.6 dB → 截获效果很好）。
- **能否从地平线收到（9.1.7）**：由卫星-地平点-地心平面三角形求地平线距离与地心角
  `C = arccos[R_E/(R_E+H)]`（300 km → 17.2°）；算总损耗（例：LOS 173.9 + 大气 2.2 + 雨 3.9 =
  **180 dB**）→ P_R = 100−180 = −80 dBm → 余量 6 dB（**仍可见**）。
- **卫星能看多久（9.1.8）**：由周期与地心角求（见 [[satellite-observation-duration|观测时长]]）。

## 2. 地球上的地平线图（Horizon Plot on the Earth，Ch9.2）

把卫星在各地面点地平线以上的区域画成图，直观显示其对地表的**可见覆盖**。

## 3. 用窄波束接收天线截获地面目标（Ch9.3）

- **天线指向（Antenna Pointing）**：须把窄波束对准目标方向（由轨道几何求指向角）。
- **截获链路方程**：`P_R = P_T + G_T − 链路损耗 + G_R`。
- **链路损耗**（LOS/大气/雨/指向/极化）。
- **从地平线截获（Intercept from the Horizon）**：地平线处的链路预算。

## 4. 从静止卫星截获（Ch9.4）

- **卫星在地平线时**（低仰角、远距离）。
- **卫星正上方时**（近距、高仰角）。
- 对比 LEO 与 GEO 的截获几何与效能（GEO 距离远 ~37,000 km，损耗大，但可对一点持续覆盖）。

## 5. 作战意义与研究价值

- 空间截获的“地心角→链路距离→各损耗→灵敏度→链路余量→地平线判据→可观时长”流程，是把
  [[orbit-mechanics-for-ew|轨道力学]] + [[space-radio-propagation|空间传播]] + 链路预算**串成一次
  完整空间截获分析**的通用模板。
- “卫星正对垂直鞭状/偶极子天线的零点方向可能收不到”（见 [[satellite-links|卫星链路]]）是空间
  截获特有的几何陷阱。
- LEO（近、驻留短）vs GEO（远、可持续）的截获权衡，是空间 EW 平台选择的核心。

## 关联

- 概念：[[orbit-mechanics-for-ew|轨道力学]]、[[space-radio-propagation|空间无线电传播]]、[[satellite-links|卫星链路]]、
  [[satellite-link-vulnerability|卫星链路脆弱性]]、[[satellite-observation-duration|观测时长与多普勒]]、
  [[jamming-from-space|空间干扰]]、[[communications-intercept|通信信号截获]]、[[ew-link-equation-and-db-math|链路方程]]
- 来源：[[sources/ew-105-adamy|EW 105]]

## 资料来源

[[sources/ew-105-adamy|Adamy《EW 105》]] Ch9（空间截获）。技术参考汇总；算例为**演示用合成数据**，非真实系统。
