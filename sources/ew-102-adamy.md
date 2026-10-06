---
title: "EW 102: A Second Course in Electronic Warfare（David Adamy, Artech House, 2004）"
type: source
source_type: book
author: David L. Adamy
year: 2004
publisher: Artech House
raw_file: raw/papers/ew-102-adamy.pdf
tags: [source, electronic-warfare, technical-reference, textbook]
sources: [ew-102-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# EW 102: A Second Course in Electronic Warfare

David L. Adamy 著，Artech House Radar Library，2004 年（ISBN 1-58053-686-7）。是
[[sources/ew-101-adamy|EW 101]] 的续编，同由《Journal of Electronic Defense》"EW 101/102" 专栏
文章汇编扩展而成（附录 B 有专栏-章节对照）。定位同为电子战**技术教材/技术参考**。

## 摄入定位（技术参考资料模式）

本书按用户指示作为 **technical reference** 摄入：优先提取具有**长期研究价值、可跨战争复用**
的技术概念、原理、分类、参数关系、公式及作战意义，增量补齐/扩展本库电子战技术概念层。
**不**将教材章节机械拆分为大量页面；**不**用其一般性技术说明代替具体历史事件的史料证据。
具体历史事实、装备实际运用和历史时期术语**仅在本书明确提供证据时**摄入（本批未发现足量的
此类史料，故未据本书新增历史实体/事件页）。

## 全书结构（7 章 + 附录）

1. **Introduction**——EW 总论、信息战、如何理解 EW。
2. **Threats**——威胁定义、威胁类型、频段体系、四类制导方式、威胁雷达扫描/调制特征、通信信号威胁。
3. **Radar Characteristics**——雷达功能与分类、雷达距离方程各形式、脉冲调制与脉冲压缩、CW/脉冲
   多普勒/MTI/SAR、LPI 雷达。
4. **Infrared and Electro-Optical Considerations**——电磁频谱与红外分带、黑体辐射、IR 制导导弹与
   导引头/调制盘、IR 线扫描器、FLIR/IRST、夜视、激光指示/告警、IRCM。
5. **EW Against Communications Signals**——HF/VHF/UHF 传播模型（自由空间/双径/刀边）、背景噪声、
   数字通信（调制/BER/带宽）、扩频信号、通信干扰、对扩频信号的干扰与定位。
6. **Accuracy of Emitter Location Systems**——角度测量技术、TDOA/FDOA 精确定位、RMS/CEP/EEP、
   误差预算与合成。
7. **Communication Satellite Links**——卫星链路术语（EIRP/G/T/Q）、噪声温度、链路损耗、链路性能、
   与 EW 链路方程的关系、卫星链路干扰。

附录 A：习题解答（含 EW 101 与 EW 102 两部分）；附录 B：专栏交叉对照；附录 C：参考文献。

## 关键可复用公式（索引）

- 雷达距离方程（能量/功率/与频率无关三形式 + dB 形式）：
  `P_R = −103 + P_T + 2G − 20 log(F) − 40 log(D) + 10 log(σ)`。
- 最大不模糊距离 `R_MAX < 0.5·PRI·c`；最小距离 `R_MIN > 0.5·PW·c`；距离分辨率 `d_r = c·PW/2`。
- 多普勒 `ΔF = 2(V/c)F`；AMTI 机载多普勒 `2FS·cos(θ)/c`；SAR 方位分辨 `d_a = λR/(2L)`（合成）/`λR/L`（真实）。
- 双径损耗 `L = 120 + 40 log(d) − 20 log(h_t) − 20 log(h_r)`；菲涅尔区 `FZ = (h_t·h_r·f)/24,000`。
- kTB `= −114 dBm + 10 log(带宽/1 MHz)`；系统噪声温度 `T_S = T_ANT + T_LINE + (10^(L/10))T_RX`。
- 定位误差合成 `√(Σ error_i²)`；CEP/EEP 与 1.037σ 关系。

## 注意与局限

- dB 常数仅在正确单位下有效（km/MHz/m²/dBm/dBW）。
- 本书为**入门技术教材**，非史料：不提供具体战例的战果、日期、部队等一手证据。本库引用本书之处
  仅限技术概念、分类与公式。
- OCR 提取文本中部分图表与公式排版错乱（如频段表、Table 5.3、部分行内公式、图表页码混入正文），
  摄入时以正文叙述核对，未据乱码臆造数值。

## 关联

- 由本书建立的技术概念页：[[ew-threats-and-guidance|威胁与制导]]、
  [[radar-characteristics|雷达特征]]、[[lpi-radar|LPI 雷达]]、
  [[infrared-electro-optical-ew|红外与光电 EW]]、[[ew-against-communications|对通信的 EW]]、
  [[emitter-location-accuracy|定位精度]]、[[satellite-communication-links|卫星通信链路]]。
- 与 [[sources/ew-101-adamy|EW 101]] 建立的姊妹页（链路方程/dB 数学、天线、接收机、处理与识别、
  辐射源定位、干扰、诱饵、LPI 信号、仿真）同属专题 [[topics/electronic-warfare-technical-foundations|电子战技术基础]]。
- 与本库既有电子战历史线衔接：[[electronic-warfare-in-ww2|二战电子战]]、
  [[electronic-warfare-cold-war-1946-64|电子战·冷战早期]]、[[sead|SEAD/DEAD]]、[[sigint|SIGINT]]。

## 原始资料

- `raw/papers/ew-102-adamy.pdf`（原始 PDF，291 页）
- `raw/papers/ew-102-adamy.txt`（本地提取文本，SHA256: 658fd6c8396eab083eb41fdcb6223960a2ec222f964d1ca7a9940a707b355fbb）
