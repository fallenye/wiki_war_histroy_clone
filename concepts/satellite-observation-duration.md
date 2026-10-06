---
title: 卫星观测时长与多普勒频移（Observation Duration & Doppler）
type: concept
concept_type: technology
tags: [concept, electronic-warfare, space, satellite, viewing-time, doppler, horizon]
aliases: [Observation Duration, 观测时长, Viewing Time, Doppler Shift, 多普勒]
sources: [ew-105-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# 卫星观测时长与多普勒频移

技术参考层页面。Adamy《EW 105》Ch8 汇总的**卫星对地面目标的可视时长（地平线→地平线）与
星-地链路多普勒频移**计算。是空间 EW（截获/干扰）的“何时能做、做多久”的量化基础。作为技术参考，
不作为具体历史事件的史料。

## 1. 地平线距离（Ch8.1–8.2）

与 Ch3 一致：由卫星-地平点-地心**平面直角三角形**求得。
- 地心角 `C = arccos[R_E/(R_E+H)]`（R_E 地球半径 6,371 km、H 卫星高度）。
- 到地平线链路距离 `c = (R_E+H)·sin(C)`；地表距离 = `40,030 km × (C/360°)`。
- 各周期圆轨道的地平线距离见 [[orbit-mechanics-for-ew|轨道力学]]表 3.3。

## 2. 目标可用时长（Duration of Target Availability，Ch8.3）

- **地心视角（Geocentric Viewing Angle）**：由北极、SVP、地面点构成球面三角形，用**球面余弦律**
  `cos(a) = cos(b)cos(c) + sin(b)sin(c)cos(A)` 求卫星与地面点的地心角（b=90°−卫星纬度、
  c=90°−地面点纬度、A=经度差）。
- **卫星能与一地面点相见的时长（地球不自转时）**：卫星 SVP 自地平点 F 走到 G 所需时间
  = `周期 × (角 H / 360°)`，其中 `H = 2·arccos(R_E/a)`（a 半长轴）。例：周期 180 min、a 10,560 km、
  R_E 6,371 → `H = 2·arccos(6371/10560) = 105.78°` → 观测时长 = `180 × (105.78/360) = 52.8 min`。
- **地球自转的影响（Ch8.3.3）**：卫星相对固定经纬点的净速度 = 卫星实际速度**减去**地球在其下方
  移动的速度。地球每年自转 366 次 → 赤道点向东移 **0.25068°/min**（赤道点东向速度 27.90 km/min）；
  某纬度点东向速度 = `27.90·cos(lat) km/min`。
  - 卫星 SVP 沿轨道速度 = `2πa/P`；经过目标处的东向速度 = `(2πa/P)·cos(i)·cos(lat)`。
- **观测时长公式（Ch8.3.4）**：

  `T_TOTAL = P·[2·arccos(R_E/a)]·[1 + cos(i)·cos(lat)]`

  （P 周期、a 半长轴、i 倾角、lat 目标纬度）。算例：不自转 52.8 min；i=60°、lat=45° 时地球自转使
  观测时间**延长 18.6 min** → 总截获时间（地平线到地平线）**71.4 min**。

## 3. 星-地链路多普勒频移（Ch8.4）

卫星高速运动，故固定地面站收到的频率有偏移。

- **多普勒公式**：`ΔF = F·V·cos(θ)/c = F·V_R/c`（F 发射频率、V 运动收发机速度、c 光速、
  θ 运动速度矢量与信号矢量间的真球面角、V_R 径向速度/距离变化率）。
- **星-地对**：卫星沿轨道、地球也在其内转动，**收发都在动**；多普勒是两速度差经两速度矢量夹角
  修正后的函数。
- **最大频移**出现在**卫星出现在地面站地平线时**（对过顶圆轨道卫星）。
- **接收站速度**、**卫星速度**、最大多普勒一般式与一般式（Ch8.4.2–8.4.5）。

## 4. 作战意义与研究价值

- 观测时长公式 `T_TOTAL = P[2arccos(R_E/a)][1+cos(i)cos(lat)]` 是空间 EW 平台的“覆盖时间”标尺——
  低轨单星对一点仅十几分钟（见 [[jamming-from-space|空间干扰]]算例 12.2 min），持续覆盖须多星或
  静止轨道（但有距离劣势）。
- 地心角/地平点几何是所有“卫星能否看到目标”判断的通用算法。
- 多普勒频移是星-地链路解调、频差定位（FDOA）与信号识别的输入；最大频移在地平线出现这一点对
  空间截获的链路预算有实际意义。

## 关联

- 概念：[[orbit-mechanics-for-ew|轨道力学]]、[[satellite-links|卫星链路]]、[[space-radio-propagation|空间无线电传播]]、
  [[intercept-from-space|空间截获]]、[[jamming-from-space|空间干扰]]、[[emitter-location-accuracy|定位精度（FDOA）]]、
  [[ew-link-equation-and-db-math|链路方程与球面三角]]
- 来源：[[sources/ew-105-adamy|EW 105]]

## 资料来源

[[sources/ew-105-adamy|Adamy《EW 105》]] Ch8（观测时长与多普勒）。技术参考汇总，非史料。
