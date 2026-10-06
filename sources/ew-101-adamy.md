---
title: "EW 101: A First Course in Electronic Warfare（David Adamy, Artech House, 2001）"
type: source
source_type: book
author: David L. Adamy
year: 2001
publisher: Artech House
raw_file: raw/papers/ew-101-adamy.pdf
tags: [source, electronic-warfare, technical-reference, textbook]
sources: [ew-101-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# EW 101: A First Course in Electronic Warfare

David L. Adamy 著，Artech House Radar Library，2001 年（ISBN 1-58053-169-5）。本书由作者在
《Journal of Electronic Defense》的 "EW 101" 专栏文章汇编扩展而成（附录 A 有专栏-章节对照），
定位为电子战**入门教材/技术参考**。

## 摄入定位（技术参考资料模式）

本书按用户指示作为 **technical reference** 摄入：优先提取具有**长期研究价值、可跨战争复用**
的技术概念、原理、分类、参数关系、公式及作战意义，增量补齐本库原有以历史叙事/装备为主的
**技术概念层**空缺。**不**将教材章节机械拆分为大量页面；**不**用其一般性技术说明代替具体历史
事件的史料证据。具体历史事实、装备实际运用和历史时期术语**仅在本书明确提供证据时**摄入
（本批未发现足量的此类史料，故未据本书新增历史实体/事件页）。

## 全书结构（11 章）

1. Introduction（电子战导论与全书路线图）
2. **Basic Mathematical Concepts**——dB 数学、链路方程、传播损耗、球面三角。
3. **Antennas**——参数定义、类型、抛物面参数权衡、相控阵。
4. **Receivers**——九类接收机、组合体制、灵敏度计算。
5. **EW Processing**——威胁识别、去交错、操作员界面。
6. **Search**——搜索维度与参数权衡、窄带搜索策略、look-through。
7. **LPI Signals**——低截获概率信号：跳频、chirp、直接序列扩频。
8. **Emitter Location**——定位目的与精度、测向/定位技术（幅度、Watson-Watt、干涉仪、多普勒、
   TOA/TDOA）。
9. **Jamming**——干扰分类、J/S、烧穿、覆盖/欺骗干扰、对单脉冲雷达的欺骗。
10. **Decoys**——诱饵类型与任务、RCS 与反射功率、被动/主动诱饵、交战中的有效 RCS。
11. **Simulation**——建模/仿真/仿真注入、威胁与天线方向图仿真、保真度。

附录 A：与《Journal of Electronic Defense》专栏的交叉对照。

## 关键可复用公式（索引）

- 扩散损耗：`Ls = 32.4 + 20 log(d_km) + 20 log(f_MHz)`
- 雷达 RCS 反射增益：`P_r − P_i = −39 + 10 log(σ) + 20 log(F)`
- 天线有效面积：`A(dBsm) = 38.6 + G − 20 log(F)`
- 抛物面增益：`G = −42.2 + 20 log(D) + 20 log(F)`
- 球面三角正弦律/余弦律、Napier 规则、多普勒频移 `Δf = f·Verr/c`、
  仅测方位 DF 的仰角致误差 `Error = M − acos[cos(M)/cos(El)]`。
- J/S 与烧穿距离方程（见 [[jamming|干扰页]]）。

## 注意与局限

- 所有 dB 常数（32/32.4/39 等）**仅在正确单位下有效**（km/MHz/m²/dBm）。
- 本书为**入门技术教材**，非史料：不提供具体战例的战果、日期、部队等一手证据。本库引用本书
  之处仅限技术概念、分类与公式。
- OCR 提取文本中部分图表与公式排版错乱（如 Table 4.2 能力矩阵、部分行内公式），摄入时以
  正文叙述核对，未据乱码臆造数值。

## 关联

- 由本书建立/增补的技术概念页：[[ew-link-equation-and-db-math|链路方程与 dB 数学]]、
  [[ew-antenna-parameters|EW 天线]]、[[ew-receiver-architecture|EW 接收机]]、
  [[ew-processing-and-threat-id|EW 处理与威胁识别]]、[[lpi-signals|LPI 信号]]、
  [[emitter-location|辐射源定位]]、[[jamming|干扰]]、[[radar-decoys|雷达诱饵]]、
  [[ew-simulation|EW 仿真]]。
- 与本库既有电子战线的衔接：[[electronic-warfare-in-ww2|二战电子战]]、
  [[electronic-warfare-cold-war-1946-64|电子战·冷战早期]]、[[sead|SEAD/DEAD]]、[[sigint|SIGINT]]。

## 原始资料

- `raw/papers/ew-101-adamy.pdf`（原始 PDF，344 页）
- `raw/papers/ew-101-adamy.txt`（本地提取文本，SHA256: 30b55351d5e0895ecfaabcf990acc59b81e9da83fff309d3c2b2588609feade2）
