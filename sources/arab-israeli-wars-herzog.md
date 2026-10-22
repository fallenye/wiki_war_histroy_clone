---
title: Herzog《The Arab-Israeli Wars：War and Peace in the Middle East》
type: source
source_type: book
author: Chaim Herzog
year: 1982
publisher: Arms & Armour Press / Vintage Books（1984 年平装）
sha256: 79cea61f26858aaa4ca914879a35a016b1c3e4658079f3bc259eb1a9c82ff409
tags: [source, middle-east, israel, arab-israeli-wars]
created: 2026-10-22
updated: 2026-10-22
---

# Herzog《The Arab-Israeli Wars》

## 书目与文件

- 作者 **Chaim Herzog**：以色列国防军退役少将，曾任军事情报部门负责人、驻联合国代表，后任以色列总统（本书 1982 年初版时的身份为公共人物与军事评论者）。
- 版本：Arms & Armour Press（Lionel Leventhal Ltd，伦敦）1982 年初版；Vintage Books 1984 年 1 月平装版。地图与排版版权 Lionel Leventhal Ltd。
- 文件：`raw/papers/arab-israeli-wars-herzog/herzog-arab-israeli-wars.pdf`
- sha256：`79cea61f26858aaa4ca914879a35a016b1c3e4658079f3bc259eb1a9c82ff409`
- 原始扫描：Internet Archive 藏本（`arabisraeliwarsw00herz`），2012 年数字化，LuraDocument PDF。
- 规模：**440 页**（386×577 pt），文本约 118 万字符。
- 提取：`pdftotext -layout` 未跑 OCR；文本层质量**中等偏差**——正文可读但存在系统性替代错误
  （如 `RafuP`=Raful、`wassel`/`WasseP`=Wasel、`Shazli`/`Shazly` 混用、`Hon`=Hofi、
  `Mandler`/`Mendler` 混用、页码与页眉混入正文）。**地图页完全不可判读**（地名、符号、路线混杂），
  本库一律不从地图文字层取名，只取正文叙述。

## 结构与页码（PDF 页序）

| 部分 | 标题 | PDF 页 |
|---|---|---|
| — | 卷首、目录、地图目录 | 1—17 |
| BOOK I | The War of Independence 1948-1949 | 18—127 |
| BOOK II | The Sinai Campaign of 1956 | 128—165 |
| BOOK III | The Six Day War 1967 | 166—215 |
| BOOK IV | The War of Attrition | 216—247 |
| BOOK V | The Yom Kippur War 1973 | 248—347 |
| BOOK VI | The War against Terrorism: Entebbe | 348—359 |
| BOOK VII | Operation 'Peace for Galilee' | 360—409 |
| — | Index / 出版广告 | 410—440 |

Book V 内部小节（章级）：Prologue（227 页起）→ 1. The Southern Front（含 The deception／The onslaught／
Defending the Bar-Lev Line／'Shovach Yonim'／The first counterattack／The crisis／The Israeli plan／
Opening the gap／The crossing／The battle for the corridor／On the west bank／The cease-fire）→
2. The Northern Front（The Syrian attack／The Israeli break-in／Syria's plight／Iraqi and Jordanian
counterattacks／The recapture of Mount Hermon）→ 3. The Air and Naval War（SAMs v. 'Flying artillery'／
Missiles at sea）→ Summary: A New Era。

## 来源性质与用法

- **以色列官方视角的通史**：作者是前军情负责人，大量采用**以色列军方访谈、战后复盘与 Agranat 委员会材料**；
  阿方叙述多转引沙兹利回忆录与埃方战后公开表态。
- 与既有主源 [[yom-kippur-war-rabinovich|Rabinovich《The Yom Kippur War》]]的关系：
  **同一场战争、同一方视角的第二来源**，覆盖范围更广（1948—1982 六场战争），但 1973 部分的
  细节密度低于 Rabinovich。**两书数字多处不一致**——本库的处理是：冲突数字在两处并列并标口径来源，
  不做加权、不做"取中"、不合并为一个"权威值"。
- 对 1948、1956、1967、消耗战、恩德培、1982 黎巴嫩六条线，本书是本库**唯一来源**，
  因此相应页面必须标"单源未校"。
- 全书用"以色列视角 + 事后诸葛"的叙述方式，评价性语句（如"军事胜利属于以色列"）为本书记载的作者判断，
  入库时标明"本书作者的判断"。

## 提取产物

- `herzog-full.txt`：全文（`pdftotext -layout`）。
- `herzog-paged.txt`：按 `\f` 分页，每页前缀 `===== [PAGE n] =====` 标记（与 PDF 页序一致）。
- 分卷切片在会话临时目录，重建方式：按上表页码范围切 `herzog-paged.txt`。

## 与其他来源的关系

- 1973：与 [[yom-kippur-war-rabinovich]] 并列为该战争线的**双主源**（Rabinovich 叙事细、Herzog 全景）。
- 防空与电子战：与 Price《美国电子战史·卷三》ch13（[[yom-kippur-1973-air-sam-ew]]）在 SAM 编成与
  射程上互为参照（Herzog 给出 SAM-2／3／6 的射程与阵地数量，Price 给出电子战细节）。
- 冷战线：本书 1973 章的苏美互动可与 [[wars/cold-war-cuban-missile-crisis/index|古巴导弹危机战争线]] 战争线对照阅读。

## 待办

- Book I—IV、VI、VII 尚未摄入（本轮只完成 Book V 的 1973 年部分）。
- 本书无脚注与页码注释，引用一律以"ch/小节 + PDF 页"标注。
