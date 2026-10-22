---
title: No Margin for Error（Ehud Yonay）：以色列空军的形成
type: source
tags: [israel, iaf, air-power]
created: 2026-10-22
updated: 2026-10-22
---

# No Margin for Error：The Making of the Israeli Air Force

> Ehud Yonay，Pantheon Books（Random House），纽约，1993 年。
> ISBN 0-679-41563-7。副题即"以色列空军的形成"，叙事止于 1973 年赎罪日战争及其后（第 24 章 "Legacies"）。
> **本页是来源页**：记录文件、sha256、提取方式、结构、可核查性限制与本书的写作性质。

## 一、文件与提取

| 项 | 内容 |
|---|---|
| 源文件 | `/mnt/share/test/No margin for error  the making of the Israeli Air Force (Yonay, Ehud) (z-library.sk, 1lib.sk, z-lib.sk).pdf` |
| sha256 | `5a98fc53229894dee7ff4282a6357b87732cd7126ca199609d3124af226bd09d` |
| 原始件 | `raw/papers/iaf-yonay/`（完整 PDF） |
| 页数 | 472 页（pdfinfo）；PDF 每页对应扫描图一页 |
| 提取方式 | `pdftotext -layout`（**未跑 OCR**；该 PDF 为 Internet Archive 2007 年扫描＋LuraDocument 转换，正文层已可读） |
| 提取文本 | `iaf-yonay.txt`（1,157,058 字符）、`iaf-yonay-paged.txt`（470 个 `===== [PAGE n] =====` 标记） |
| 分章文本 | `ch/ch01.txt`—`ch/ch26.txt`（按 PDF 页码切分，见下表） |

### 章节—PDF 页码对照

| # | 章节 | PDF 页 | 书内页 |
|---|---|---|---|
| 1 | Introduction | 17—22 | xi—xiv |
| 2 | 1 Dead Reckoning | 23—32 | 3—12 |
| 3 | 2 The New Brunswick Warning | 33—42 | 13—22 |
| 4 | 3 The Czech Knives | 43—55 | 23—35 |
| 5 | 4 The Banana Grove | 56—68 | 36—48 |
| 6 | 5 The Red Squadron | 69—79 | 49—59 |
| 7 | 6 Bloodying the RAF | 80—92 | 60—72 |
| 8 | 7 The Prince | 95—108 | 75—88 |
| 9 | 8 The Farmer | 109—121 | 89—101 |
| 10 | 9 The Blues and the Greens | 122—139 | 102—119 |
| 11 | 10 The Black Spitfire | 140—156 | 120—136 |
| 12 | 11 French Shuttle | 157—174 | 137—154 |
| 13 | 12 Kadesh | 175—196 | 155—176 |
| 14 | 13 Mirage | 197—207 | 177—187 |
| 15 | 14 Rebels | 208—221 | 188—201 |
| 16 | 15 Moked | 222—233 | 202—213 |
| 17 | 16 The Frontiersman | 234—247 | 214—227 |
| 18 | 17 Three Hours in June | 248—280 | 228—260 |
| 19 | 18 Keep It Simple | 281—296 | 245—260（书内页码有误，见注） |
| 20 | 19 "Texas" | 297—311 | 261—275 |
| 21 | 20 Phantoms | 312—327 | 276—291 |
| 22 | 21 Missiles | 328—342 | 292—306 |
| 23 | 22 Judgment Day | 343—358 | 307—322 |
| 24 | 23 Operatziot | 359—374 | 323—338 |
| 25 | 24 Legacies | 375—394 | 339—356 |
| 26 | Epilogue / Author's Notes | 395—408 | 357—370 |
| — | Notes / Sources / Maps / Index | 409 页以后 | 377 页以后 |

> 页码注：目录标第 18 章起为 245 页，但正文页眉显示第 18 章自 246 页开始，
> 且第 17 章亦标 228 页——**印刷页码本身有跳号**，故本表以 PDF 页为准，书内页仅作参考。

## 二、OCR 质量与可核查性限制

- **正文总体可读**，但有三类问题：
  1. **人名／地名讹误**（如 `A1 Schwimmer`＝Al Schwimmer、`El 'Arlsh`＝El 'Arish、
     `Ishdud`＝Isdud、`HAP'`＝RAF、`Alon` 与 `Ealluja`＝al-Falluja、`G-55 Fiat`＝Fiat G.55）；
  2. **数字与型号**常见混淆（`4-8 war`＝1948、`Ig6os`＝1960s、`Io,ooo`＝10,000、
     `1,200 pounds` 类数字需回查上下文）；
  3. **引号、破折号与分栏错位**较多。
- **本页以下的所有页面一律遵守**：
  - 不复制含数字粘连的乱码词；数字无法判读者**留白并标"本书数字不清"**；
  - **不从地图或插图图注取名**（本 PDF 的地图页与图注文字层不可靠）；
  - 人名以本书通行拼写为准，OCR 明显错拼处改回并在括号内保留原文。

## 三、本书的写作性质（决定用法）

- 这是一部**记者体叙事史**（作者 Ehud Yonay 为记者，1970 年代以报道以色列空军闻名），
  以**人物、轶事与访谈**为主体，不是档案研究，也不是作战序列研究。
- 书末有 "Notes"（377—390 页）与 "Sources"（391 页以后），但**正文大量细节不带注**，
  对话与心理描写显然是重构。**本库只在有具体事实（日期、编制、机型、数量、决策）时引用，
  不引用对话与内心活动作为史实。**
- **以色列视角**：作者明确站在以色列一方，对阿拉伯空军的描述多为转述。
  但本书对以色列自身的批评相当尖锐（见 [[concepts/iaf-independence-struggle-1948]]）。
- 与库内既有来源的关系：
  - **Herzog** 提供以色列官方视角的战役叙事；本书提供**空军内部视角**与人事脉络；
  - **Pollack** 提供阿拉伯军队的效能评估与外部学术分析；
  - 本书与这两者的交叉点（1948 年空中行动、1956、1967）**并列叙述、不合并数字**。

## 四、本书的核心论题（就本库关心的部分）

1. **"没有误差余量"**：以色列的国土、人口与装备都不允许一次失败，空军因此被赋予
   极端的结果导向；这是书名所指，也是全书反复出现的判断标准。
2. **空军独立的代价与收获**：1948 年空军从"陆军的运输队"变成独立军种，
   关键不是装备而是**指挥关系**（[[concepts/iaf-independence-struggle-1948]]）。
3. **人的来源决定早期能力**：1948 年的战斗力几乎全部来自**外国志愿飞行员**，
   他们一走，空军必须从零重建（[[events/iaf-volunteer-era-1948]]）。
4. **装备依赖与外交脆弱**：捷克斯洛伐克（1948）、法国（1950 年代—1967）、美国（1968 以后），
   每一次换供应国都改变空军的战术与政治处境。

## 四之二、Sources 的结构（批 4 录入）

书末三层，本库按其性质分别使用：

### （一）General Bibliography（约 55 种）

- **回忆录／传记（英文本或希伯来文本）**：Eban《An Autobiography》(1977)；Dayan《Avnei Derech》／英文 *Story of My Life*(1976)；
  Rabin《The Rabin Memoirs》(1979)；Meir《My Life》(1975)；Weizman《Le'cha Sha'maim, Le'cha Eretz》／英文 *On Eagles' Wings*(1976)；
  Rafael Eitan《A Soldier's Story》；Eliezer "Cheetah" Cohen《The Sky Is Not the Limit》(1990)；Israel Amir《Unpaved Road》(1988)；
  Mardor《Strictly Illegal》(1957)。
- **学术／第三方史著**：Milstein《The War of Independence》三卷（1989）；Gelber《The Emergence of a Jewish Army》(1986)；
  Bar-Zohar《Ben Gurion》(1986)；Slater《The Pledge》(1970)；Steven《The Spymasters of Israel》(1980)；
  Schiff & Ya'ari《Israel's Lebanon War》(1984)；Schueftan《Attrition》(1989)；Nakdimon《Low Probability》(1982)；
  Haber《Today War Will Break Out》(1987)；Heikal《Cutting the Lion's Tail》(1987)；**Herzog《The Arab-Israeli Wars》(1982)**。
- **技术／装备**：Gunston、Nordeen《Air Warfare in the Missile Age》(1985)、Mason《Phantom》(1984)、
  Taylor《Missiles of the World》(1980)、Rubinstein & Goldman《Shield of David》(1978)、Halperin & Lapidot《G Suit》(1987)。
- **本库已有或可用的**：Herzog（本库第 2 来源）在本书参考书目中；**Rabinovich 与 Pollack 不在其中**（本书成稿于 1992 年）。

### （二）IAF Publications and Manuscripts（6 种，多数标注 classified）

- 《The Air Force in the "Yom Kippur War"》（空军历史处，1975）；
- 101 中队队史日记（1973）、191 中队《In Day, Night and Fog》（1981）与《Squadron Pilots Recall the Six Day War》（1968）、
  221 中队《The One and Only 221: 1969—1982》（1982）、117 中队《The First Jet Squadron》（1982）、
  101 中队《20 La'Tayeset (1948—1968)》（1968）；
- 以及 Maj. Itzhak Shteigman 的 *Operation "Kadesh"*（1986，**classified**）与
  《From the War of Independence to Operation Kadesh》（1990）。

> **本库的处理**：这些队史是本书最细的细节来源（如 Bir Gafgafa 的大钟、Rooster 的炮弹卡壳），但**不可核**
> 且部分为机密；引用时一律标"本书引某中队队史"。

### （三）Interviews（约 75 人次，1982—1991）

按本书排列，涵盖：Agasi、Agmon、Ambar、Amir、Antin、Augarten、Axelrod、Bar On、**Menachem Bar (Bernstein)**、
Barak、Ben-Eliahu、Bnaya、Cheetah Cohen、Sid Cohen、Commanday、Yair David、Eini、**Gad Eldar（化名）**、Al Ellis、
Elrom、Even-Nir、Achikar Eyal、Eli Eyal、Red Finkel、Furman、**Amichai Gal（化名）**、**Shaya Gazit (Schwartzman)**、
Gilbo'a、Coleman Goldstein、Goodlin、Har'el、**Harlev**、Harpaz、**Hod (Fine)**、Penina Hod、**Ivri**、"Bill" Kaiser、
Koren、**Lahat (Landau)**、**Lou Lenart**、**George Lichter**、Liron、**Marom**、**Na'or**、**Yak Nevo (Milner)**、
Nomis、**Beni Peled (Feldman)**、Eitan Peled、**Moshe Peled (Weidenfeld)**、**Rabin**、**Remez**、**Ran Ronen (Pecker)**、
Roof、Rosner、Boris Senior、Shahar、**Danny Shapira**、**Yalo Shavit (Yalovsky)**、Shmul、**Sivron**、Somekh、
**Spector**、**Tolkowsky**、**Tsiddon (Chato)**、Tsivoni、Tsuk、**Weizman**、Denny Wilson、Yavneh、**Yoeli**。

括号内为**改姓前的原姓**（如 Beni Peled 原姓 Feldman、Moti Hod 原姓 Fine、Shaya Gazit 原姓 Schwartzman、
Yak Nevo 原姓 Milner、Ran Ronen 原姓 Pecker、Menachem Bar 原姓 Bernstein）——**这是核对同名异人的关键**。

### （四）对本库最有用的三条史料学事实

1. **作者没服过役，且被视作 Yored**（对居外以色列人的贬称）；前空军司令 Lapidot 当面拒他：
   "你是个 Yored，你为钱写作。我为什么要帮你。"→ 见 [[concepts/yonay-sources-and-methodology]]
2. **本书是为纠正"空军始于 Weizman"这一神话而写的**——作者自陈"我以为我知道的，大部分是错的"。
3. **作者承认机构内部的"修正主义"**，并特别致谢三位 Palmach 老飞行员提醒他 Menahem Bar 被主流空军史省略的贡献。

## 五、与库内既有页面的对应

- 1948 年空战：[[events/iaf-first-fighter-mission-1948]]、[[events/israeli-b17-bombing-cairo-1948]]、
  [[events/operation-dust-bowl-1948]]、[[events/downing-of-raf-spitfires-1949]]、
  [[events/iaf-spitfire-ferry-winter-1948-49]]
- 概念：[[concepts/iaf-independence-struggle-1948]]、[[concepts/iaf-doctrine-air-superiority-first]]
- 装备：[[entities/equipment/avia-s-199]]、[[entities/organizations/iaf-101-squadron]]
- 人物：[[entities/people/aharon-remez]]、[[entities/people/modi-alon]]、
  [[entities/people/ezer-weizman]]（既有页将据本书扩写）

## 相关页面

- 其他来源：[[sources/arab-israeli-wars-herzog|Herzog《The Arab-Israeli Wars》]] ·
  [[sources/yom-kippur-war-rabinovich|Rabinovich《The Yom Kippur War》]] ·
  [[sources/arabs-at-war-pollack|Pollack《Arabs at War》]]

## 五之二、Yonay 线的页面总表（四批）

**概念 8**：[[concepts/iaf-independence-struggle-1948]] · [[concepts/iaf-doctrine-air-superiority-first]] ·
[[concepts/iaf-blues-vs-greens]] · [[concepts/iaf-training-revolution-ot-u-105]] · [[concepts/iaf-french-shuttle-1953-56]] ·
[[concepts/moked-plan-1967]] · [[concepts/iaf-operatziot-vs-hunt]] · [[concepts/iaf-1973-intelligence-blindness]] ·
[[concepts/iaf-reconstruction-after-1973]] · [[concepts/yonay-sources-and-methodology]] · [[concepts/iaf-six-theses-yonay]]

**事件 15**：[[events/iaf-first-fighter-mission-1948]] · [[events/iaf-volunteer-era-1948]] ·
[[events/iaf-czech-airlift-1948]] · [[events/israeli-b17-bombing-cairo-1948]] · [[events/operation-dust-bowl-1948]] ·
[[events/iaf-spitfire-ferry-winter-1948-49]] · [[events/downing-of-raf-spitfires-1949]] ·
[[events/el-hamma-and-hula-air-actions-1951]] · [[events/iaf-meteor-vs-vampire-1955]] · [[events/iaf-sinai-air-war-1956]] ·
[[events/iaf-operation-rooster-1956]] · [[events/operation-moked-1967-06-05]] · [[events/elie-cohen-syrian-front-1960s]] ·
[[events/iaf-attrition-air-war-1969-70]] · [[events/dougman-v-1973-10-07]] · [[events/bekaa-valley-1982-air-battle]] ·
[[events/entebbe-airlift-1976]] · [[events/osirak-raid-1981]]

**实体 7**：[[entities/equipment/avia-s-199]] · [[entities/organizations/iaf-101-squadron]] ·
[[entities/people/aharon-remez]] · [[entities/people/modi-alon]] · [[entities/people/dan-tolkowsky]] ·
[[entities/people/beni-peled]] · [[entities/people/iftach-spector]] · [[entities/people/shmuel-hetz]] ·
[[entities/people/avihu-ben-nun]]

**扩写既有页 5**：[[entities/people/ezer-weizman]] · [[entities/people/mordechai-hod]] · [[entities/people/haim-laskov]] ·
[[entities/people/david-ivri]] · [[entities/equipment/mirage-iiicj]]
