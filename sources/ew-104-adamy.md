---
title: "EW 104: EW Against a New Generation of Threats（David L. Adamy, Artech House, 2015）"
type: source
source_type: book
author: David L. Adamy
year: 2015
publisher: Artech House
raw_file: raw/papers/ew-104-adamy.epub
tags: [source, electronic-warfare, technical-reference, textbook, drfm, electronic-protection]
sources: [ew-104-adamy]
created: 2026-10-05
updated: 2026-10-05
---

# EW 104: EW Against a New Generation of Threats

David L. Adamy 著，Artech House，2015 年（ISBN 13: 978-1-60807-869-1）。是 EW 100 系列
（[[sources/ew-101-adamy|EW 101]]／[[sources/ew-102-adamy|EW 102]]／[[sources/ew-103-adamy|EW 103]]）
的**第四册**，据《Journal of Electronic Defense》的 EW 101 专栏（当时已 213 篇、跨两十年）汇编。
定位为**面向新一代威胁**的技术教材/技术参考，用**开放源**威胁信息（作者明确声明"非威胁简报"）。

## 摄入定位（技术参考资料模式）

本书按用户指示作为 **technical reference** 摄入：优先提取具有**长期研究价值、可跨战争复用**的
技术概念、原理、分类、参数关系、公式及作战意义，增量补齐/扩展本库电子战技术概念层（尤其
**频谱战概念层、雷达电子防护、DRFM** 等新方向）。**不**将教材章节机械拆分为大量页面；**不**用其
一般性技术说明代替具体历史事件的史料证据。具体历史事实、装备实际运用和历史时期术语**仅在本书
明确提供证据时**摄入——本书确有据**开放源**转录的威胁型号参数（S-300 家族、MANPADS 等），已照录
于 [[radar-electronic-protection|雷达电子防护页]]并**明确标注系本书据开放源、非一手史料**。

## 全书结构（11 章）

1. **Introduction**——EW 领域的变化。
2. **Spectrum Warfare**——战争性质变化、传播相关问题、连通性、抗干扰、带宽需求、分布式能力/
   网络中心战、传输安全 vs 消息安全、赛博战 vs EW、带宽权衡、纠错、EMS 战现实性、隐写术、链路干扰。
3. **Legacy Radars**——老式 SAM/高炮/截获雷达参数、雷达干扰（J/S、自卫/远距、烧穿）、雷达干扰
   技术（覆盖/阻塞/点/扫频点/欺骗；距离/角度欺骗；频率波门拖引；对抗单脉冲；编队/闪烁/地形反射/
   交叉极化/交叉眼）。
4. **Next Generation Threat Radars**——威胁雷达改进、**雷达电子防护（EP）技术**（超低旁瓣、旁瓣
   对消/匿隐、单脉冲、抗交叉极化、chirp/Barker 脉冲压缩、RGPO/AGC/Dicke-Fix、PD 雷达 EP、相干
   干扰、频率分集、PRF 抖动、寻的干扰）、SAM 升级（S-300/SA-10/12/6/8、MANPADS）、截获雷达升级、
   AAA 升级、各能力的 EW 影响。
5. **Digital Communication**——比特流、内容保真、数字调制、BER vs Eb/N0、数字链路规范、抗干扰余量、
   链路余量、天线对准损耗、图像数字化、编码。
6. **Legacy Communication Threats**——通信 EW、单向链路、传播模型、截获、通信辐射源搜索与定位、
   通信干扰（与 EW 103 高度重叠）。
7. **Modern Communications Threats**——LPI 通信信号、跳频/chirp/DSSS 干扰、自相残杀、LPI 辐射源
   精确定位、干扰手机。
8. **Digital RF Memories**——DRFM 框图、宽带/窄带、DRFM 功能、相干干扰、威胁信号分析、非相干干扰、
   跟随干扰、雷达分辨单元与脉冲压缩、复杂假目标、DRFM 使能技术、时延问题、需 DRFM 对抗的雷达技术小结。
9. **Infrared Threats and Countermeasures**——电磁频谱、IR 传播、黑体理论、IR 制导导弹与导引头/
   调制盘、跟踪器（含 rosette/交叉线阵/成像）、IR 传感器、大气窗口、传感器材料、单色 vs 双色、
   照明弹（诱离/迷惑/稀释及定时/光谱/温度/几何）、成像跟踪器、IR 干扰机（热砖/激光 DIRCM/干扰波形）。
10. **Radar Decoys**——诱饵任务、被动/主动诱饵、部署、饱和诱饵、诱离诱饵、消耗性/拖曳诱饵、
    舰船防护诱饵。
11. **Electromagnetic Support Versus Signal Intelligence**——SIGINT（COMINT/ELINT）与 ES（通信 ES/
    雷达 ES）的区别与天线/距离/接收机/搜索/处理技术差异。

## 关键可复用公式（索引）

- 通信链路 J/S：`J/S = ERP_J − ERP_S − LOSS_J + LOSS_S + G_RJ − G_R`。
- 远距支援干扰 J/S：`J/S = 71 + ERP_J − ERP_R + 40logR_T − 20logR_J + G_S − G_M − 10logσ`。
- PD 雷达：处理增益（dB）`= 10log(CPI × PRF)`；`R_U = (PRI/2)·c`；`ΔF = (v_R/c)·2F`。
- DRFM 动态范围 `= 20log₁₀(2ⁿ)`；ADC 约 2.5 样本/Hz + I&Q。
- 数字信号：J/S = 0 dB、占空比 20%–33% 即可停通信（纠错码会提高所需值）。
- 远距支援 J/S 的 `−20 log R_J` 项（杀伤距离增大使 SOJ 效率大降）。

## 注意与局限

- 本书为**入门技术教材**，非史料：其威胁型号参数系**开放源转录**（作者反复声明），本库引用时照录
  并标注来源性质，不当作一手史料。
- 与 EW 101/102/103 在**传播模型、J/S、天线、接收机、中断/搜索/定位、干扰/诱饵、IR**上存在系统
  重叠；摄入时**优先增量更新既有概念页**，仅对**频谱战概念层、雷达电子防护、DRFM、ES vs SIGINT**
  等新主题另建专页，避免重复建页。
- 原书为 EPUB；本库按 Skill 的 EPUB 流程解包 XHTML 提取正文（保留章节顺序），未跑 OCR。

## 关联

- 由本书**新建**的概念页：[[spectrum-warfare-ems|频谱战]]、[[radar-electronic-protection|雷达电子防护（EP）]]、
  [[digital-rf-memory|数字射频存储（DRFM）]]、[[electronic-support-vs-sigint|电子支援 vs 信号情报]]。
- 由本书**增量更新**的既有页：[[jamming|干扰]]（老式雷达干扰技术分类）、
  [[infrared-electro-optical-ew|红外与光电 EW]]（照明弹战术/跟踪器/激光干扰机）、
  [[radar-decoys|雷达诱饵]]、[[ew-against-communications|对通信的 EW]]（数字通信/链路规范）。
- 姊妹来源：[[sources/ew-101-adamy|EW 101]]、[[sources/ew-102-adamy|EW 102]]、[[sources/ew-103-adamy|EW 103]]；
  同属专题 [[topics/electronic-warfare-technical-foundations|电子战技术基础]]。
- 与本库历史线衔接：[[electronic-warfare-in-ww2|二战电子战]]、[[electronic-warfare-cold-war-1946-64|电子战·冷战早期]]、
  [[sead|SEAD/DEAD]]、[[sigint|SIGINT]]。

## 原始资料

- `raw/papers/ew-104-adamy.epub`（原始 EPUB）
- `raw/papers/ew-104-adamy.txt`（本地解包 XHTML 提取文本，SHA256: 8f5913aaddb7722ee02a08db0e90177be540c074410d4d9dc15f3a495d556955）
