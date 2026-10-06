---
title: "EW 103: Tactical Battlefield Communications Electronic Warfare（David L. Adamy, Artech House, 2009）"
type: source
source_type: book
author: David L. Adamy
year: 2009
publisher: Artech House
raw_file: raw/papers/ew-103-adamy.pdf
tags: [source, electronic-warfare, technical-reference, textbook, communications]
sources: [ew-103-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# EW 103: Tactical Battlefield Communications Electronic Warfare

David L. Adamy 著，Artech House，2009 年。是 [[sources/ew-101-adamy|EW 101]] 与
[[sources/ew-102-adamy|EW 102]] 的续编，三书同属 "EW 100 系列"。本书副题即定位：**战术战场通信
电子战**——聚焦 VHF/UHF/低微波频段的战术战场通信，兼及较低频传播、数字指挥/数据链与卫星通信。
**不含**雷达威胁、搜索、截获、干扰、诱饵（这些见 EW 101/102）。

## 摄入定位（技术参考资料模式）

本书按用户指示作为 **technical reference** 摄入：优先提取具有**长期研究价值、可跨战争复用**
的技术概念、原理、分类、参数关系、公式及作战意义，增量补齐/扩展本库电子战技术概念层（尤其
通信 EW 方向）。**不**将教材章节机械拆分为大量页面；**不**用其一般性技术说明代替具体历史事件
的史料证据。具体历史事实、装备实际运用和历史时期术语**仅在本书明确提供证据时**摄入（本批未
发现足量的此类史料，故未据本书新增历史实体/事件页）。

## 全书结构（9 章 + 附录）

1. **Introduction**——通信的本质、频段、dB 数学（含滑尺换算）。
2. **Communications Signals**——模拟/数字调制、数字带宽与结构、噪声、LPI 信号（伪随机码/跳频/
   chirp/直接序列/组合技术/手机信号）、纠错码。
3. **Communication Antennas**——天线参数、通信天线类型（鞭状/对数周期/抛物面/偶极子阵）、波束、
   增益、极化、相控阵、抛物面盘。
4. **Communications Receivers**——接收机类型（脉冲/超外差/TRF/固定调谐/信道化/布拉格盒/压缩/
   数字）、数字化（采样率/I&Q）、数字化信号质量问题（码片检测/截获跳频）、系统灵敏度（kTB/噪声
   系数/所需预检 SNR）、系统动态范围（模拟 vs 数字）、典型接收机系统配置（多接收机侦察/ESM、
   遥控接收）。
5. **Communications Propagation**——单向链路方程、传播损耗、视线、双径、菲涅尔区、刀边衍射、
   大气与雨损耗、HF 传播、卫星链路。
6. **Search for Communication Emitters**——截获概率（POI）、搜索策略（一般/定向/顺序甄别）、
   系统配置与搜索用接收机、信号环境、无线电视距、LPI 信号搜索、look-through、自相残杀、
   搜索策略示例。
7. **Location of Communications Emitters**——定位途径（三角/单站 SSL/方位仰角）、精度定义
   （RMS/CEP/EEP）、站点位置与北向基准、中/高精度测向技术、精确定位（TDOA/FDOA）、误差预算、
   扩频辐射源定位。
8. **Intercept of Communications Signals**——截获链路、定向/非定向传输截获、机载截获、非视线
   截获、强信号环境中截获弱信号、LPI 信号截获。
9. **Communications Jamming**——J/S、其他损耗、stand-in 干扰、数字 vs 模拟信号、脉冲干扰、
   对扩频信号干扰（部分频带/跳频/chirp/DSSS/组合模式）、纠错编码对干扰的影响、干扰手机
   （上行/下行）。

附录 A：习题解答；附录 B：参考文献；附录 C：附赠 CD 使用说明。

## 关键可复用公式（索引）

- 截获链路：`P_R = P_T + G_T − L + G_R`。
- 通信 J/S：`J/S = ERP_J − ERP_S − L_J + L_S + G_RJ − G_R`。
- 无线电视距（4/3 地球）：`D = 4.12·(√H_T + √H_R)`（km、m）。
- DF 系统 CEP 近似：`CEP = 1.17·d·tan(RMS)`；`90% CEP = 1.57·d·tan(RMS)`；`CEP = 0.75·√(a²+b²)`（由 EEP）。
- FDOA：`F_R = F_T·[1 + V_R·cos(θ)/c]`；`ΔF = F_T·[V_2cosθ_2 − V_1cosθ_1]/c`。
- 灵敏度 `S = kTB + NF + RFSNR`；数字带宽（3-dB = 0.88×码钟；MSK 为 0.66×码钟、旁瓣 −23 dB）。
- 传播损耗（扩散 `32.4+20log d+20log f`）、双径、菲涅尔区、刀边衍射（同 EW 101/102，见
  [[ew-link-equation-and-db-math|链路方程页]]）。

## 注意与局限

- 本书为**入门技术教材**，非史料：不提供具体战例的战果、日期、部队等一手证据。本库引用本书之处
  仅限技术概念、分类与公式。
- 与 EW 101/102 在**非通信专项**（天线、接收机、传播模型、J/S、定位精度）上存在系统重叠；
  摄入时**优先增量更新既有概念页**（如 [[ew-against-communications|对通信的 EW]]、
  [[ew-link-equation-and-db-math|链路方程]]、[[ew-receiver-architecture|接收机]]、
  [[ew-antenna-parameters|天线]]），仅对**通信搜索/截获/定位**等新主题另建专页，避免重复建页。
- OCR 提取文本中部分图表与公式排版错乱；摄入时以正文叙述核对，未据乱码臆造数值。

## 关联

- 由本书**新建**的通信 EW 概念页：[[communications-search-and-poi|通信辐射源搜索与 POI]]、
  [[communications-intercept|通信信号截获]]、[[communications-emitter-location|通信辐射源定位]]。
- 由本书**增量更新**的既有页：[[ew-against-communications|对通信的 EW]]、[[ew-link-equation-and-db-math|链路方程与 dB 数学]]、
  [[ew-receiver-architecture|EW 接收机]]、[[ew-antenna-parameters|EW 天线]]。
- 姊妹来源：[[sources/ew-101-adamy|EW 101]]、[[sources/ew-102-adamy|EW 102]]；同属专题
  [[topics/electronic-warfare-technical-foundations|电子战技术基础]]。
- 与本库历史线衔接：[[electronic-warfare-in-ww2|二战电子战]]、[[electronic-warfare-cold-war-1946-64|电子战·冷战早期]]、
  [[sigint|SIGINT]]、[[sead|SEAD/DEAD]]。

## 原始资料

- `raw/papers/ew-103-adamy.pdf`（原始 PDF，348 页）
- `raw/papers/ew-103-adamy.txt`（本地提取文本，SHA256: 23fca8edbad6d652c58636f8ad2691d58308da4b5c7e74544477c673287426e9）
