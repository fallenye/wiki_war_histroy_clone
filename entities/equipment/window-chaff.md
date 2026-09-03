---
title: Window／Chaff（金属箔条雷达诱饵反制）
type: entity
entity_type: equipment
equipment_type: electronic-warfare-system
wars:
  - world-war-ii
tags: [equipment, ecm, decoy, radar, window, chaff]
aliases: [Window, "Düppel", Chaff]
sources: [instruments-of-darkness-price, apr-vol10-iss1-odell, us-electronic-warfare-history-vol1-price]
created: 2026-09-02
updated: 2026-09-02
---

# Window（英）／Düppel（德）／Chaff（通用）

向空投放大量金属（锡/铝箔）条，在对方雷达萤幕上制造与飞机回波相似的散状假回波，
使操作台被多条假回波“淹没、饱和”而无法判别真机——最早期且沿用至今的雷达“箔条
诱饵”（modern chaff）反制。

## 基本原理与效能参数（据 Instruments of Darkness，第 7 章）

- 1941 底 TRE（Telecommunications Research Establishment）展开用金属条反雷达的试验；
  代号 “Window” 是当时 TRE 总监 Albert Rowe 随手选出、与设备无关联的名字。
- Joan Curran 主持最初试投：比对各种箔片，最有效是**长度约等于目标雷达半波长的简单
  长方形金属条**；最合适的材料是无线电解容器用的锡/铝箔。对 ≥200 MHz 的各雷达，被投
  材料不需过多即可产生与飞机同级的回波。
- 例证（她的报告）：约 40 张 8½×5 英寸箔，在英新型 **Type 11**(500 MHz) 雷达上的回波
  约可冒充一架 Blenheim——频点接近德 **Würzburg**(约 53 cm/570 MHz)。
- 从约 10,000 ft 投放，一团箔云有效约 15 分钟；相隔约 1 英里放出的十团即能在雷达上连成
  一片饱和屏。
- 后续（美国 RRL/Harvard，Terman 请 L. J. Chu 理论分析，Fred Whipple 归纳）：**同样重量
  下，条更多且更窄远比条少而宽有效率**——据此把投放条切为“半 Würzburg 波长”的窄条
  大批量产，交货积存备用。
- 局限：对更低频率（长波）雷达效果较差；而对最高频（厘米波）雷达则影响剧烈——这也
  是 1942–43 英方是否自制反用而须谨慎、先要发展抗反制手段的原因（如 AI Mk IX 自动跟踪、
  美制 SCR-720/AI Mk X、保留不披露的 500 MHz Type 11 GCI）。

## 使用争议（1942–43）

- RAF 于 1942 年初即制出 Window，原拟用于预定于月底执行的“千机”科隆大空袭；而
  Portal/Cherwell 以“若德方以同样手段反用于英方，需先备妥不惧其反制且能有效对抗的
  英雷达”为由暂缓其使用（Bomber Command、TRE 的 Cockburn、R. V. Jones 等主张早用）。
  Derek Jackson（牛津光谱学家、夜战机雷达操作员出身）于 Coltishall 做第二批试投并
  协助拟定英方雷达抗 Window 的对策。
- 德方同期在波罗的海做 **Düppel**（偶极）试验，结论同样「能有效地屏蔽对目标的精确
  跟踪」；但 1942 年 Göring 阅报后下令禁止一切相关试投、连反制研究亦停止，以免英方
  得知——这让德夜战/高炮系统对箔条毫无准备，直至 1943 年夏英方大量上门。

## 首次大规模实战（1943-07-24/25，Operation Gomorrah—汉堡）

- 1943-07-24/25 夜，Bomber Command 在 **Operation Gomorrah** 对汉堡的大攻势中首次
  大规模投放 Window，使该夜德制雷达（高炮指挥用 Würzburg 连带若干地面预警）遭箔条
  饱和而「失明」；随后数夜对汉堡的连续攻击合称“战役级轰炸”（Hamburg / Gomorrah），
  标志二战中大规模雷达箔条反制的实战起点。

## 后续变体（长波/特殊）

- 反德 **Seetakt**（舰载/岸防）与 **Freya** 等较长波雷达，需约 6 英尺长条；机上不便，
  由 Derek Jackson 设计成 **手风琴式折叠条**，投出后尾部小锤将其展开至正确长度——
  为 D-Day 欺骗两“鬼舰队”（Taxable/Glimmer）核心依据（参见 WWII 时间线与 Invasion
  ECM 段）。

## 美国发展线（据 Price·美国卷 ch5；第二来源补充）

- 美 RRL 侧自研“金属箔/偶极子”平行线：1942 年内一度因保密要求暂停其空中抛投试验，但无线电研究
  实验室仍续作对**箔条（window）的“首个（自身）理论研究”**。其中单位重量箔料之散射截面理论——
  〔书中人名印作“查”，学界通行作美籍华裔学者 **Chu（朱/楚）**；本页照书留形并注此〕——并得出
  “远离谐振区时箔条愈窄、散射截面愈大”推论。该时属绝密，至 1943-07 汉堡之战才由英方首次实战。
- 美方装备生产同线（ch5）：APT-2（Carpet）1943 春确定经德尔科（GM 体系）量产（首批 100 部约 50
  万美元、附设计师两名）；同期 APT-1“黛娜”、APT-3“鹤”、APQ-2“小地毯”亦投产，合计覆盖约
  85–720 MHz——欧洲战场实战（8AF 首用等）见 ch7–8。

## 关联

- 战争：[[wars/world-war-ii/index|World War II]]
- 雷达（德）：[[freya-early-warning-radar]]、[[wuerzburg-radar]]
- ECM 上位概念：[[electronic-warfare-in-ww2]]
- 事件：[[battle-of-the-beams]]；D-Day 欺骗相关（Gomorrah 等）详 WWII 时间线
- 深度史：[[instruments-of-darkness-price]]（第 7 章技术/争议、第 9 章 Hamburg、
  第 11 章 D-Day 长波折叠条）与 [[us-electronic-warfare-history-vol1-price|美国卷（美系管线）]]。

> 技术史（研制人 Joan Curran；概念来源 Albert Rowe；美 RRL 侧 Chu/Whipple）与
> 两部争议、首战（Hamburg）均据 [[instruments-of-darkness-price]] 第 7、9 章明文；
> 日期/地点以该章叙述为准，跨源同异另表。

## 数量与片长（APR Vol.10-1 第二来源补充）

- 1943-07-24/25 汉堡首用之机队规模/片量数字：约 746 机、投放约 **9,200 万条**（德雷达屏呈
  约 1.1 万架假机以上图像）；首夜损失剧降至 1.5%（此前一年同气候 Hamburg 为 7.2%），10 天内
  连环第四次损失回升 2.2/3.6/4.1%（德军迅速反制）。
- 依文章，Würzburg（53.5 cm）与 早期 Lichtenstein（61 cm）同以约 27cm长条可一并压制。
- Churchill/RAF 亲自授权 1943-07 实战解禁（英方先前因自家雷达脆弱而延用）；德方 Düppel
  试验同因保密被戈林叫停（与前来源一致）。
