---
title: 通信信号截获（Intercept of Communications Signals）
type: concept
concept_type: technology
tags: [concept, electronic-warfare, communications, comint, intercept, esm, lpi]
aliases: [Communications Intercept, 通信截获, COMINT, Intercept Link]
sources: [ew-103-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# 通信信号截获（Intercept of Communications Signals）

技术参考层页面。Adamy《EW 103》Ch8 汇总的**通信信号截获链路、定向/非定向传输截获、强信号环境中
截获弱信号、LPI 信号截获**。作为技术参考，不作为具体历史事件的史料。

## 1. 定义与分工：COMINT vs 通信 ESM

- **截获（intercept）**通常指敌接收机**解调**通信信号以恢复其承载信息，亦称**通信情报（COMINT）**。
- **通信 ESM** 通常处理信号**外部特征**（频率、辐射源位置、调制等），对构建**电子战斗序列（EOB）**
  （据以判断敌组织乃至意图）极有用。因许多通信信号加密，恢复**内部信息**可能不实用——故截获
  价值可能仅限于**外部特征的获取与利用**。

本章主要讲接收与解调各类敌通信信号的技术；信号从发端到截获接收机的传播遵循 [[ew-against-communications|传播
模型]]；截获接收机灵敏度由 [[ew-receiver-architecture|灵敏度技术]]确定；据此可计算作为链路参数函数
的**截获有效距离**。

## 2. 截获链路（The Intercept Link）

截获接收机收到的功率：

`P_R = P_T + G_T − L + G_R`

（P_R 由截获天线进入接收机的信号强度 dBm；P_T 发射机输出功率 dBm；G_T 发射天线在**截获接收机方向**
上的增益 dB；L 从发射机到截获接收机的传播损耗 dB——用适当的传播模型；G_R 截获系统接收天线在
**发射机方向**上的增益 dB。）

要点：

- **发射天线在“期望接收机方向”与“截获接收机方向”上的增益可能不同**（截获机常不在发射主瓣内）。
- 若接收功率大于截获接收机系统灵敏度，截获可能。**理想上截获接收机带宽应与被截获信号调制匹配**，
  以获得最佳灵敏度、从而最大截获距离。
- 求最大截获距离：令接收功率 = 灵敏度，反解传播损耗中的距离项。

### 2.1 定向传输的截获

发信机用定向天线对准期望接收机，敌接收机不在发射方向图主瓣内；收发均在高地（接收天线不受本地
地形强反射）→ 传播损耗用**视线模型**：

`P_R = P_T + G_T − [32.4 + 20 log(d) + 20 log(f)] + G_R`

例（书中算例）：发 100 W、20 dBi（期望接收机方向）、5 GHz、20 km、旁瓣电平 −15 dB、截获天线
增益 6 dBi、截获接收机灵敏度 −80 dBm。

### 2.2 非定向传输的截获

发信机用 360° 覆盖天线（如战术电台）时，截获机只需在方位上可见即可。

## 3. 机载截获系统（Airborne Intercept System）

机载接收机升高可“看”得远（无线电视距更大，见 [[communications-search-and-poi|搜索页]]的 radio
horizon）；可截获地面发射。

## 4. 非视线截获（Nonline-of-Sight Intercept）

地形遮挡时的截获，须考虑**刀边衍射（KED）损耗**（用 KED 诺谟图，见
[[ew-link-equation-and-db-math|链路方程页]]的传播损耗节）。

## 5. 强信号环境中截获弱信号

接收系统须能在强信号存在下截获弱信号（动态范围问题，见 [[ew-receiver-architecture|接收机]]）。

## 6. LPI 信号的截获

LPI 信号的运作见 [[lpi-signals|LPI 信号页]]。

- **截获跳频（Frequency Hoppers）**：跳频信号各时刻集中在一个信息带宽，须在正确跳频上截获；
  可通过延时截获信道等法（让截获信道延时足够以对准某跳）。
- **截获 chirp 信号**。
- **截获直接序列扩频信号**：因扩频码受保护（如同加密的伪随机码），敌无从折叠信号，只能面对
  极低的（展宽）功率密度。

## 7. 作战意义与研究价值

- 截获链路方程（`P_R = P_T + G_T − L + G_R`，含“发射天线在截获方向增益”与宽带匹配）是把“能否
  截获敌通信”量化为距离的通用标尺，跨战争通用。
- COMINT（信息内容）与通信 ESM（外部特征/EOB）的分工，界定了通信情报的两类产出。
- 对 LPI/跳频/DSSS 的截获难点，连接 [[communications-search-and-poi|搜索]]与 [[lpi-signals|LPI 信号]]。
- 机载/非视线截获把 [[ew-link-equation-and-db-math|传播模型]]与无线电地平线结合，支撑截获系统的
  部署与效能评估。

## 关联

- 概念：[[ew-against-communications|对通信的 EW]]、[[communications-search-and-poi|通信搜索与 POI]]、
  [[communications-emitter-location|通信辐射源定位]]、[[lpi-signals|LPI 信号]]、
  [[ew-receiver-architecture|EW 接收机]]、[[sigint|SIGINT]]、[[ew-link-equation-and-db-math|链路方程与 dB 数学]]
- 装备：[[rc-135-signals-family|RC-135 家族]]、[[ru-21-electric-warrior|RU-21]]、[[rb-66c-elint|RB-66C]]
- 来源：[[sources/ew-103-adamy|EW 103]]

## 资料来源

[[sources/ew-103-adamy|Adamy《EW 103》]] Ch8（通信信号截获）。技术参考汇总，非史料。
