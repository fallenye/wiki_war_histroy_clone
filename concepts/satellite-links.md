---
title: 卫星链路（Satellite Links，空间 EW 视角）
type: concept
concept_type: technology
tags: [concept, electronic-warfare, space, satellite, uplink, downlink, link-geometry]
aliases: [Satellite Links, 卫星链路, Uplink, Downlink, Command Link]
sources: [ew-105-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# 卫星链路（空间 EW 视角）

技术参考层页面。Adamy《EW 105》Ch6 汇总的**卫星链路几何与类型**（上行/下行、指令/遥测/数据/
载荷/探测/干扰链路、敌对链路）。是空间 EW 的链路框架；通信卫星链路的噪声温度/EIRP/G-T 体系见
[[satellite-communication-links|通信卫星链路]]。作为技术参考，不作为具体历史事件的史料。

> 卫星无人 → 与卫星通信须靠**电磁链路**，而链路**易被敌方对抗**（截获/欺骗/干扰）。

## 1. 链路几何（Link Geometry）

- **向下看（looking down）**：卫星在目标上方，须计算卫星到地面点的距离（用轨道几何）。
- **向上看（looking up）**：地面站看卫星的仰角/方位（由地面站-卫星-地心平面三角形求）。
- 用一组轨道数例演示链路几何（见 [[orbit-mechanics-for-ew|轨道力学]]的球面/平面三角）。
- 链路指向**相对地面控制站**与**相对敌截获站**的角度须分别计算（截获几何与己方控制几何不同）。

## 2. 上行链路（Uplinks）

- **指令链路（Command Links）**：地面站→卫星，携带同步/地址/数据/纠错位；指令信号带宽通常低，
  但可为容纳差错检测与纠正而显著增大带宽；须确保指令被卫星**正确接收**（数据率与报文结构须
  设计到在执行速度上避免不可接受的时延）。
- **拦截链路（Intercept Links）**：敌发信机→**卫星载荷接收机**（图 6.8）。敌发信机可关联雷达、
  通信系统、广播台或数据链，可有任何调制，可在地面或机上。接收功率
  `P_R = P_T + G_T − 链路损耗 + G_R`。
  - 被截获的发信天线可能有**两个不同增益值**——对期望接收机的、与对卫星截获接收机的；若目标用
    极宽角天线（偶极子/鞭状），二者可相等。
  - **几何要点**：垂直安装的此类天线在**离地平线 90°**（即卫星正上方）有**零点**——故卫星**正对**
    敌发信机时可能收不到信号；且信号到卫星的**极化**可能不同于其对本方期望接收机的极化，会降低
    卫星收到功率。工程惯例：**假定敌发信机对本方期望接收机取最优指向与极化**。
- 链路距离由敌发信机与卫星位置决定；天线取向决定有效收发增益与极化损耗。

## 3. 下行链路（Downlinks）

卫星→地面的下行可指向：卫星**控制站**、需要卫星所收集信息的**其他站**、或**截获卫星下行的敌
接收机**；亦可指向“被卫星干扰的敌接收机”。下行方程同为
`P_R = P_T + G_T − 链路损耗 + G_R`。

- **遥测链路（Telemetry Link）**：卫星→地面，报卫星状态。
- **数据链路（Data Link）**：载荷数据下行（如图像）。
- **面向数据用户的链路（Links to Data Users）**。
- **干扰链路（Jamming Links）**：下行被干扰的链路。

## 4. 敌对链路（Hostile Links）

- **敌地面干扰机干扰任何卫星上行**。
- **敌机载干扰机干扰任何卫星下行**。
- 敌接收机可**截获卫星下行**；机载敌接收机可截获卫星或载荷上行。
- 详细覆盖见 [[satellite-link-vulnerability|链路脆弱性]]（Ch7）。

## 5. 作战意义与研究价值

- “卫星无人 → 链路是命门”是空间 EW 的核心：卫星的价值在载荷（截获/干扰/通信），而其**指令与数据
  链路**是对手最容易攻击的环节。
- 上行（指令/截获）与下行（遥测/数据/用户/干扰）的分类，是把任何卫星链路归类、并判断其
  截获/欺骗/干扰意义的通用框架。
- 链路几何（相对控制站 vs 相对敌截获站的角度）是空间截获/干扰效能的决定性输入。

## 关联

- 概念：[[orbit-mechanics-for-ew|轨道力学]]、[[space-radio-propagation|空间无线电传播]]、
  [[satellite-link-vulnerability|卫星链路脆弱性]]、[[satellite-observation-duration|观测时长与多普勒]]、
  [[intercept-from-space|空间截获]]、[[jamming-from-space|空间干扰]]、
  [[satellite-communication-links|通信卫星链路]]、[[ew-against-communications|对通信的 EW]]
- 来源：[[sources/ew-105-adamy|EW 105]]

## 资料来源

[[sources/ew-105-adamy|Adamy《EW 105》]] Ch6（卫星链路）。技术参考汇总，非史料。
