# 变更记录

## 2026-09-02

- **任务**：初始化 Wiki。
- **变更**：依据 `SCHEMA.md` 第 4 节基础目录结构，建立顶层目录与原始资料子目录，创建首页 `index.md` 与变更记录页 `log.md`。
- **新建目录**：`wars/`、`events/`、`entities/equipment/`、`entities/organizations/`、`entities/people/`、`entities/places/`、`concepts/`、`topics/`、`timelines/`、`sources/`、`raw/papers/`、`raw/articles/`、`raw/transcripts/`、`raw/assets/`、`_archive/`。
- **新建页面**：`index.md`、`log.md`。
- **摄入资料**：无。
- **异常**：无。
- **检查**：未修改 `SCHEMA.md`；未创建战争 / 实体 / 事件 / 专题等资料页面。

## 2026-09-02（首次正式摄入）

- **来源**：Peter E. Davies，《F-4 Phantom II Wild Weasel Units in Combat》，Osprey，2023。
- **SHA256**：`cf0d74ff2f9682cf37457f18fb1daa49377f8eaee61dbd64d9ce20bf30dc4aea`。
- **raw 保存**：`raw/papers/F-4 Phantom II Wild Weasel Units in Combat (…).pdf`（复制原件）；
  提取文本 `raw/papers/f4-wild-weasel-units-davies.txt`（pdftotext -layout，本地文本层，未 OCR）。
- **新建页面**：
  - 来源记录：`sources/f-4-wild-weasel-units-in-combat.md`
  - 战争索引+时间线×2：`wars/vietnam-war/{index,timeline}.md`、
    `wars/gulf-war/{index,timeline}.md`
  - 概念：`concepts/sead.md`
  - 事件：`events/linebacker-ii-wild-weasel-sead.md`、`events/desert-storm-opening-night.md`
  - 实体-装备：`entities/equipment/` 下 f-100f-wild-weasel-i、f-105-wild-weasel、
    f-4cww-wild-weasel-iv、f-4g-wild-weasel-v、sa-2-guideline、agm-45-shrike、
    agm-78-standard-arm、agm-88-harm、agm-65-maverick
  - 实体-组织：`entities/organizations/` 下 6234th-tfw、388th-tfw、67th-tfs、81st-tfs、
    52nd-tfw、george-afb-f-4g、561st-tfs、90th-tfs、190th-fs-idaho-ang
  - 实体-人物：`entities/people/` 下 kenneth-dempster、allen-lamb、jim-uken、
    edward-ballanco、bruce-benyshek、charles-horner
  - 更新首页 `index.md`。
- **Index 变化**：两战争首页加入上述 canonical 链接，全球时间线 `timelines/master.md` 未建。
- **时间线**：越战、海湾两战争时间线被更新；日期均取自该来源并标注不确定性。
- **跳过**：彩色插页机体涂装细节仅作佐证不再单页化；end matter 不建页。
- **异常**：无 OCR；SCHEMA.md 未改动。多页面在撰写中发现并更正个别机身/日期表述。
- **检查**：
  - frontmatter 均有效；页面自 canonical 页/索引可达；
  - wikilink 尽量采用可解析 basename 或相对路径表示；
  - 全卷基于单来源：战果/日期留存最与官方史冲突处注明 contested／待校核；
  - raw PDF＋提取文本留存；未出现重复 canonical 页。

## 2026-09-02（增量摄入·F-105 vs SA-2 Duel）

- **来源**：Peter Davies，《F-105 Wild Weasel vs SA-2 Guideline SAM Vietnam 1965–73》，
  Osprey Duel #35（2011）。
- **SHA256**：`6472f403d60157461cc6efefd6a130304206b0e2d5ab8b420aba5792747c51ca`。
- **raw 保存**：`raw/papers/…F-105 Wild…SA-2…pdf`（复制原件）；
  提取文本 `raw/papers/f105-wild-weasel-vs-sa2.txt`（pdftotext -layout，4096 行，未 OCR）。
- **新增页面**：来源页 `sources/f-105-wild-weasel-vs-sa2.md`；事件
  `events/operation-kingpin-son-tay.md`；人物
  `entities/people/leo-thorsness.md`、`entities/people/merlyn-dethlefsen.md`。
- **增量更新（不重写）**：F-105（WW II/III）、SA-2、AGM-45 Shrike、AGM-78、
  SEAD（concepts）与 388th TFW（org）处以“补充资料（Duel 35）”小节追加该卷新事实，
  各自扩充 `sources:` 至双来源；越南战争时间线（wars/vietnam-war）补充/修正若干
  1965 首次击落日期（并更正 24 Jul/25 Jul 之别，采 24 Jul）及 1966-74 阶段条目。
- **无重复实体**：全文检索既有 canonical（F-105、SA-2、Shrike、Standard ARM、SEAD、
  388、67th、vietnam-war 等）后只做增量，未另开同型页。
- **Index**：越南战争 index 补 Kingpin、双新增人物与第二来源链接；根 index 增列第二来源。
- **时间线**：内容在上级说明。
- **异常**：Duel 卷内个别命中/尺寸（如 AGM-78 弹头 215 vs 219-lb、损失数）与早期来源
  并存，均如实注明口径、未擅归一；F-4C→63-7599 首击日期跨来源证据已用作判定。
- **重复对象/冲突处理**：无重复 canonical；对先前“首架 F-4C 击落日期 24 Jun/25 Jul”
  的两说按本卷 24-Jul──并对照机体 63-7599 予以修正记录。（详情在 timeline 该条注释内。）
- **检查**：frontmatter 可解析；38 个 .md 全部 wikilink 目标可解析（唯 SCHEMA.md 为目的
  性文件链）；SCHEMA.md SHA 未变；该卷 raw 与提取文本均已留存。

## 2026-09-02（增量摄入·Rolling Thunder Air Campaign #3）

- **来源**：Richard P. Hallion，《Rolling Thunder 1965-68：Johnson 的北越空战》，Osprey
  Air Campaign #3（2018）。
- **SHA256**：`d3dd10dcf43f705a3c3f2da71190f572fd00b4a58b26221fc717acbaee05e3a0`（raw 库查无
  重复）。
- **raw 保存**：`raw/papers/rolling-thunder-1965-68-hallion.pdf`（复制原件）；提炼文本
  `raw/papers/rolling-thunder-1965-68-hallion.txt`（pdftotext -layout，4,836 行，未 OCR）。
- **新增页面（3）**：来源页 `sources/rolling-thunder-1965-68-hallion.md`；战役事件页
  `events/rolling-thunder.md`（Rolling Thunder 此前无 canonical event 页，只以纯文本散见
  越南索引与年份行，故按 SCHEMA 判定建立：批准/首袭/阶段/政策限制与总量统计）；装备页
  `entities/equipment/f-111a.md`（F-111A/TFX 及其越战首战 Combat Lancer——本书首次以
  单卷重点覆盖该机型在 SEA 的开端）。
- **增量更新（不整页重写）**：`entities/equipment/sa-2-guideline.md` 追加补充小节（防空
  一体化与 1967-03-24 地区化重组——ADF-VPAF → 361/363/365/367 Air Defence Division，
  及 SA-2 每击落一机所需导弹数 17.64→65.75 的抑制量化，均已注 Rolling Thunder 源）；
  `wars/vietnam-war/timeline.md` 只在既有年份块补充缺失的战略/战役节点（下述）；战争
  索引与根 index 补第三来源及对应链接；事件页间互相 wikilink（Rolling Thunder ⇄
  Linebacker II / Kingpin）。
- **Index**：`wars/vietnam-war/index.md`——战役与行动区把 Rolling Thunder 由纯文本改为
  [[rolling-thunder|…]]，装备区新增 F-111A，主要来源增第三源 ③；根 `index.md` 改“三批”
  结构并补战役入口、F-111 与来源 ③。
- **时间线新增（战略/战役层；此前缺失；本卷未见重复既有 SEAD/Weasel 条目）**：
  1965-02-13 批准、03-02 Rolling Thunder V 首袭；1965-12-24─66-01-31 37 天停炸；
  1966-06-29 首次 POL 联合打击；1967-03-24 防空地区化重组（＋AAA/SAM/MiG 协同之差）；
  1967-08-11 355th TFW 炸落 Doumer 桥铁路公路中心跨；1967-10-24 首袭 Phuc Yen 机场；
  1968-01 Khe Sanh/Tet（后打击集中 Pack I）、03-17 Combat Lancer F-111A 抵 Takhli 与
  03-25 首夜作战、03-31 宣布限制、11-01 对北越全面停炸。原有 1960–75 条目保留未重复。
- **重复对象／冲突处理**：滚动轰炸的武器/战术不再另建重复页（仍指向既有 Wild Weasel
  /SEAD/实体）；F-111A 与 Rolling Thunder 战役页为新开；与既有数字（SA-2 per-kill 等）并
  存处均标注两来源口径。另：书中把“南越上空首次 B-52（Arc Light）”写作 1965-04-01，但
  常见官方早期 Arc Light 纪录有另说（多作同期/1965-06），因不属战役主线、疑点高，故本页
  不将该具体日期写入时间线，仅按需在后续跨源时复核。
- **异常**：无 OCR；PDF 副本与文本同存 raw；SCHEMA.md 全程未变（SHA 保持 `191cd2…`）。
- **检查**：全库 .md（不含 SCHEMA 计 41 个）frontmatter 合法、wikilink 全部命中（唯刻意
  文件链 [[SCHEMA.md]]／[[log.md]] 指向根文件属预期）；经 grep 复查无草稿残留乱词。

## 2026-09-02（增量摄入·DANAS 卷2 第 5 章 VP-HL 海军巡逻）

- **来源**：Dictionary of American Naval Aviation Squadrons（DANAS），第 5 章「Heavy
  Patrol (Landplane) Squadrons (VP-HL)」，海军历史中心编辑（原 PDF 元数据 John Grier，
  Distiller 1999）。
- **SHA256**：`b279ef027b5bddf73c556175e7e22ff650449cf44fd5c1486250740d8fb4b1f7`
  （查重：库内原无）。
- **资料性质**：为单章抽页断档（第 5 章，内容为奇数编号 VP-HL-1、-3、-5 三条目——
  标题写 1–5 但抽页仅含 -1/-3/-5；VP-HL-2/4 不在本 PDF）。
- **raw**：副本 `raw/papers/danas-vol2-chap5-vp-hl.pdf`；提取文本
  `raw/papers/danas-vol2-chap5-vp-hl.txt`（pdftotext -layout，471 行，未 OCR）。
- **入库决策**（用户明确）：当前库为**综合战史库**（不限于越战），本章为二战海军线即可
  正常增量扩新战争导航；组织和装备一律全局 canonical，不为了连上既有越南/SEAD 内容
  而硬造毫无历史关系的外链。
- **新建页面（8，均为新战争线）**：
  - 战源/来源：`sources/dictionary-of-american-naval-aviation-squadrons.md`
  - 战争导航：`wars/world-war-ii/index.md`、`wars/world-war-ii/timeline.md`（时间线上只有
    自该章確证、具战役/研究意义的选点；不虚构全球 WWII 总表）
  - 单位：`entities/organizations/vp-hl-1.md`、`vp-hl-3.md`、`vp-hl-5.md`
  - 装备：`pb4y-1-liberator.md`、`pb4y-2-privateer.md`、`bat-guided-bomb.md`（Bat 页整体
    定义在反舰制导滑翔炸弹、别名/口径注明 SWOD/ASM-N-2 跨源差异）
- **Index / 导航**：根 index 增战争入口 WWII 并列表第四批来源（①–④条）+ WWII 海军巡逻
  线单位装备快链；`wars/world-war-ii/index` 即以上实体入口。
- **Timeline**：见 wars/world-war-ii/timeline——1943-08-16 南大西洋 Recife、1945 太平洋
  侧（Iwo 中转、Yontan/Bat、6-26 上海损失、8-27 厚木）选点；**不过量**照抄编中队 Chronology。
- **重复对象**：库内无 WWII 巡海军 vp-hl/PB4Y 相关 canonical，新建即唯一；与现有越战/
  沙漠风暴内容无实体重复；按用户要求不为此建 theater 层（数据量尚未到需要）。
- **异常**：源文本内部有一处明显异文——VP-HL-5 段 chron 把 10 May 1944 Curaçao→Hato 与
  VS-37 协作写作 “VB-142 …”，与其 Home Port/Deployment 表（VB/VPB-143）矛盾；按表格口径
  记录并留待跨源复核。卷名 “Volume I/II” 页眉冲突仅在来源页备注。
- **检查**：SCHEMA.md 未改（SHA 保持 `191cd2…`）；对新增/全库 frontmatter 全 49 个
  页面合法、wikilink 全部命中；raw 原件＋文本保留；grep 排除了草稿残留乱词。

## 2026-09-02（增量摄入·Alfred Price《Instruments of Darkness》WWII 电子战）

- **来源**：Alfred Price，《Instruments of Darkness: The History of Electronic Warfare,
  1939–1945》（2017 Frontline 修编平装；首版 1967）。文件名中文《暗中的幽灵：电子战
  史话 1939–1945》，实际 PDF 为英文原版。
- **SHA256**：`3d70594279175e0d18655107a25881b651c91e5d674817fca170fa958e66a50f`（查重：库内
  无）。
- **raw**：`raw/papers/instruments-of-darkness-ew-1939-45-alfred-price.(pdf|txt)`；
  文本 pdftotext -layout（11,346 行，未 OCR）。
- **新建页面（7）**：
  - 来源页 `sources/instruments-of-darkness-price.md`
  - 概念 `concepts/electronic-warfare-in-ww2.md`（WWII 电战体系/术语）
  - 事件 `events/battle-of-the-beams.md`（波束之战 1940–41）
  - 装备 canonical：`entities/equipment/window-chaff.md`、
    `freya-early-warning-radar.md`、`wuerzburg-radar.md`、`lichtenstein-airborne-radar.md`
  - 组织 `entities/organizations/raf-no80-wing.md`
- **更新**：`wars/world-war-ii/index.md`（把 WWII 扩展为 海军巡逻 + 电子战两线并补来源）、
  `wars/world-war-ii/timeline.md`（电子战 1940–45 锚点：波束、Gee/Mandrel、汉堡 Window、
  D-Day 欺骗、B-29/Raven 对日）、根 `index.md`（增“来源⑤”与 WWII 电战快速链/状态第 5 批）。
- **时间线**：仅新增来源正文可核查锚点（含 Coventry 14-11-40、Operation Gomorrah
  24/25-7-43、D-Day 鬼舰队 Taxable/Glimmer/Titanic、B-29 APR-4 等）；未机械照抄逐日。
- **Index**：WWII 战争索引增加 战役/行动、概念、装备、组织各节链接；不向既有越南/海湾语料
  强搭历史无关链接（二战电子战与 SEAD 之承续另以 concepts 页中一句言明，双方同概念层互链，
  不制造单位级假关系）。
- **异常/宽记**：RAW 原书名与中文文件名不同语言；涉及 Oboe/H2S、100 Group、Naxos/F&S 等系统
  的逐项细节多在后续章节正文，本次未专开装备页完整者，均以“概念页存名 /正文为准”处理，
  留待再按章节细读时建页。个别英文专用语（如 “星条诱火、8 5×4、0sp…”—中文转写）见各页
  原文核对。
- **检查**：SCHEMA.md 未变（`191cd2…`）；全库 57 pages frontmatter 合法且全部 wikilink
  命中；raw PDF＋提取文本均存；无草稿残留乱码（个别中文误字已在最终扫尾修正）。

## 2026-09-02（增量摄入·Air Power Review 10-1《RAF 电子战与德国夜轰战》）

- **来源**：Sqn Ldr Rob O’Dell RAF，“To What Extent Did Royal Air Force Employment of
  Electronic Warfare Contribute to the Outcome of the Strategic Night Bomber Offensive
  of World War II?”，RAF《Air Power Review》Vol. 10, Issue 1（2007），pp. 97–118。
- **SHA256**：`dad55161e489ecfd089295961eb7a9c30ee9e3bc63d497a7b42cca8c0befc674`（库内查无）。
- **raw**：`raw/papers/apr-vol10-iss1-bombercommand-ew-odell.(pdf|txt)`；文本 1,153 行（未 OCR）。
- **源码页**：`sources/apr-vol10-iss1-odell.md`（期刊文章）。
- **增量更新（第二来源叠加，按 canonical 边界）**：
  - `concepts/electronic-warfare-in-ww2.md` —— frontmatter 增 sources；新增“RAF 战略夜轰战
    四阶段（APR10-1）”小节（09-39~12-41 僵持 → 01-42~07-43／07-43~03-44／04-44~05-45；
    核心论点：电子战为夜防瓦解与战役可维持第一因素；Post Mortem 1945-06 试飞证明）。
  - WWII 时间线 `wars/world-war-ii/timeline.md` —— 新增 B1 段：Gee 首发（42-03-08/09）、
    PFF 成立（42-08）、Mandrel/Tinsel 首次（42-12-06/07 Mannheim）、H2S 首发（43-01-30）、
    Oboe 泄密（44-01）、柏林战役损失合计 1,047+1,682（43-11—44-03）、最大单夜 纽伦堡
    44-03-30/31（11.9%）、Gisella（45-03-03/04）、Post Mortem（45-06）等 RAF 侧量化。
  - `entities/equipment/window-chaff.md` —— sources 增；新“数量与片长（第二来源）”小节
    （汉堡 24/25-07-1943：746 机约 9200 万条、1.5%→连环损失回升，及 27cm 条压制 53.5/61cm）。
  - **复核**（仅 sources 增补，无正文改变）：`wuerzburg-radar`、`freya-early-warning-radar`、
    `lichtenstein-airborne-radar` 各把本文列为第二来源。
- **Index**：`wars/world-war-ii/index` 来源＋战役导航；根 index 增“来源⑥”并在状态记第 6 批。
- **时间线**：本文日期若与 Instruments 细节措辞有出入以各自原文并列（已在时间线末注明）。
- **异常**：PDF 无标题元数据（PyPDF2）；依据文内页眉识别卷号/页码。本文为单一作者 RAF
  评估，其观点仅作 RAF 侧分析、非全局定论。
- **检查**：SCHEMA 未改；全库 frontmatter／wikilink 通过（58 内容页＋）；raw 已保存。

## 2026-09-03（摄入·《鹰击长空——志愿军空军在战斗中成长》/朝鲜战争线·第7批）

- 来源：刘亮《鹰击长空——志愿军空军在战斗中成长》（共和国故事·抗美援朝全纪实），
  PDF SHA 42052312…04b；raw/papers/yingjichangkong-pva-airforce.txt（2,161 行·未 OCR）。
- 判断：全库无朝鲜战争内容 → 新开 战争线；叙事为中方口径宣传体，数字/战果按原书转写、
  冲突与明显矛盾（如王天保段落日期）作“版本分歧”留注。
- 新建：# korean-war index+timeline；# sources/yingjichangkong-pva-airforce；entities：
  装备 mig-15、f-86-sabre、polikarpov-po-2；部队 pva-airforce-korea；事件
  daehwa-island-bombing-1951；人物 li-han-pva、wang-hai-pva —— 共**10 个新文件**。
- 更新：根 index.md（战争入口/第 7 批状态/来源⑦/快速导航）。
- 后续可扩展（暂未建页，先书于时间线）：张积慧/戴维斯、韩德彩/费席尔、赵宝桐、刘玉堤、
  刘亚楼、聂凤智等个人 canonical；米格走廊地图概念；美远东空军/苏联援朝航空史实校勘页。
- 检查：SCHEMA 未更；需重跑全库 wikilink/frontmatter。

### 2026-09-03（权威全史《抗美援朝战争史》—连续任务之“首批·战争主干”）

- 来源：军事科学院军事历史研究部《抗美援朝战争史》（三卷本电子版），sha 307ffb63…；
  343 节拆分于 raw/papers/korean-war-history-cams/extracted/OEBPS/Text（j01/j02/j03 卷章
  ＋biao/序列表、tu、end 等）。
- 处置：大部头官方全史，用户决定按“同一持续摄入任务”分批进行；本批只建战争主干
  （来源页＋索引＋综合时间线＋地面战役/谈判 canonical 事件页），每批断点入本 log。
- 本批已读范围：# 一至三卷各关键章开篇（一、二卷五次战役主线与决策章节；三卷谈判、
  夏/秋季攻势、上甘岭、金城、停战签字、战俘议程、绞杀战与细菌战章节导语；全书结束语）。
- 新建：# sources/kangmeiyuanchao-zhanzhenshi-cams-milhistory；将 korean-war index、
  timeline 改建为官方全史综合主干（原空军成长叙事作为〔空〕来源并入）；事件页
  first/second/third/fourth/fifth-campaign-korean-war、korean-war-summer-autumn-
  offensive-1951、shangganling-campaign-1952、kumsong-campaign-1953、
  korean-war-armistice-1953 —— 本批地面“战争主干”。
- 下一批续读起点：从本批“战役导语”往下展开对应的正文细部 —— 第二卷（四次-五次战役
  转移阶段、第二卷后与第三卷）的逐节作战细账；第三卷 ch03-22 谈判议程与空/防空/铁路/
  细菌战细账、反登陆作战准备、夏季反击各阶段与金城细根、战后/撤朝 ch23-30。断点以
  “本 log 之批序号＋read 节清单”为续。
- 待办：全库 wikilink／frontmatter QC 于“主干批·末尾”最后一次统一执行。

### 2026-09-03（同一任务·第二批：战役细部与反绞杀canonical）

- 续读（官方全史·核心细部）范围：第二卷五大战役细部（ch02_04-06 首役-云山、ch05_03/04
  第二次-德川清川江、ch06_04/05 长津-陆战1师南撤、ch18_02/ch19_03/ch20_02/03 第五次
  战役-县里与转移）与第三卷细部（ch24_03 夏季反击一阶段、ch26_04 金城反扑、ch18_04 上甘岭
  第二阶段、ch10_04-07 反绞杀战四系统、ch08_02/03 秋线文登里等）。
- 新增 canonical：events/strangulation-war-counter-1951-1952.md（绞杀战/反·体系与美第5
  航空队损失月表等）。
- 增量补充料块（据细读，作“补充资料（第二批·细叙）”小节加到既有事件页面，未重描正文）：
  second/fifth-campaign、shangganling-campaign（修正第二阶段为 10-21～29，并记美7师
  伤亡超2000撤出、转授韩2师）、korean-war-summer-autumn-offensive-1951（补文登里反坦克
  大队等）。
- Index/timeline：朝鲜战争 index 增“绞杀战”子项；综合时间线补引该页。
- 本批断点后，继续第三卷其余细部（细菌战/防疫 ch13_03-05、谈判各议程 ch03-05/09/14/15、
  上甘岭阶段一/三细节与 12 军投入、反登陆 ch21-22、1953 夏季反击二/三阶段细账与金城各支、
  停战协定后 post-ceasefire (ch27_04-ch30)）。
- 校验：SCHEMA sha 不变；全库 wikilink/frontmatter 需于批尾复查。

### 2026-09-03（同一任务·第三批：战俘协议终点/战后-重建撤军/第三卷尾声）

- 续读：细菌战（ch13_03/04/05 控诉声明、调查团、防疫组织）、克拉克接任与“空中摧毁战”水丰
  轰炸等（ch15_01）、战术反击第一阶段（ch17_02 老秃山等）、反登陆判断与准备（ch21_03/
  ch22_02/08 匪特清剿统计）、夏季反击二三段与谈判终点（ch24_04/05/06 美撤“就地释放”、
  6-04 复会南日宣读草案）、金城后各军配合（ch26_05）、庆祝胜利与停战后维持（ch27_04、
  ch28_01/04）、战后经济援助与重建（ch29_01）、志愿军撤朝（ch30_02）、全书结束语意义（end_03）。
- 新增 canonical：# aftermath-korean-armistice-1953-1958.md（停战后维护/重建/撤朝 1953-58）。
- 增量更新：korean-war-armistice-1953（新“补充资料”：战俘“就地释放”之争与 5-25 撤案、
  6-04 复会终点）；korean-war index/timeline（终结与战后段改写并链战后页）。断点已记于此批。
- 其余新读素材（战术反击阶段/细菌战调查/反登陆匪特与动员等）已获；除明显可并入时间线的
  日期外，多数（细菌战申诉程序、匪特数据）暂不整页展开：细菌战内容以“双方攻讦点·按官方
  史口径存目”，避免单侧专页。后续可做“主题深化批”。
- 本库官方全史主干至此（起于入朝、止于撤军）已通读至第三卷末：核心主干批次(1-3)收束。后续
  批次可按“主题深化”做补充（详读校核各节细账、增 person/org canonical），亦可停。
- 校验：SCHEMA 未更（sha 191cd20f…）；全库 wikilink/frontmatter 复查见批尾。

### 2026-09-03（同一任务·第四批：主题深化·定量校核）

- 续读定位（未展开的正文结果段）：横城反击结果（ch12_04）、上甘岭战役全程定量（ch18_05尾）、
  第五次转移防御（ch20_03）、主力转移（ch12_05 砥平里等作取舍）。
- 增量补充资料（第三/四批给既有 canonical，未增页无重复实体）至：fourth-campaign（横城反击
  定量：2-09部署·9个师、2-11 17时发起、118师1300余、39军117师2300余等、后砥平里受阻），
  shangganling-campaign（43天总量、志愿军伤亡约1.1万、打退营上25/营下653次按书口径、597.9/537.7
  恢复顺序）等。
- 目的：官方全史主干已三批贯通；本批转入对重要战役页做“结果/数量”校核性补充。未建新 canonical。
- 待：分批接续可对第二/三卷未细读之“非决定性”段落（国内动员/中苏后勤协商/停战执行期细节）
  继续主题深化；或作整库 final QC close。

### 2026-09-03（新来源·连续任务批1：Alfred Price《美国电子战史·卷一》（OCR 主干线）

- 来源：Alfred Price, THE HISTORY OF US ELECTRONIC WARFARE Vol.1：
  "Years of Innovation — Beginnings to 1946"（美国老乌鸦会1984；中译总参第四部；
  扫描 OCR PDF 520 页）。sha ba7b1ed7…。
  raw：raw/papers/us-electronic-warfare-history-vol1-alfred-price.pdf + …vol1.txt（16,413 行）。
- 处置：大部头（17 章 90 万字符）按“同一连续摄入任务”分批；用户确认本批先主干线并跨章节
  案例地图，后续按章续（OCR 错字甄别、标〔OCR〕）。
- 本批已读/主要据：该书前 17 章主题主导语（ch1–17 界面 overview）、ch2（RRL成立）、ch3
  （初战 HF-DF DAQ 等）、ch5（英-美设备代号澄清 + 地毯APT）、ch8（1943-12 八航空队首批
  使用“窗”、四个月量级、美 482 大队雷达领航）、ch17（RRL 统计/关闭等）。
- 新建：# sources/us-electronic-warfare-history-vol1-price；# org us-radio-research-
  laboratory（Harvard RRL）。
- 更新：electronic-warfare-in-ww2 概念页加“美国电子战线（主干首批）”段；WWII index（概念、
  组织、主要来源）与 WWII timeline 增 “B2 美国电子战线·首批” 段；根 index（WWII 电子战线
  行→RRL、来源⑨）。
- OCR 甄别记录：书名/人名按封面；个别字按上下文校正（未订正处保留），设备代号以书内括号
  为准（见来源页 OCR 约定）。
- 下一批断点：自第一章正文细读（珍珠港前美军早期无线电侦听/雷达发展）起按章推进（1→17），
  并以各章先行锚点增量事件/装备 canonical；本 log 记每批范围。
- 检查：SCHEMA 未更；全库 wikilink/frontmatter 于批末重跑。

### 2026-09-03（《美国电子战史·卷一》批2：第1章「珍珠港之前」细读增量）

- 续读：第一章正文（行526–1406 重点段落），主得：电子战原生史（内战电报假命令/1902-03 首批
  干扰截收演练）、美早期雷达演进与 SCR/CXAM 等型号、战前测向/接收起步（P-540→SCR-587、
  DAQ、DT）与 1941-12 前美方状态。
- 新增 canonical：# entities/equipment/us-early-radar-pre-pearl.md（美早期雷达至珍珠港综述）。
- 增量：concepts/electronic-warfare-in-ww2 加“1941年前起源（美）”小节；WWII timeline 加 B0
  （美雷达源起）小节；WWII index 增该 canonical。
- OCR 甄别：型号以书内相照；个别字按上下文改写字（如 U-字误、海军型号“利里”号等均取意）。
- 断点：下一批读第2-3 章（“陷入未知的领域/投入战斗”：欧战中英美雷达对抗机构成立与首次作
  战），按需在既有/新 canonical 增量。
- 关注：库已开始新增较多页——本卷仍为“主干+单页”，尽量低频次泛改，遇文误即 patch 后置。

### 2026-09-03（《美国电子战史·卷一》批3：第2-3章优先事实采辑）

- 续读：第2-3章关键技术锚点采辑（RRL 成立时间/拨款/首期组目概况、Carpet/鹤/SCR-587 职责、
  APR-1 改进、美国侧窗口试验（1942-07-柱体试验）等）。
- 精确更新：us-radio-research-laboratory 页（组建时间线 1941-12-11 海军建议→30万美元/
  6月拨备→特曼 1942-02-12 就任；四个初创组），WWII timeline B2 修正为同一时间与组目。
- 无新建 canonical（OCR 与既有重合处维护）。
- 断点：下一批 ch3 余（第3章正文“投入战斗”细节：美 HF/DF/DAQ 海上试验与首批反潜）及 ch4。
  逐批小步增量符合主源长期连续摄入，全库 page 数为既有+0（本批仅修改）。SCHEMA 不更。

### 2026-09-03（《美国电子战史·卷一》批4：ch3 尾＋ch4 导）

- 读：ch3 尾（DAQ HF/DF 实战前、博卡拉顿雷达学校、Moonshine 月光 515 中队试练与美 B-17 欧陆
  首袭同期）+ ch4 导（太平洋初次缴获日雷达、XARD 侦察接收机与“一号制止怠工”）。
- 增量：WWII timeline B2 增 Moonshine/月光与 1942-08-17 8AF 首袭同日条；concept（electronic
  -warfare-in-ww2）“美直线”blocks 补 ch4 情报起点；均未开新页。
- OCR：核对（月光/Moonshine、XARD、ARC-1=SCR-587 海军名等），首袭路由法国鲁昂（谷昂即鲁昂）；
  假编队归属不臆断。
- 断点：下一批 ch4 续（南太“一号制止怠工”作业细节）→ch5（以太小战斗，Carpet 等美制首用）。

### 2026-09-03（美国电子战·卷一·批5：ch4 南太电子侦察续）
- 采辑：一号制止怠工小队（丘吉尔/拉塞尔）至南太、首次 B-17E 41-2523 电子侦察（1942-10-31
  Esp.→瓜岛→布干维尔 11h）、鼓鱼号近海捕收等（含“首个人记录”存疑注）。
- 增量：concept（electronic-warfare-in-ww2）“情报起点”小节扩写了上述日期与机号（未建新 canonical；
  未来 CH4 细作可在专题页深化）。
- OCR：组名、机号、拉丁地名按原文核对；争议叙述注明存疑。
- 断点：ch5（“空中小规模战斗”：美制 ECM 物，含 RRL 初期与8AF等）下一步读入。

### 2026-09-03（美国电子战·卷一·批6：ch5 美国 RRL自研箔条理论 + APT量产）
- 采辑：ch5 美国侧：1942 因保密暂停空中试验仍续理论；一带箔料的散射理论（OCR 人名“查”→通行
  Chu，保留原形并注明）；远离谐振窄条截面愈大等结论。生产：APT-2(Carpet) 1943春经德尔科量产
  （百部约50万）、APT-1/3、APQ-2 投产（85-720MHz）。
- 增量：window-chaff（美国发展线小节、sources 增美卷）。
- OCR：人名、频率、代号详见正文注。
- 断点：ch6（地中海插曲：搜索者电子侦察机）下一批。

### 2026-09-03（美国电子战·卷一·批7：ch6 地中海“搜索者”电子侦察）
- 采辑：Searcher III(B-17F 42-29644) 1943-04 改装（S-27/SCR-587/APR-3+双向测向）、4-22 移防、
  5-18 首检（西西里/撒丁 Freya 122.5/125.4/129.1）、夜航 480MHz 谐波教训等。
- 增量：electronic-warfare-in-ww2 概念于美直主线加“搜索者”例（未开新 canonical；未来 Med/ESM
  专题可视累进另立）。
- OCR：机身号、频值、地名与前文一致确认。
- 考量记录：多批次在长上下文下转写偶现字渣，已逐次 patch（单文件高频改写风险）——后续会将文件
  结构每批一次性修审（read→repair）而非即兴续写以防偏离。
- 断点：ch7（加快步伐：8AF 干扰作业展开）等下一批。

### 2026-09-03（美国电子战·卷一·批8：ch7 8AF地毯干扰首次作战）
- 采辑：482 领航大队（9-27 埃姆登）；1943 初秋 68 部 APT-2 抵英装大队；10-08 第3轰炸师 42 架
  Carpet 机对不来梅首“编队干扰”（间隔 500kHz、cover 553-568MHz）；损失下降；德尔科 15000/年
  级合同议及；德反测→（Würzburg 反干扰应变逐后）。
- 增量：WWII timeline B2 中原“1943-10 首用”条目改/细化为上述带日与机制（未开新页）。
- OCR：机型编号与频率可按 ch7 原文核对；命名个例谨慎。
- 断点：ch8（推进·迂回：1944 干扰升级与窗用量）随后。

### 2026-09-03（批9·ch8 推进/迂回：1944 干扰、窗量与德反制）
- 采辑：美 8AF 1943-12 首用窗数量曲线（40/125/260/355t 1944,2-5月）；第15航空队 1944-03 起复用；
  Carpet 在用/损失/在途（4-06：202/101/201）;德加装“维尔茨劳斯/纽伦堡”〔OCR〕反窗件；94BG
  改装 B-17 频率监视（APR-4）。
- 增量：WWII timeline B2 加“1944春配套演变”条（未开新页）。
- OCR：反制机名以〔OCR名〕框定，不硬译对史实名。
- 断点：ch9（“霸王”作战计划·ECM 奥维）随后。

### 2026-09-03（批10·ch9「霸王」ECM/欺骗规划；第二来源合注）
- 采辑：霸王 ECM 总体目标（防早期预警/扰德空指挥+佯攻、“每目标外≥2处假目标”等）；TRE“乒乓”
  DF 三高精度（<¼°）置于英南定法国岸 Freya；反雷达 1944-03-16 No.198 台风(奥斯坦德-Wassermann)
  例。与英源一致处标第二来源并补注本目。
- 增量：WWII timeline（1944 D-day附近）补“〔美卷ch9第二来源〕”合注（未开新页）。
- OCR：乒乓等译名按书中；不硬译。
- 断点：ch10 日本雷达：堪/逐步——下一批。

### 2026-09-03（批11·ch10：对日雷达与电子战 1943）
- 采辑：对日初期 ESM/ECM（一号队/卡特琳娜；安姆奇特卡伯德角式干扰站 APT-3+AM14-140W对基斯卡、
  APQ-2 疑300MHz→误判；雪风/蒙彼利埃早期 RWR 不对称）等。
- 增量：electronic-warfare-in-ww2（美直-线）补“对日早期电子战（ch10）”；未开新页。
- OCR：舰名频率等按原书校对并说明。
- 断点：ch11（B-29 对日/中国，ECM 预留与电子侦察）随后。

### 2026-09-03（批12·ch11：B-29 对日 ECM/侦察 第二来源附注）
- 采辑/实证附：58th BW 1944-04 转 Kharagpur（克勒格布尔）；B-29 入役预留 ECM 布线；每约 4 架
  其一为 ECM 机（APR-1+APA 分析）；克罗斯利产 TV-系批量（40~1000MHz）〔型号未稳〕；日外海谐波
  疑判。
- 增量：WWII timeline（1944-05 B-29/Raven 行）附「美卷ch11 第二来源」补充。
- OCR：承书留号并注明未核实。
- 断点：ch12（干扰升级：欧 ECM 演进与 8AF；APQ-9 及其对抗 1944）下一批。
### 2026-09-03（批13·ch12 欧 ECM 干扰升级与 APQ-9）
- 采辑：8AF 地毯阻塞/瞄准双增（1944-10 大量涌抵；年底 12-31 阻塞约3460/瞄准507 架装表）；调谐
  式 APQ-9 需机上对抗操作员单频对;每欧箱条月耗约千吨（第15 航空队亦续增）。
- 增量：WWII timeline B（美卷 ch12 节）新增行；OCR 表数字按书录并注对原版表。
- 断点：ch13（欧洲的结局：德厘米波火控与盟军 ECM 1945）下一批。
### 2026-09-03（批14·ch13：欧洲结局·厘米波/APT-5）
- 采辑：德 cm 迟滞（1943 H2S 获起、3 300MHz 埃格兰样机 1944末试）；美 APQ-9 1/4机、APT-5(15W)
  零星、APT-2 仍主阻塞；1945 欧末美重轰以箔+干扰压制 Würzburg/曼海姆。
- 增量：timeline 欧战 1945-早行加（第二来源亦给出埃格兰等细节一致）。
- OCR：机型/数值按原卷并注；与英源一致处注明互为印证。
- 断点：ch14（越岛/对冲绳 EW与TDY/SPT）下一批。
### 2026-09-03（依请求新增）：二战美国电战设备合集 canonical
- 新页：entities/equipment/us-ww2-rf-equipment-compendium（干扰/测向/侦察接收汇总指路合集，
  类似美早期雷达页；型号表 A-D + 箔条交代引）。
- 接线：WWII index 装备技术入链。源依 Price 卷一（含〔OCR〕；单型号丰足后另拆页）。
- 注：CH 分批待续 ch14-…。
### 2026-09-03（批15·ch14：越岛/太平洋海军 EW(TDY/SPT)
- 采辑：佩莱利乌-昂奥尔(1944-09)机改干扰；1944-10 台海日夜间雷达引导鱼雷（G4M 150-160MHz、Ki-67
  200-209）：美 TDY 高频不足→改磁控管下延、SPT-4 阻塞 152-157MHz 等（1944-10-19）。
- 增量：WWII timeline（1945 太平洋段上插）ch14 摘要（OCR 个别舰名原书复核）。
- 断点：ch15（太平洋战争高潮·B-29/EW 展开）下一批。
### 2026-09-03（批16·ch15：冲绳 EW（1945）雷达哨戒收尾
- 采辑：冲绳岛约12部警戒雷达信息；30艘登陆艇改装 SPT-1/4；Estes 旗舰记录马克VI(153/PRF1k/8us)；
  TDY 接收上限约116MHz；雷达哨戒36DD（6沉13伤重5轻伤）；6月后敌势减。
- 增量：timeline 太平洋（1945）补冲绳 EW 条目。（OCR 小数复核待原版）。
- 断点：ch16（太平洋高潮·美国本土高功率/设备收束）+17 追溯 = 下批即收尾卷。
### 2026-09-03（批17·ch16-17【卷1收尾】）
- 读 ch16/17：终战试验装备（APQ-20/21、大象 Elephant 舰载 1945-02、ARQ-11、小鸟、迷魂药、APQ-14
  反辐"蛾"）及第17章全卷统计/效费（RRL 1500万+71万、订购额2.42亿、试件2800/463、箔条-曳光3万吨、
  每$1→$13；估挽救欧洲-600重轰/太平洋-200 B-29 等）。
- 增量：us-radio-research-laboratory 页面补充/效费与终战新机小节（与既有合集指路互参）。
- 【阶段完成】《美国电子战史·卷一》逐章分批读毕 ch1–17（连续任务结束；如需对单型号深化建
  canonical 可后续批次），SCHEMA 未变。
### 2026-09-03（新源·卷二·批1：来源＋章图主干）
- 新源第二卷：Alfred Price《美国电子战史·二卷 复兴的年代 1946–1964》（总参四部/解放军1993内）；
  sha 3b643b1a…；607p；raw 文本 18,824 行（约1.0M字符）20 章。
- 建立 sources/us-electronic-warfare-history-vol2-price（OCR 约定、章行位图、跨页互参）。根 index
  记来源⑩。逐章分批续按用户指令入（本页即“卷地图主干”）。
- 断点：可从 ch1（第一章 1946–47，行≈405 起）逐章续读。
### 2026-09-03（新源·卷二·批2·ch1：铁幕降落及其苏军雷达/火控基线）
- 新概念页：concepts/electronic-warfare-cold-war-1946-64（战后冷战早段主壳，接卷二主源；
  根 hub 挂接）。
- 内核（ch1 1946–47）：战后美裁军/苏复员后约300万；美 1946 评估苏空海不足以远征、战略远轰无
  雷达；附录C始列 1946 苏雷达/火控（RUS-2 75MHz/战时约600；P-3 约72MHz；英GL马克/SCR-545/548
  高炮火控的苏仿与改频等 待续 OCR 核定）。以上初记概念页首读（标〔OCR〕少量）。
- 断点：ch2（1948–1950，行≈1046）。
### 2026-09-03（卷二·批3·ch2：1948–50 冷战时-克隆雷达与SAC疲弱的ECM）
- 概念页 电子战冷战中段续二节：
  ①图-4事件+苏克隆雷达（SCR-584E→COH?、英291/285、美SO-13及 Г-20"标记"⇄CPS-6 辐射室手册公开技术
    逆向）。──〔含 OCR 名待续复核〕
  ②SAC 1948 清单/后勤紧缩/李梅 1948-10 / 侦察 F-9/F-13、原子护航≥4、1949-05 ECM低频缺口与 APT-10
  25 部覆盖 2700–3350 等；SAC 另恢复电子对抗军官。
- 断点：ch3（1946–1950 另线，行≈1886）。
### 2026-09-03（卷二·批4·ch3：ELINT 缘起 - 外围侦察）
- 概念扩展：美机/地/海军舰 ELINT 缘起（1946-09 B-17 格陵兰；德/奥 7499 B-17；B-29"靶机"与
  APR-9；奥柏林走廊侦察、72/324、训练7888；远东 RB-29 海参崴-嘉手纳与中国雷达序；VP-26 邮班；
  1950 陆军三"气象幌子"站；月球回波 最早被动；1950 被击落首例──收紧的冷战。
- 断点：ch4（1950–1951，行≈2818）。
### 2026-09-03（卷二·批5·ch4：朝鲜战争开段 ELINT，空窗期）延伸概念
- “无雷”窗前：RB-29 黄海-夜越朝-横田、300英里推进无雷达；元山文件认出苏仿英291（基乌伊
  伊斯-俄音译Hughes）。1950-11 米格-15伤第31照相RB-29→喷气化；改91 SRS；SCR-270+П-3平壤等；多
  摩-机-18 “4-脉冲组→”威尔逊逐脉冲摄影”判无意故（维保评估用途）。
- 断点：ch5（1950–1953，行≈3188）。
### 2026-09-03（卷二·批6·ch5：改革与 SAC EW 专业化）概念续
- kil半岛战带动研究、应急采购法；SAC1951末842架、61批专设EW操作员、李梅EW纳入考核/战略考核中队；
  苏微波标记少装；APR-4/9、ALT-5/6、B-47舱包；B-52无EW位→Perry备忘录促李梅；本土防空网+F89/F94(休斯E-1)。
- 断点：ch6（1950–1953，行≈4185）。
### 2026-09-03（卷二·批7·ch6：外围侦察2 - "标记"雷达曝光/ELINT平台重乘）
- concept续：东京→莫斯科伊兹梅洛沃拍"标记"（Г-20/CPS-6基、5频≠6）等震动至1952-06黑海6部组网；
  П-8 70-73；火控米波/E 频渐别/换回RUS-2实物；324→55联343 RB-50G; 7499换C-54;米格-17火控E波段收；
  海军 P4M-1Q 水星桑莱/利奥特 VW-1/VW-2；攻击案5（含1951-11-06 VP-6 P2V）。
- 断点：ch7（1951–1953，行≈4626）。
### 2026-09-03（卷二·批8·ch7：朝鲜空战 ECM 战术实战）
- concept续：朝重估 PY/П/COH-2；B-29 19/98/307 收窄运用ARQ-8/AM-33；Shoran-干扰节奏、探照灯对抗
  与郭山/水丰（1952-09-12 30→45架紧凑编队+箔条+瞄干）；RR-3A/U与RR-20A/U可靠度改进；陆战队夜战
  防夜袭；附录G（被照159/跟踪36 23%等）。
- 断点：ch8（1946–1955，行≈5586）。
### 2026-09-03（卷二·批9·ch8：EW专属新管/天线部件1946-55）
- 概念续：CW磁控(QK946)…COH-4烧穿5频→TWT(斯坦福S-100/110/130,远胜APR-9)；欺骗vs噪声研究；
  BWO(W-G-D; 400M-18G), QRC-23可靠性10h/电弧/油/天线螺旋螺旋缺口; 高截获接收机/回答式干扰/CW/无源
  TOA等铺路。
- 断点：ch9（1954–1957，行≈6430）。
### 2026-09-03（卷二·批10·ch9：欺骗/自动EW與安装）
- concept续: 1954红场图-16/米亚-4; 城市"分布抑制"异议(400+)与玻纤箔条; ALQ-3自搜压/ALQ-14/ALT-2;
  斯坦福CW相参/门拖(莫古角),桑德斯回答式; B-52机头45°天线/失电损/半月天线1955; SAC 900架+盟队,
  ALT-3取消; 376联对北美防空演练。
- 断点：ch10（1954–1959，行≈7678）。
### 2026-09-03（卷二·批11·ch10：对苏周边/越界收集与涉险）
- concept续：无漂气球载雷达录至北太平触发投舱(AMF/西屋)、U-2授权艾森豪威尔1954-11/首飞1956-07-04、
  9112分队/日本队；RB-47H与ALR-8(50-10750MHz)；友邻共9机伤/投(VP-22 1954-09-04、RB-29 11-07、VP-9、
  VQ-1 1959-06-16)、切萨皮克湾月反射站1957/新苏160MHz警戒等。
- 断点：ch11（1947–1957，行≈8399）。
### 2026-09-03（卷二·批12·ch11：自动化/高截获ELINT接收）
- concept续：1956前标准APR-9+APA-17/64铅笔记录、火控常漏；高截获(德·罗莎FTL即时方位/电影记录
  Della Rosa B-50→1955末APD-4装RB-47H/RB-66C；APR-17=APR-9+14；局限饱和&胶卷人工读±500；DLD-1/
  ALD-4磁带记录前端铺垫。
- 断点：ch12（1956–1958，行≈8811）。
### 2026-09-03（卷二·批13·ch12：苏SA-1莫斯科环与TWS火控研究）
- concept上增：SA-1 1957运用、莫斯科双环~30阵(各60枚立)、火控"约-约"(橘皮三角形)边跟扫3批/TWS、
  量规/点头测高目标指示; 美国的摸底（密大磁带化告警/海军&GE模拟器莫霍克河1958）;抗核/多对空强点与
  "功率散向天空"弱点及1960-11协会公开前情难全。
- 断点：ch13（1957–1959，行≈9145）。
### 2026-09-03（卷二·批14·ch13：SAC喷气化/ECCM与训练）
- concept增: B-52十四座干扰ALT-6B/7/8、B-47低空与梯城(60架303/509)阶段V、奈基-大力神1958-01 &
  霍克多频/MG-10数据链, ECCM培训观 - 海军TF-1/EC-1A(RED) VAW-33/13东西岸内容。
- 断点：ch14（1954–1959，行≈9920）。
### 2026-09-03（卷二·批15·ch14：ALQ-27 - “走太远”）
- concept续: 斯佩里50初半/全自动;CW200-300/脉冲1000W TWT三级、ALQ-5信道化祖型;29k磅过度→
  1959-09李梅取消、$1.4亿;KC-135减配试好废弃/信道化到埃格林;ALE-24(伦迪=TWT推动)/B-1 ALQ-161。
- 断点：ch15（1957–1962，行≈10530）。
### 2026-09-03（卷二·批16·ch15：ELINT自自动化2 ALD-4/ERB/GoldenFleece）
- concept续：ALD-4(RB-58系吊舱/200晶视频道100M-16G/龙伯-方位/数字磁带+GSQ-17Finder)银王装RB-47H
  1961入役；DLD-1全晶体管；粗vs细粒&ERB-47H×3；金羊毛→ASD-1/USD-7 RC-135原型1961、量产RC-135B
  1967(自动化约20年)；RA-5C 1964/IOIC(霍尔库姆)。
- 断点：ch16（1954–1962，行≈11046）。
### 2026-09-03（卷二·批17·ch16：红外威胁IRCM开端）
- concept: 猎鹰/响尾蛇1954、赖特四路(闪烁/拖曳/投放→最后主); PbS虚警; MgNaQRC-30/35石墨弃;
  Mg+Teflon更优;ALE-14试1956埃格林; ALE-20 1961 SAC;AA-2 1958金马实战响尾蛇称31仅存疑;
  QRC-125/126红外告警仍虚警未深入。
- 断点：ch17（1959–1960，行≈11365）。
### 2026-09-03（卷二·批18·ch17：60s初 快速配装与新战术）
- concept续：QRC入库ALT-13/16(E/F/D返波)+ALT-15取代ALT-12(A)、Hallicrafterss独产1960线；
  B-52显配表(10×ALT-6B+APR9/14等)、ALE-24/25; 低空静默战术&B-47重训/B-58三人及防御者、
  GD沃斯堡评估&ALQ-24设; 战术空军薄(老T-33/B-26/29); QRC 60s末取消。
- 断点：ch18（1961–1962，行≈12315）。
### 2026-09-03（卷二·批19·ch18：行业复元;模拟台与1962 ARD-15 空中测向）
- concept续: SADS-2/FlintStone(扇歌代)…F-100/105大吊舱、B-52G起录/ALT-6B组；麻-雀反辐射(ARM早期);
  ARD-15(L-20海狸HF测向)1962新山一标6处越共指挥→第3无线电分队首集体嘉奖&扩到~100架。
- 断点：ch19（1960–1964，行≈12977）。
### 2026-09-03（卷二·批20·ch19：U-2/SAM成熟与U-2 被击）
- concept: U-2 ELINT包(QRC-192、COMINT100-150、Ⅳ型150M-40G 570lb)；SA-1围莫/列SA-2扩城；
  1960-05-01斯维尔德洛夫斯克被SA-2击、鲍尔斯跳伞被俘；1962-10-27古巴4080联U-2被击、驾亡
  ——纪录之二；对中/古弱防空续侦。
- 断点：ch20（1962–1964，行≈13715；于此应接近卷末）。
### 2026-09-03（卷二·批21·ch20 末章：走向冲突 1962-64 及卷完成）
- concept末篇: 古巴危机U-2/SA-2(10-27击,4720?U-2驾亡)、SA-2阵地情报、ALQ-49(G转发)兴趣；
  海军警預击E-1B演练; SAC低空化完(1963末);QRC-160 GE 1963、模拟器更名AF;1964北部湾VQ-1监视。
- 【卷完成】《美电子战史·卷二》(ch1–20 文读毕 1946–64)；其后附录 A–L 为表/参考文献（本批未整
  批摘，需时按需采用）；SCHEMA 未变。
### 2026-09-03（Price Instruments 中影视题为“暗中的幽灵…”；依请求建行动专页 6 张）
- 该卷实为已入库《Instruments of Darkness》2017 英版之同(sha 3d705942…)副本 → 不重建源；据此新建：
  events/millennium-raid-cologne-1942（千机科隆）、events/moonlight-sonata-1940-x-beam-raids、
  events/bruneval-raid-1942-capture-wuerzburg、entities/equipment/german-beam-nav（Knickebein/X）、
  people/rv-jones、people/john-frost。
- 增量：battle-of-the-beams 关联尾纳入上述指要；WWII timeline 1942 段补布吕/科隆/月光指针。
- 全文 93 内容页、wikilink 0 断；SCHEMA 未改。
### 2026-09-03（WWII 按战区分类导航；非新源）
- 依 SCHEMA 5.2 为 WWII（大规模战争）加 Theater 层，并按其规范分类（canonical 事件/实体仍全局单页，
  仅以 Index/MOC + 分区时间线导航）：
  wars/world-war-ii/theaters/{european-theater,pacific-theater,north-atlantic-theater}/{index,timeline}.md（6 页新增）
  - 欧洲(含地中海)：光束战/布吕讷瓦/千机科隆等 + RCM/装备/RAF 主题
  - 太平洋：对日 EW/B-29/冲绳等（登记于主时间线 44-45 节）
  - 北大西洋-海区：VP-HL/DANAS 军建设置（VP 跨区又属太平洋后期视 说明）
  - 东线-苏德待后续资料充盈再开战区（如用户所述）
- WWII index 更新：新增“战区”段并补月光/布吕讷瓦/千机三条行动链、german-beam-nav、rv/frost 人物链。
- 检查：99 内容 .md、wikilink 0 断；SCHEMA 未改(191cd20f9952)。
### 2026-09-03（F-105 WW vs SA-2 "再次摄入"增补——补缺专页，sha 6472f403d60…）
- 复核：源已在库（sha 6472f403...）；本批聚焦此前未单独建页之行动/人物。
- 新建（5）：events/operation-spring-high-1965（SAM 6/7,6×F-105D 损/假阵诱歼）、
  events/operation-proud-deep-alpha-1971（50 Shrike+10 AGM-78>5 Fan Song+3 EW）、
  events/pepper-01-loss-1966（首届 F-105F EWO 阵亡 Morgan/Hestle）、
  people/ingwald-haugen（Problem Child/四机 QRC-160 编队）、people/charles-morgan。
- 增量更新：concepts/sead（关联行动 专页锚）。
- 检查：104 内容页、wikilink 0 断；SCHEMA 未改（见下）。
### 2026-09-03（新源·美国电子战史·卷三 来源+章图 主干批1）
- 卷三「响彻盟军的滚滚雷声」(1964–2000) sha 97af4f8ba…；OCR 740p。原作者 Alfred Price/AOC，中译总参
  四部2002-12。
- raw: us-electronic-warfare-history-vol3-price.pdf / .txt(27,933行~1.59MB)。
- 建 source 页 + 章主题表(1情报攻击…11后卫I…17两种电子干扰系统/24来自空间窃听/26科索沃...27明天后天、
  含 OCR 目录错行注明)；root index 记来源⑪ (卷一至三闭环)。
- 检查: 105 内容页、wikilink 0 断；SCHEMA 不变(见下)。断点：ch1 情报攻击-1（正文起始约 raw 行583）后续按
  需指令续。
### 2026-09-03（卷三·批2·ch1 情报攻击-1：冷战情报搜集/遥测——并回顾线）
- 读 ch1（raw≈583-1444）：苏航迹/码追踪、CIA遥测与B-47改机、功率方向图测（高王/扇歌）与EC-121改(强盗/
  APS-20→APR-9方法)、EB-47E值更、早期天基照期(1959-02–1960-06 12次失败〔OCR〕)等；末接越南升级。
- 增量 concepts/electronic-warfare-cold-war-1946-64（尾加卷III回顾章段；OCR个别名保留）。
- 断点：ch2（一个遥远国度的危机，raw≈1445起）。
### 2026-09-03（卷三·批3·ch2 遥远国度的危机：行动与装备专页）
- 读 ch2（raw≈1445-2485）：报复循环→Rolling Thunder(1965-03)；1965 夏初始 SAM 战（F-4C 7-24 击、Spring
  High 7-27、Iron Hand 8 初出 Midway/Coral Sea）；8-21 Left Hook（火蜂无人机诱 + 3×RB-66C 方位 + EC-121 中
  继）等；早期 QRC-160-1 失误/吊舱弃 4 部 & RF-101 无效等。
- 新建 3：events/operation-left-hook-1965、entities/equipment/ec-121-warning-star、rb-66c-elint（各据源内
   越战定位+早期法注）；sead 概念行动列表补链。
- 检查：108 内容页、wikilink 0 断；SCHEMA 未改（见 checksum）。
- 断点：ch3（与地对空导弹共处，raw≈2486 起）。
### 2026-09-03（卷三·批4·ch3 与地对空导弹共处→装备专页）
- 读 ch3（raw≈2486-3419）：SA-2“扇歌”威胁里美军南海空军-海军电子防（Shoe Horn ALQ-51 往 A-4）、EB/RB66C
  “猎豹4”击落、VMJ EF-10B 伴随、A-1 EA-1F 过渡、RA-5C/ALQ-61（企业号）等；Iron Hand 阶段陆续。
- 新建装备 4：entities/equipment/{alq-51-shoehorn, ef-10b-skyknight, ea-1f-queer-spad, ra-5c-vigilante}。
  （行动本批未见全新增独立代号战场——仍处 Iron Hand/Rolling Thunder 之战术技续中，故未新开行动页。）
- 检查：112 内容页、wikilink 0 断；SCHEMA 未改。
- 断点：ch4（“野鼬鼠”初露锋芒，raw≈3420 起）。
### 2026-09-03（卷三·批5·ch4 野鼬鼠初露锋芒：行动+装备+人物专页）
- 读 ch4（raw≈3420-4118）：Weasel I（F-100F）训练/300对SADS-1；12-20 武庙、12-22 安沛遭遇；1966-04-18
  百舌鸟Iron Hand首战IR-133；首批机组列表（Lamb、Donovan诸Ewo等）。
- 新建4：entities/equipment/ir-133-search-receiver、events/weasel-combat-encounters-1965-12、
  events/iron-hand-first-shrike-1966、people/jack-donovan；sead关联行动表补。
- 检查：116 内容页、wikilink 0 断；SCHEMA 未改。
- 断点：ch5（干扰吊舱传奇，raw≈4119 起）。
### 2026-09-03（卷三·批6·ch5 干扰吊舱传奇：装备专页）
- 读 ch5（raw≈4119-4762）：QRC-160-1/1A 干扰飞机编队Problem Child、APR-25/26(含WR-300)、部署及 1966-09
  -/10 装F-105；反对-支持论证等；吊舱家族后置型不复制。
- 新建2 页：entities/equipment/qrc-160-pod-family（Problem Child 时代/1A 效果概述）、
  entities/equipment/apr-25-26-rhaw。
- 人物：本批无经可靠源新增可确证人物（Haugen 已建页；反方发言人（布里斯/t）OCR未能定名──不做）。
- 行动：ch5 未现新命名行动页级；Route Package 1 不另开。
- 检查：118 内容页、0 断；SCHEMA 不变（见 checksum）。
- 断点：ch6（措施与反措施，raw≈4763）。
### 2026-09-03（卷三·批7·ch6 措施与反措施：行动+装备+人物专页）
- 读 ch6（raw≈4763-5722）：空识别-报知（PIRAZ/红冠 距岸25mi巡洋舰）；EC-121更名College Eye(1967)、
  QRC-248 米格SRO-2应答询问(1967-05)；反部（Sidesaddle对ALQ-51A、感测“宏观”EC-121微细收）等。
- 新建3：entities/equipment/qrc-248-iff-exploit、entities/people/robin-olds（第8TFW/F-4C 越战语境）、
  events/piraz-red-crown-identification-1966（北部湾识别-报知体制 1966）；ec-121 页补 CollegeEye/红冠语境；
  QRC/APR-25-26 等已在(卷三两卷正面不重复)。
- 检查：121 内容页、相关新页 0 断链；SCHEMA 未改。
- 断点：ch7（远和宽，raw≈5723）。
### 2026-09-03（卷三·批8·ch7 远和宽：行动+装备专页）
- 读 ch7（raw≈5723-6905）：舰载有源干扰/告警（ULQ-6→SLQ-22/23/24、SLQ-12、ALR-45/50）与反舰导弹语境
  （埃拉特被 S-2N-2 冥河 1967 击沉首次舰射导弹毁舰）；ALQ-59 B-52 通信干扰机、ALR-45 等；模拟器 DEES/
  AFEWES；EA-6B 1968-05 首飞等。
- 新建3：events/eilat-sinking-1967、entities/equipment/eilat shipjam??（=ulq-6-slq-22-shipejam）、
  entities/equipment/ea-6b-prowler。人物：本章为装备综述无稳定新人名可直接立（不臆造）。
- 检查：124 内容页、相关断链 0；SCHEMA 不变(见 checksum)。
- 断点：ch8（持续时间最长的战争，raw≈6906）。
### 2026-09-03（卷三·批9·ch8 持续时间最长的战争：行动+装备+人物专页）
- 读 ch8（raw≈6906-7795）：Igloo White 传感(1968)；Commando Club Skyspot(TSQ-81, Phou Pha Thi)；
  EA-6A(1966-11抵舰港,U-Pack/ALQ-76-A箱ALT-6B噪) 与更大型 EA-6B；EKA-3B加油+干扰应急(沿至EA-6B)；
  RU-6/8系列陆搜索分队、金兰湾 Crazy Cat P2V(6架分工)等。
- 新建4：events/igloo-white-1968、entities/equipment/ea-6a-electronic-warfare、
  entities/equipment/eka-3b-tanker-jammer、entities/people/william-gardner。
- 检查：128 内容页、4 新页 0 断链；SCHEMA 未改。
- 断点：ch9（1960s中 条令/编队…见源 raw≈7796）。
### 2026-09-03（卷三·批10·ch9 情报攻击—2：装备+事件专页；修正错位段定页）
- 读 ch9（raw≈7795-8547，止 ch10 实力检验8548）：可靠高置信内容为 RC-135 信号情报族（RC-135M“战斗苹果”
  1967、串接4252战略联队约18h；RC-135E 里萨安 相控阵 7.5MW 改至1966秋；RC-135S 遥测窃听；ASD-1 大型
  机载分析+GSQ-17 地面回放）、VQ-1 EC-121 Willie Victor 1969-04-14/15 遭朝机无警示击落等。
- 新建2：entities/equipment/rc-135-signals-family、events/ec-121-vq1-shootdown-1969。人物：本章为平台/代号,
  无可靠代表性人名可立。
- 检查：130 内容页、2 页 0 断链、库内无反乱/替换字符残留；SCHEMA 未改。
- 断点自 ch9 末进入 ch10「实力检验」（Linebacker/1972 及相关装备），相应下次批续 [raw8548…]。
### 2026-09-03（卷三·批11·ch10 实力检验：行动+装备专页与既有页增量）
- 读 ch10（raw≈8548-9854）：Lam Son 719(1971-02)直升机电战检验；F-111A EW 套件(ALR-41+APS-109A 告警、
  ALQ-94 欺骗逆锥扫、ALQ-87 吊舱、ALE-28/AAR-34)；ALQ-119(Pacer Granite 反 SA-3 应急) ；ALE-38(F-4)；
  EA-6B(4机组)、SA-7 亮相等。
- 新建2：events/lam-son-719-1971、entities/equipment/alq-119-jammer-pod；给 f-111a 补 EW 套件节并按原文核
  正（ALE-38 属 F-4、不含 F-111 干扰语）。
- 人物：本章人名多“任务/采访联络官”式（如 Albert Haber、Gene Simmons）缺代表性主角级，不浅建=遵守规则。
- 检查：132 内容页、相关 0 断；全文无替换字符残留(log 一处已修)；SCHEMA 未改，断点 ch11(后卫II, raw9855)。
### 2026-09-03（卷三·批12·ch11 后卫II/Linebacker II 1972-12：B-52 防御性 EW 专页）
- 读 ch11（raw≈9855-11326）：1972-12-14 尼克松决策；12-18 起对河内/海防三昼夜最大攻击（夜间逐波等）；
  参战 B-52D/G 分第三/第五阶段 EW 改装（原书分栏 OCR 错位须对原版）；最压 Fan Song/导弹链为 ALT-68/13/28；
  三阶段机≈7部、五阶段≈10；TTR 机动三机 Z 摆；SA-3 短波多机自扰间距约束（~75 ft）等。
- 新建1：entities/equipment/b-52g-sac-ew-suite（B-52 后卫II 防御性 EW 要点，专余分栏随后源补）。
- 人物：ch11 人名（安迪·维多利亚、麦卡西上校、Roland Scott 等）皆机组/访谈见证角色，无战役主线主角-浅，
  按规则不建。
- 检查：133 内容页、新页 0 断、无 �/混杂；SCHEMA 未改（见下）。断点 ch12 新技术影响(11327)。
### 2026-09-03（卷三·批13·ch12 新技术的影响—1（1972~75）：装备页×2，人物0）
- 读 ch12（raw≈11327–12012）：电子战综合重编 EWIR 数据库、SA-6/1973 效应、功率管理与自动调谐、
  舰外快速散开销条 Mk33 RBOC→Mk36 SRBOC、陆军 RU-21 A/B/C（ARD-22 测向/ALR-32 情报吊舱/ALT-29 通信
  干扰）、CHEAP 等。本章为技术横断面、无独立战役及代表级人物（人名皆访谈/作者）。
- 新建2：entities/equipment/rboc-srboc-chaff、entities/equipment/ru-21-electric-warrior（扫描清 �/？ 残留）
- 检查：135 内容页、相关 0 断；SCHEMA 未改（191d…）。断点按 TOC ch13（≈raw12013，对应表内同号）。
### 2026-09-03（卷三·批14a·ch13 短期/近期/其他民族战争：起步——SA‑6 装备页）
- ch13(raw≈12013…)覆盖多役：1973-10 中东(SA-6 首战/以空军重损、SA-2/SA-3、ALQ-101-6/-8 限用)、
  后续 1982 贝卡/波斯湾、EP-3 静默等；按需逐役开专页（下批续）。
- 新建1：entities/equipment/sa-6-2k12-kub；正文只用原书可支撑要点(S.A-CW制导/对ALQ抗性/2600架次与50机之
  损、19单元宣称17等注明口径)。人物仍无代表级。
- 检查：136 内容页、新页0 断、无 ?/�；SCHEMA 191cd…。

### 2026-09-03（卷三批14b · ch13 续：1973-10 中东空气-SAM/EW）
- 新建 events/yom-kippur-1973-air-sam-ew（开战/前4天约2600架次·失近50机≈七分之一·静默与ALQ-101对SA-6等，全按该书ch13措词/口径收）。
- 连同SA-6页两页均0断链、无?/乱字。人物仍未出现可直接代表级的叙事主角（witness only）。
- 检查：137内容页；SCHEMA未改，下步按序续ch13余役（贝卡/两伊/波斯湾）或ch14。

### 2026-09-03（卷三批14c · ch13 续：贝卡谷地1982）
- 新建 events/bekaa-valley-1982-sam-suppression：以 Price ch13 作范例段（情报综合→假目标无人机诱开机 SAM→主攻→无人复核；作者对报道不实现象的提示）。0 断链、无杂字。
- ch13（短期/其他民族战争）主干役已覆盖：1973-10（SA-6页+空气SAM/EW页）、贝卡1982；仍余两伊时期/波斯湾等，随 ch18-22 主线将由后续批次接。全库 138 内容页

### 2026-09-03（卷三批15 · ch14 新技术的影响—2：SLQ-31/32 竞标专页）
- 新建 entities/equipment/slq-31-slq-32-1976（1976 莱希号CG-16 双样机实舰对比；Rotman 透镜 vs 喇叭阵列；含 WLR-1 前置背景）。已清正文少与标点。
- 全章以产品/采办为主，无独立命名行动、亦无代表性主角级人物（多为军种采办/访谈人）—不臆建。
- 检查：139 内容页；0 真断；SCHEMA 191cd20f951e9952。

### 2026-09-03（卷三批16 · ch15 情报攻击 3：S300 / 米格31雷达 2 页）
- 读 ch15（raw≈13694-14482，1971~1991 SIGINT 主段）：SA-10/S-300（80年代替代SA-5、Flap Lip 相控阵）、米格-31 Zaslon、TR-1/RTASS-TREDS、MASINT、1989德军入西德等。
- 新建 2：sa-10-s300、mig31-zaslon（均只有 Price 卷III 章内要点，0断链/no?/no-乱）。
- 其余（TR-1/RTASS 等）及命名行动/代表人物的出现与否留卷内相应小节续；检查 141 页；SCHEMA未改。

### 2026-09-03（卷三批17 · ch16 新技术影响3 摘记：EA-6B 型号沿革增量）
- ch16(raw≈14483-15854)为 70/80 年代产品/项目综述（ALQ-161A、ASPJ/ALQ-165、EA-6 EXCAP/ICAP、TLQ通信干扰族等），无独立行动、亦无代表性人物（人名皆项目官，如 Monte Correll 因提 B-1B 意见停权；不浅建）。
- 本步给既有 ea-6b-prowler 补：EXCAP 1974-01 首飞；ICAP 1977-04 上舰/达 C-J；基线 ALQ-99+ALQ-92。未必要新专页的其余则留按其整条目。
- 页数仍 141；SCHEMA 未改。

### 2026-09-03（卷三批18 · ch17 两种电子干扰系统的故事：ALQ‑165 案例专页）
- 新建 entities/equipment/alq-165-aspj：完整研制/试验(1985样机→AFEWES/帕图克森整合1986)、拨款中断(87冻结)、20 套产品验证/1989-12 首交、空/海分道(1991-07 36套)、OPEVAL1991-08~92-05 双指标(+30### 2026-09-03（卷三批18 · ch17 两种电子干扰系统的故事：ALQ-165 案例专页）
- 新建 entities/equipment/alq-165-aspj：研制/试验（1985 样机 → AFEWES/帕图克森整合 1986）、87 春冻结、20 套产品验证与 1989-12 首交、空海分道（1991-07 36 套）、OPEVAL 1991-08 至 1992-05 双指标（+30% 生存未证）、约 15 亿美元/136 套后裁撤；收参议员与凯泽上校引语及作者败因归结。
- 人物政策同上（项目当事人非代表性主角，不开）；ALQ-161A/B-1 此章同述（后续整页承接）。检查 142 内容页；SCHEMA 未改。
### 2026-09-03（卷三批20 · ch19 隐身探索 ：F117A & 海影 2 专页；人物无）
- 读 ch19（raw≈16884-18079；“甚低可见度”全谱）：DARPA 1974 招标→RCS 验证(1975)→Have Blue(HB1001 1977-11 C-5A 至格鲁姆湖)→F-117/4450试验群(Tonopah,C-5 转场)；Tacit Blue; Navy Sea Shadow; A-12 系线; 1980 后代 GT…。
- 新建2：entities/equipment/f-117a-have-blue、entities/equipment/sea-shadow-1980s（章内要点：长宽/吨/员、平面斜接浴缸形）。B2/N-G等按 ch 内其他专题留述。人物仍无（书中 Paul?阳氏 为佩里特别助理 name OCR 未尽稳定，不浅建）。
- 全库 144 内容页、0 断、无 ?/乱码；SCHEMA 191cd20f951e9952。
### 2026-09-03（卷三批21 · ch20 沙漠盾牌(1990-08~1991-01-17)：行动+REDCAP 装置 2 页）
- 读 ch20（raw18080-18696）：RC-135 先遣；EF-111/F-4G/EC-130 压制单元集結；远距 14-17h/6-7 次加油；REDCAP+AFEWES 对伊雷达编程之准备；电磁管制/隐蔽对抗等。
- 新建2：events/desert-shield-1990-91、entities/equipment/redcap-ew-sim（职能性言简）。人物：主章无代表级人物（伊恩·哈密尔顿为卷首引言典），不开。
- 检查：146 内容页（+2），SCHEMA 未改（191d…）。
### 2026-09-03（卷三批22 · ch21 沙漠风暴空中(上段)：TF Normandy 行动专页）
- 读 ch21（raw≈18697…）上段并提取开头（1-17 03:00 H；B-52/ALCM 远程；105th/…；Normandy 8架AH-64+2 MH-53J 引导直升低空破 EW/GCI 两站前窗；EF111/EA6B/HARM 编/跟压制）。中段以既有装备族（EA-6B RS HARM、RC-135V/W、EC-130H Rivet Fire+心理战等）描述为主。
- 新建1 ：events/tf-normandy-1991-ewgci-raid（只按原书叙事写 /不转述未载杀伤）。人物：无代表主角（巴兰考等即执行军官引述）不过度单开。
- 检查：147 内容页、相关 0 断、SCHEMA 未改；余 ch21 中段可逐批增量。

### 2026-09-05（防空 Spine · 《抗美援朝防空作战实录》新源登记＋骨架）
- 新源：陈辉亭、陈雷《抗美援朝防空作战实录》（解放军文艺出版社 2010-10 第 1 版，
  ISBN 978-7-5033-2273-0；主题=志愿军地面防空兵 反美轰炸实录）。源 PDF 505p/OCR
  （Acrobat ClearScan）；提取 txt 19,450 行≈1.318MB，35 章。我侧叙事，战果/数字按
  该书我方口径记录。sha256（PDF）aef80df97e05…（txt）1a718134ff1c…。
- 登记 raw：raw/papers/kangmeiyuanchao-fangkong-zuozhan-shilu.{pdf,txt}。
- 新建：sources/kangmeiyuanchao-fangkong-zuozhan-shilu（源页＋35 章地图）；
  entities/organizations/korea-pva-air-defense（志愿军防空兵 org 骨架：前言总规模＋
  ch1-2 建 10 高炮团/东北防空/军委防空司令部 1950-10-23/入朝初期主力）。
- 更新：wars/korean-war/index（防空兵线栏目＋sources 增入本源）；wars/korean-war/timeline
  （加〔防〕标目 1950-07/08/10-19/10-23 等可靠日期目）；根 index（加来源⑫与防空线枢纽）。
- 读到：前言＋ch1（全套 ch1）+ch2（精读部分，含美东轰炸背景/购炮上书/防空司令部）。
- 断点：下一批从 ch2 尾部/ch3 续读（ch3=入朝高炮掩护炮兵，含高炮14团行军故事）。
- 检查：见本批 glitch + 链接抽查。

### 2026-09-05（防空批2 · ch3 入朝首役：云山防空战）
- 续读 ch3（只要你炸不死我，我就要把你打下来；raw≈1596-2085）：高炮第1团（王思谦）
  与高炮第14团（彭宗义）入朝承担对空;夜行军难/老炮劣势主轴；云山战斗后防空战。
- 新建 2：
  - events/gaojiao1-yunshan-fangkong-1950-11（志愿军高炮入朝首役=云山 1950-11-01~03；
    11-02 9连以旧日制75mm近截首落F-84；两日本书口径击落2/击伤10余，牺牲11伤15）。
  - entities/equipment/japanese-type88-75mm-aa-gun（日制八八式75mm高炮：12炮手/入朝老炮/
    云山近截战果/换装）。
- 更新：wars/korean-war/index（防空栏目加役目/炮目）、wars/korean-war/timeline（1950-11
  〔防〕云山防空战）、korea-pva-air-defense org（关联加役炮）。
- 代表性人物甄别：ch3 主角级叙事人物多为团长级（王思谦/彭宗义已有出镜）与 9/7连连长
  （书未具名其一）；按本库“不浅建/不 who's-who 膨胀”暂不单开人物页，身份保留在事件/
  组织页内，待其在后续更反复/更代表时再建。
- 断点：下一批自 ch4（安东鸭绿江畔首战告捷）读起。SCHEMA 未改。

### 2026-09-05（防空批3 · ch4：安东鸭绿江桥防空战／王秉珩）
- 续读 ch4（安东鸭绿江畔首战告捷；raw≈2090-2556）：高炮17团（尹洪、谢慰民）口袋阵
  安东鸭绿江桥整月保卫战；同日大捷击落4架F-84E（军委11-04通令嘉奖）；美侧麦克阿瑟
  -华盛顿决策链（11-06禁→11-09安委会准）、11-08 B-29大编队、11-09~11海航F4U/AD、
  11月中B-29/5航空队连番轰炸被击退。
- 新建 2：
  - events/andong-yalu-bridge-airdef-1950-11（战役级页：11月77次对空战斗，本书口径
    击落7/击伤35，保桥成功，17团两获军委通报表扬；并记美方禁令解除与多轮轰炸背景）。
  - entities/people/wang-bingheng（高炮17团2营4连连长；ch1阵地部署＋ch4近距截击首落喷气机
    主角，按“有存在感作战指挥”建立）。
- 更新：wars/korean-war/index（防空栏目加安东役/人物王秉珩）、korean-war/timeline
  （〔防〕11-01 安东役目）、entities/organizations/korea-pva-air-defense（关联加安东役＋人物）、
  既有云山防空战/type88 页链接一致。
- 装备甄别：敌机型号（B-29/F-84E/F-4U等）为主防空对抗目标，主体跨源且材料未足，暂不建
  美机型号专页（防空侧专注高炮/探照灯/雷达装备）；待后续ch14/19等该型对我打击更多时再定。
- 断点：下一批自 ch5（保卫辑安江桥之战）读起。SCHEMA 未改。

### 2026-09-05（防空批4 · ch5：辑安—满浦桥防空战／高炮首落B-29）
- 续读 ch5（保卫辑安江桥之战；raw≈2556-3107）：高炮第4团（周承重，日式75mm老炮 18门）
  守辑安段，遭美远东大型混合编队轰炸；高炮第14团（彭宗义）由入朝返防合并编连协同；
  11-22 2连（李金贵）/3连（董兆华）以苏式85mm首开地面高炮击落B-29先例，12-06/12-19再
  落各1；12-19高炮13团(长甸河口)首战；11月三江桥全面概数与远东暂停轰炸背景。
- 新建3：
  - events/jian-mampo-bridge-airdef-1950（辑安—满浦鸭绿江桥防空战1950-11~12：4团初战
    [韩景山牺牲]、14团返防、11-22首落B-29、12-06/19续落；14团段40余次击落B-29×3/F80×2；
    11月三江桥我方击落11击伤69）。
  - entities/people/han-jingshan（高炮4团3连电话班长，1950-11辑安战中以身作导线接通被炸断
    电话线而壮烈牺牲——防空烈士叙事主角）。
  - entities/equipment/sov-85mm-aa-gun（苏式85mm：中口径主力，能打B-29，11-22辑安创地面
    高炮击落B-29首例；据书泛称，不定M1939型号）。
- 更新：wars/korean-war/index（防空役目+苏85炮+人物韩景山）、timeline（〔防〕辑安桥防空目）、
  korea-pva-air-defense org（关联役炮人更新）。检查：字面无?/乱、0断链。
- 人物甄别：本役另现连长李金贵/董兆华（14团2/3连）、政委梁一民/副团长吴则忠等为叙事/领导
  角色，未单开人物页（抑who's-who），保留在事件/org内；韩景山因具代表性（典型烈士英雄叙事）
  已建页。
- 断点：下一批自 ch6（防空哨兵逞英豪）读起。SCHEMA 未改。

### 2026-09-05（防空批5 · ch6：防空哨／大榆洞／毛岸英）
- 续读 ch6（防空哨兵逞英豪；raw≈3107-3690）：战初低空无防空火力（6军仅18挺高机）→
  运输对空预警危机；第一届后勤会议（1951-01-22~30 沈阳）建 32 条 2500km 公路约1308
  对空监视哨（防空哨）鸣枪报警防B-26低空/夜袭，诱敌假车队等战法；开篇记大榆洞志司
  遇空袭（毛岸英/高瑞欣牺牲，洪学智劝彭入防空洞）。
- 新建 3：
  - concepts/fang-kong-shao-sentry-earlywarning（防空哨/对空监视哨概念页：运输防空预警
    制度+战法+跨期链接）。
  - events/dayudong-hq-airstrike-1950-11（大榆洞志司遇空袭：毛岸英/高瑞欣殉难、彭德怀
    幸免于防空洞；日期按本书11-24，注明与通行11-25日分歧）。
  - entities/people/mao-an-ying（毛岸英：防空源为防空议题引述其牺牲，非全传，生平以他源
    为准）。
- 更新：timeline（〔防〕1950-11 大榆洞、1951-01 防空哨两目）、wars/korean-war/index（防空
  栏目加防空哨概念与大榆洞役、人物加毛岸英）、org korea-pva-air-defense（关联加防空哨/毛岸英）。
- 甄别：防空哨兵马德融（步枪击落+俘获飞行员）与一等功臣吕俊生（一挺高机击落9架）等为ch6
  战例人物，本批未单开（无后续反复依据），保留在概念/战例描述内；防空哨为本制度载体故建
  概念页。
- 断点：下一批自 ch7（大同江上四战四捷）读起。SCHEMA 未改。字面无?/乱、0断链。

### 2026-09-05（防空批6 · ch7：顺川大同江四战四捷／李金贵）
- 续读 ch7（大同江上四战四捷；raw≈3690-4178）：高炮第14团 1951-01-06 二次入朝（铁路行军、
  途历险/捞炮），1951-01-21 中央军委新番号改**高炮524团**并归野战高炮64师（吴昌炽），布两
  火力群卫顺川大同江桥与成川沸流江桥；约 1951-02~03 对桥来袭美军 F-51/F-80 **四战四捷、
  不足20天击落4架**，先后在 2-19（F-51 坠新仓）、后续（8架F-80双梯队，坠松得洞）等；保
  “运动防御/横城反击”物资过江。
- 新建 2：
  - events/shuncheon-taedong-bridge-airdef-1951（顺川大同江/成川沸流江桥防空战 1951-02~03：
    524团四战四捷4架、部署行军、战果与保障对象）。
  - entities/people/li-jingui（524/14团2连连长李金贵：新四军出身、辑安首落B-29役主导2连、
    大同江四战打高空F-80梯队——跨两章反复的中层指挥代表）。
- 更新：korean-war index（防空役目+人物李金贵）、timeline（〔防〕1951-02~03顺川役）、org
  korea-pva-air-defense（番号编成 14→524 归野战高炮64师 + 关联役/人物）。
- 甄别：代理连长衡志强、舒永林、王世堂（捞炮/行军）等为途历人物，未单开；李金贵因跨章反复
  +作战代表性开专页。
- 断点：下一批自 ch8（沸流江上捉到了飞行员奥勃莱）读起。SCHEMA 未改。无?/乱字、0断链。

### 2026-09-05（防空批7 · ch8：沸流江桥防空战／李宏华）
- 续读 ch8（沸流江上捉到了飞行员奥勃莱；raw≈4178-4617）：高炮（524团）成川沸流江桥火力
  群初战不利（山头遮蔽漏机/江桥被炸受批）→把高炮人力拉上山头设阵地+专打敌机投弹瞄准
  段→反轰炸作战击落 F-51（6连李宏华指挥、4炮张菊明点射等）并生俘美空军第35联队少校
  飞行员卡尔·奥勃莱（书中译名/联队待他源核）；并记临时翻译（日裔司机）陈家礼暗杀叛逃
  未遂之插曲。
- 新建 2：
  - events/feiliujiang-bridge-airdef-1951（沸流江桥防空战 1951-02：拉炮上山战法、击落F-51
    俘飞行员，跨顺川成川防线战役的沸流侧专页）。
  - entities/people/li-honghua（高炮524/14团6连连长：ch3入朝行军兼ch8沸流指挥，随6连跨
    章反复，本役指挥代表，指导员刘明厚并记）。
- 更新：korean-war index（防空役目+人物李宏华）、timeline（〔防〕1951-02沸流目）、org防空兵
  关联役/人物。甄别：通信员黄满堂、文书小陈、2排长张法生、副营长王继臣等为战例/破案人物，
  未单开；张法生打法贡献保留于事件/注记，若后续反复再现再议。
- 断点：下一批自 ch9（周恩来致电斯大林催苏联政府快给高射炮）读起。SCHEMA 未改。无?/乱、0断链。

### 2026-09-05（防空批8 · ch9：高炮64师／76.2抵数／周士第）
- 续读 ch9（周恩来致电斯大林催苏联政府快给高射炮；raw≈4617-5016）：野战高炮64师（611/612
  团）入安州—清川江/大宁江护桥（师先派员向曾以日制老炮打完喷气机、后扩为604团的原高炮1团
  3营取经）；战场高炮短缺、解方/聂荣臻推动周恩来1951-03-15致斯大林购炮（苏3-17布尔加宁
  回电改80门85为76.2抵数，周士第异议）；4月底到货并续建534/542/509等多团以老带新赴朝。
  611清川初战击落3/击伤1，月内据书击落10击伤13。
- 新建 3：
  - entities/organizations/field-aa-64th-div-korea（野战高炮第64师（吴昌炽）：师辖611/612及
    指挥524（原14团）；安州清川/大宁江护桥及顺川沸流指挥关系；师属团小团编制含高机连）。
  - entities/equipment/sov-76-2mm-aa-gun（苏式76.2mm高炮：二战淘汰抵85门数，射高7000-7500
    够不到8000m B-29，周士第异议）。
  - entities/people/zhou-shidi（防空司令周士第：军委防空领导主官，华东起任/编机构/赴朝调查/
    推动军购催炮，防空源组织视角中央主官）。
- 更新：korean index（人物+周士第）、timeline〔防〕1951-03 军购+64师安州清川大宁、org防空兵
  关联（64师单位/76.2炮/周士第人）。
- 甄别：解方、聂荣臻、焦骥/赵文彬等为指挥/动员人物（官方主干另载），未单开；611团作战细节
  将在其专属或事件续中（ch反绞杀等）合入。
- 断点：下一批自 ch10（痛击空中幽灵B-26）读起。SCHEMA 未改。无?/乱字、0断链。

### 2026-09-05（防空批9 · ch10：阳德夜战B-26／陈文义／37mm）
- 续读 ch10（痛击空中幽灵B-26；raw≈5016-5285）：夜间B-26封锁交通威胁、各高炮部探索打其法
  （彩灯诱+灯前打等）；重点志愿军独立高炮营（营长陈文义，37mm）守阳德后勤3分部仓库：白昼
  击落F-84后敌转夜袭；营研"盲人夜战"——凭耳听+手感装定诸元，1951-07-02一夜连落2架B-26，
  07-03~11九天再落7架并生俘机组，军以上通令嘉奖、敌标"阳德禁区"、苏军顾问誉"世界战史奇迹"；
  美第8集团军司令范佛里特之子（美军3联 B-26 于物开里被击落）之下落成谜（未下断言）。
- 新建 3：
  - events/yongdok-warehouse-night-airdef-1951（阳德仓库夜间防空战：37mm独立营夜战B-26；
    07-02夜间2架、9天7架战果，夜战"手感/耳功"战法）。
  - entities/people/chen-wenyi（阳德独立高炮营营长：提"学盲人"夜训、指挥夜战成案）。
  - entities/equipment/sov-37mm-aa-gun（苏式37mm高炮：小口径主力、低空/夜战、37营战例）。
- 更新：korean-war index（防空役目+人物陈文义+主力炮行扩37/76）、timeline（〔防〕1951-07阳德）、
  org防空兵关联（阳德役+陈文义+37炮入行）。
- 甄别：团参谋长审讯B-26被俘飞行员（彩灯诱饵）只作背景；小范佛里特下落之追查不属防空战果定
  论，不予断言。陈文义师属番号本书前后略异，以原文为准。
- 断点：下一批自 ch11（冰雪消融，鸭绿江上重开战）读起。SCHEMA 未改。无?/乱字、0断链。

### 2026-09-05（防空批10 · ch11：春季鸭绿江三桥攻防／张培光）
- 续读 ch11（冰雪消融，鸭绿江上重开战；raw≈5285-5758）：冰后美 B-29（含两千磅塔松式制导
  炸弹）与护航歼击对安东/辑安/长甸三桥大轰炸；安东503团（易戈）断其一指击落B-29坠定州、
  长甸505团（刘永松）击伤一架＋沿江改番换装（原4→501等装苏式炮）；辑安501团仓促应战江桥
  炸4孔；战后东北防司自评兼战果与警戒/指挥失利教训（均抢修复通）。
- 新建2：
  - events/yalu-spring-1951-triple-bridge-airdef（春季鸭绿江三江桥对空大轰炸攻防 1951-03：
    多桥混战、503击落/505击伤B-29、501受损，两源口径注记）。
  - entities/people/zhang-peiguang（高炮505团电话员：3-30断桥悬空铁轨接线保团长指挥而
    立功者——防空通信保障代表性人物）。
- 更新：korean index（防空役目+人物张培光）、timeline（〔防〕1951-03-30三桥目）、防空兵org
  （春季沿江换防整理段：原4→501/17升编+新503易戈/18→504/13→505刘永松/新506等）。
- 甄别：通信/指挥类同型（韩景山牺牲 vs 张培光生还立功）并列记，不混淆；501/503/505团长为
  指挥层保留于事件/org。
- 断点：下一批自 ch12（牺牲与慰问）读起。SCHEMA 未改。无?/乱字、0断链。

### 2026-09-05（防空批11 · ch12：安东4月两战／王秉珩殉国）
- 续读 ch12（牺牲与慰问；raw≈5758-6134）：4-07 敌27联队F-84护航B-29顺光大轰炸安东桥，503
  团4连（王秉珩）硬扛三批攻击，指挥掩体被毁、连长王秉珩/高平/杨大绪（高、杨殉/王重伤续指
  挥后壮烈牺牲，连伤亡18）战后团报请抚恤；4-12 赴朝慰问团到团当日迎击40架B-29（80架F-84
  护航）击落三架击伤五架活捉10机组（多属307轰炸大队）"了不起的胜利"并向祖国献战利品；前
  后安东雷达站预警著录。
- 新建 1（复用兼更新王秉珩人物页）：
  - events/andong-airdef-1951-04（安东鸭绿江桥4月作战：4-07王秉珩殉、4-12慰问团前3落B-29，
    伤亡/战果/口径分注）。
  - 更新 entities/people/wang-bingheng（补1951春守桥与1951-04-07殉国；下接503团沿革说明）。
- 更新：korean index（防空役目+4月、人物王秉珩标殉）、timeline（〔防〕1951-04安东役）、org防空
  关联役目。
- 甄别：506/505团长等与慰问团当事人不单开；殉难高平/杨大绪亦随王秉珩页并记,不各建浅页。
- 断点：下一批自 ch13（掩护机场修建）读起。SCHEMA 未改。无?/乱字、0断链。

### 2026-09-05（防空批12 · ch13：掩护机场修建／董兆华）
- 续读 ch13（掩护机场修建；raw≈6134-6478）：1951 春抢建前推机场，野战高炮分头掩护——
  64 师（610/611/612，师长吴昌炽）护顺安机场（611 赵文斌以白布香火假火光破 B-26 夜封按时
  入场；首战 4 架 F-80 中落 2 伤 1、约 10 日敌停轰）；63 师（师长吴忠泰，607〔85mm〕/608、
  609〔37mm〕）护永柔机场（4-03 入场、4-07 近战落 B-26、一场大空袭 06–16 时击落 5 击伤 8）；
  高炮 524 团（彭宗义）护顺川机场（遭潜伏敌特打信号弹导炸机场，被团防控制止/破获；4 月中旬
  3 连董兆华低空近击落 F-51 并生俘中尉丁沙克；后十余日另落 F-51/F-80 多架，获志司/64 师表扬与廖承志
  慰问团"高射炮手"锦旗）。
- 新建 2：
  - events/airfield-construction-protection-1951-spring（顺安/永柔/顺川三机场掩护修建防空战
    1951 春，含各师团战果与敌特威胁）。
  - entities/people/dong-zhaohua（高炮 524/14 团 3 连连长：辑安 B-29 役、沸流捕俘、顺川低空落
    F-51 捕丁沙克——跨多章反复的高炮连长代表）。
- 更新：korean index（防空役目+人物董兆华）、timeline（〔防〕1951 春机场掩护目）、防空兵 org
  （关联役/人物；编成注补 63 师及 64 师顺安机场）；field-aa-64th org（补 610 团与顺安任务）。
- 甄别：吴忠泰/焦骥/赵文斌等为师团指挥层不单开；廖承志慰问为锦旗/旗背景；丁沙克系敌俘不建
  我方人物页（名留事件/战报）。
- 断点：下一批自 ch14（抗击"地毯式轰炸"）读起。SCHEMA 未改。无?/乱字、0断链。
### 2026-09-05（防空批13 · ch14：顺川机场·遏制"地毯式轰炸"／张安桐）
- 续读 ch14（抗击"地毯式轰炸"；raw≈6479-6789）：美对顺川机场由逐日战轰改（先转夜间水平投弹
  →受罗盘拦阻射表挫）继而面状"地毯式轰炸"（B-29 高空面积投弹）并战轰/B-29 交替。高炮524团
  （彭宗义）以罗盘基点拦阻射表破夜袭、按45°攻航路调阵地（3营慈山新丰里）等应对；5-13 首遇
  面状（13 架 B-29，7 连及时撤出定时弹区）、6-13 战轰＋地毯交替时集火击落（为首 B-29 返航时
  坠、另一架 8 发弹幕迫弃弹）挫该次面轰，拆缴敌机机枪改装高机；85mm 旧弹引信/卡销问题下，
  2 连炮长张安桐冒巨险自制金刚钻给旧弹弹头加装"卡销"使其可经测合机快速装定，随即以改造弹击
  落一架 B-29（其工作模范/战斗英雄、据书多次受奖5次立功）。
- 新建 2：
  - events/shunchon-airfield-carpetbombing-counter-1951（524 团顺川机场 1951-05~07 遏制"地毯
    式轰炸"：夜拦阻射表、5-13 首面状（7连续时撤离定时弹区）、6-13 集火击落挫地毯、张安桐改弹
    案与 85/37mm 分工等）。
  - entities/people/zhang-antong（524/14团2连炮长：危工手工给旧 85 弹加卡销改型、以之助击落
    B-29；屡立战功代表）。
- 更新：korean index（防空役目＋人物张安桐）、timeline〔防〕1951-05~07 遏制地毯目（插入时曾
  误删"第四次战役"标题，本次已恢复）、防空兵 org 关联役/人物。
- 甄别：7 连连长（书载名"衡志祥"，与他处"衡志强"近名字段 OCR 存疑）未就此单开人物页；带伤
  鼓舞的炮排长张良志等保留于事件内不个别开页。张安桐因战果具代表性开专页。
- 断点：下一批自 ch15（丢掉幻想，准备斗争）读起。SCHEMA 未改。无?/乱字、0断链。

### 2026-09-05（防空批14 · ch15：停战谈判期 513团/独立营 护交·安州双桥首胜）
- 续读 ch15（丢掉幻想，准备斗争；raw≈6789-7315）：主力野战师转机场后，志司以独立高炮营
  （39/40/41 守大宁-清川江、42/43/44 守大同江-成川沸流江）＋步兵改编新高炮 513 团（江萍，
  冀中7纵20旅58团，边打边练/误射友军事故后整训）及 505 团等重建江桥护交；停战谈判（7-10
  板门店）背景下"以炸促谈"预判与教育；7-11 威兰奉李奇微令首炸安州，独立39/40营＋513团4连
  （马良善）5连（田玉柱）迎击 8 架战轰，一毁四伤、双桥无恙——护交"谈判日"首胜。
- 新建 1：events/anju-jiang-ji-bridge-1951-07（安州·大宁-清川江桥护交战 1951-07-11，
  谈判期以炸促谈/39-44营结构/一毁四伤双桥无恙战果）。
- 更新：防空兵 org（中段护交再编整段：独立39-44营＋513/505团结构与链接该役）、korean index
  （防空役目加该役）、timeline〔防〕1951-07-11 安州双桥。
- 甄别：江萍/陈袭/马良善/田玉柱/袁九顺/高于林等多为师团营连指挥层（新成军过程中），本批未
  开人物页；后续若其续反复出现具代表性则再建。麦克阿瑟免职与谈判史料属官方主干，不重复建页。
- 断点：下一批自 ch16（保江桥战洪水）读起。SCHEMA 未改。无?/乱字、0断链。
### 2026-09-05（防空批15 · ch16：505团/独立营顺川成川双桥护交＋1951夏特大洪灾保安）
- 续读 ch16（保江桥战洪水；raw≈7315-7649）两话题：
  (1) 对空护交：第五次战役后敌以B-29中高空炸顺川大同江桥/成川沸流江桥；军委防司4月下旬调
     高炮505团（刘永松，长甸河口13团改番）率全团统一指挥独立42/43/44营护两桥。连战约50天，
     5月作战15次落2伤4、6月作战32次落8伤10，获志司通报；取524团沸流战斗经验。
  (2) 1951年7月中下旬-9月朝鲜四十年一遇特大洪灾（山洪/泥石流/江河泛滥）：冲毁铁桥94座、
     铁路路基116处次、约50%公路桥，河流便桥被吞没（运输中断最长45/最短13天、三登被淹）；
     在朝高炮部队日夜筑堤泄洪保兵器（顺川机场524团8连守岛垒堰、3连当危急、营参谋长何竞提
     挖开南高土梁泄洪救兵器）。
- 新建 2：
  events/shunchon-chengchon-double-bridge-505-flood-1951（双主题战役/环境事件：505团双桥50天
    护交＋夏洪保安；修多处草稿错字）
  entities/people/liu-yongsong（505团长：河口→顺川成川统筹护交与洪期检查分工）
- 更新：防空兵 op体"汛期护桥保安段"（505团/独立42-44营/524保兵器例）、org人物加刘永松、
  korean index防空役加该役、timeline〔防〕加 1951-04下旬~07 505团护交 与 1951-07洪灾两目。
- 甄别：何竞/8连/3连营长等连营指挥层与单事例子未开人物页；"50天/月别战果/灾损"等均为本书
  口径单源；洪灾为后勤抗灾非空战，按防空侧"护兵器保战备"收载。
- 断点：下一批自 ch17（反绞杀战）读起。（ch17 涉及反绞杀，相关大片主源既有
  strangulation-war-counter-1951-1952〔CAMS〕页——判断新增防空侧增量，防止叠建。）
- SCHEMA未改；无?/乱字/FFFD；0断链；全库内容页随QC计数变化（此前177→本批+2，QA下为准）。
### 2026-09-05（防空批16 · ch17：安州枢纽反绞杀防空战＋"打不垮的 4 连"）
- 续读 ch17（反绞杀战；raw=7648-8152），先比对既有 CAMS 反绞杀总页
  events/strangulation-war-counter-1951-1952（不叠建总框架，本书防空侧以逐役增量补位）。
  内容为安州交通枢纽（大宁江桥/清川江桥/车站）1951-07~08 反"绞杀"防空：
  - 布防：513团（江萍）以唯一76.2营警戒西海湾口，独立39营大宁江桥南北/40营孟中洞站/41营清川
    江桥南/3营老安州东北；505团（刘永松）+42/43/44营守顺川成川。敌以舰载F-4U/F-84云下低空偷袭
    及B-29高空集炸交替。
  - 战例：505团云下近战10余分钟顺川落3伤7（获军委防司通令嘉奖）；513 3营9连距2000m首发落
    带队机又集火落一架；约某日17:20敌48架F-84/F-51围攻大宁江桥南40营阵地（高玉林）落2伤4；
    且守清川江桥"打不垮的4连"（马良善）遭冲绳B-29+70°俯冲子母弹集炸，全连同仇（4炮孙绍武、
    1测手孙耀庭让位殉、电话兵宋守森跳江咬线、1炮手潘福信殉炮位、2炮手孙有志死战）仍不撤并击
    落敌机；8-31敌12架再袭安州又落一伤一并俘韩德森。
  - 结论与并轨：8月敌约一月绞杀未捷（8月过境1134车皮、10月一役7天1499车皮），敌另寻目标——
    边轨CAMS反绞杀页；防司/威兰等要因见单source。
- 新建 2：
  events/anzhou-hub-antistrangulation-airdef-1951-0708（安州枢纽反绞杀·夏洪暴雨防空战）
  entities/people/ma-liangshan（513团2营4连连长：谈判日7-11与8月"打不垮的4连"连续主人公渠）
- 更新：防空兵 org（役列表安州双役＋for反绞杀并轨、人物添马良善）、korean index（防空役目，
  org正文）、timeline〔防〕安州枢纽反绞杀目、既有strangulation(CAMS)关联线补本书防空侧链接
  （防叠并轨）。
- 甄别：4连连内众多英烈（闰喜明/孙绍武×班/孙耀庭/宋守森/潘福信/孙有志等）系单章连内heros未开
  页(记于专役页正文)；团长江萍、营长高玉林指挥层不另页。F4U型号陆战队战法、阴雨雷达不可目视等
  场景按书。战果/车皮自本书与《当代·抗美援朝战争》卷交接口径，同页标明。
- 断点：下一批自 ch18（打光了的半个连和一个美国飞行员）读起。QA：无?/FFFD/乱字，0断链。
- SCHEMA sha 未变（191cd2…）。内容页随QC（此前179→本批+2 计 181，以QA告为准）。
### 2026-09-05（防空批17 · ch18：顺川机场 8-24 鏖战 + 3连"半个连打光" + B-29 空勤吉本斯投降）
- 续读 ch18（打光了的半个连和一个美国飞行员；raw=8153-8644），一日（**1951-08-24**）两大叙事：
  (1) 敌"先毁高炮"战术（战轰压制守场中高炮+俯冲子母杀伤弹）；顺川机场 524 团（彭宗义）中小
     高炮混配：先破 F-80/F-84 "声东击西" 伴攻（将计就计数连齐放），继而敌 B-29×11（2 批 6000米）
     伴战轰合攻，主攻守清空域之 3 连（原董兆华）——指挥仪班（赵云汉、奚品衡、梅文斗、周纪生、
     周愈、黄俊）与电工蒋文、白曙等殉炮位，炮排长冯代培负肠坚持、电话兵宋守森跳江咬线保通；
     连长[[dong-zhaohua|董兆华]]重伤，抢救手术中牺牲；通信员黄满堂扑护殉。此役 3 连 15 名干部
     战士牺牲、22 人负伤，即卷中"打光半个连"（负伤者无一离位、连不撤），团长调全团/高机排驰援
     终打退。
  (2) 伤的一架参战 B-29（307 轰炸联队372中队）坠顺川西——空勤 9 人被军民活捉，漏失轰炸员
     爱德华·吉本斯在树山林过夜，想起陆战斗士赠的"安全通行证"（中朝英四优待条款）后，次日清晨
     持白手帕主动到 3 连投降；连队以张金凯坚持优俘政策让饭给足，吉本斯感服"把条款做得比写的好"
     请求将通行证留作纪念（志愿军战俘政策执行实例）。
- 新建 events/shunchon-aug24-524reg-3co-b29-1951（顺川机场8-24鏖战与空勤战）；同步补董兆华
  人物页 ch18 归宿（1951-08-24 牺牲）+ org 人物注 + index 防空役/Timeline〔防〕8-24 目。
- 甄别：指挥仪班赵云汉等 6 人、电工蒋文/文化教员白曙/炮排长冯代培、通信员黄满堂等单个英烈均
  系单章连内人物，未逐个开首（名记专役页）；吉本斯(美俘)、瓦纳尔非我方人物页；D1 双 11"先毁
  高炮"战术与 D-杀伤弹细节按本书。瓦纳尔等处不经跨源校。
- 断点：自 ch19（三角地区的反"窒息战"）以降续读。QA：无断链/乱字/?/FFFD；frontmatter 全。
- SCHEMA sha 191cd2 未变（前批 181→本批+1 事件页 =182；董兆华页属更新非新增，实增1）。git
  提交信息"防空批17…"。
### 2026-09-05（防空批18 · ch19：三角地区反"窒息战"——铁道高炮指挥所成立/63师阁岩12-16）
- 续读 ch19（三角地区的反"窒息战"；raw≈8645-9411）。反绞杀护交进入"三角地区"（新成川—价川—
  安州等枢纽）＋京义线肃川—万城及中坪—价川、殷山—阳德等段的夺气封锁与反夺气：
  · 中央军委 1951-09-15 加强铁桥江桥防空决定；9 月下旬抽出 1 高炮团+11 独立营+6 高机连掩护三
    角地区（敌昼间战斗轰炸机定时定点"窒息"轨站、夜 B-29/B-26 等以单架跟进打桥），因高炮不足
    （在朝约七成用于护路仍紧张）志愿军向苏联恳请再派一个三团制高炮师赴安州护交。
  · 10 月起在安州成立**铁道高炮指挥所**〔铁道高指〕，命高炮 64 师师长[[wu-changchi|吴昌炽]]兼司
    令员统一在朝护交高炮（后各师/505"一兵两用"日夜机动），以集中兵力重点保卫+高度机动、打临
    近不打临远等的运用；12 月成部布防调 62 师（王星）万城—肃川、63 师中坪—价川、64 师各团
    殷山—阳德/顺川等。
  · 冬 1951-12-16 63 师（607/608 团+配属独立营）守阁岩车站一日：击落 5/击伤 8，敌投弹命中率
    约 60%→3%，顺川—价川间恢复通车。
  · （书内并载反窒息期间的〔空〕4 师/3 师米格机群掩护等空军线战例，系空军叙事、本防侧不作重复
    展开——归 yingjichangkong 线。）
- 新建 2：events/geyan-station-airdef-63div-1951-12（阁岩车站保卫战 1951-12-16）；
  entities/people/wu-changchi（吴昌炽：64 师长→铁道高指司令员，防空护交统筹）。
- 更新：防空兵 org（编成补"铁道高炮指挥所/铁道高指"整段 + 人物列增吴昌炽）、korean
  index（防空役列增阁岩役）、timeline〔防〕1951-10~12 铁道高指护交统编 + 12-16 阁岩二目。
- 甄别：62 师（王星）、63/64 师团/营连级指挥与"一兵两用"等例并入 org 注；〔空〕4/3 师、李永
  泰/王海/刘涌新等空军英雄不建本线人物页（归属空军线源页）；阁岩页内连排名（炮长/测手等）未
  开人页。均按本书单源、不跨 CAMS 并吞。
- 断点：下一批自 ch20（血战丁山里）读起。QC：无断链/乱字/?/FFFD；frontmatter 完整。
- SCHEMA 191cd2 未变；内容页 182→+2=184（QA 以实际为准）。git 提交"防空批18…"。
### 2026-09-05（防空批19 · ch20：血战丁山里——524团机动防空／6连归队行军防空）
- 续读 ch20（血战丁山里；raw≈9412-9851）。绞杀战"第三阶段"敌专攻无防空重点段后：
  · 敌先转慈山一带（顺川方向数日不通）；铁道高指令保卫顺川机场的 524 团抽 3 营（王金声）赴慈
    山机动游击（首战因拂晓未全备、营参犹豫只末机集火落一架；团长彭宗义纠正"切忌犹豫"），其
    "神出鬼没"使敌不敢久呆、转殷山—新成川（三德里）。团再以两个中连＋两个小连守新成川站、两
    个小连＋高机连在长阳/新仓/殷山机动；2 营仅 4 连、6 连原配 601 团在阳德同需归队。
  · 6 连由阳德归队"行军防空"（ch20）：连长[[li-honghua|李宏华]]/指导员刘明厚，拟"行军随时备
    战"案（干部坐车顶监视、炮手坐炮位、车间距 50~100 米、每炮携应急 30~40 发）；温井里突遇
    F-84×6，过桥占阵以 4 炮张菊明近距长点射接落 1 架（约 10 分钟 167 发）。
  · 丁山里·长鲜江桥血战（ch20）：敌锁定长鲜江支流丁山里水网铁公路（"一石二鸟"地）；524 团
    1 营设伏新成川、2/3 营机动布丁山里（4/6 连布长鲜江桥两侧、3 营守 望日黑）。晨战敌 42 机
    混合被 3 营集团击落 F-84（香枫洞）、4 连自衛；当日下午 16:30 敌二十余机专攻 6 连（连长在营
    开会，指导员就地指挥各炮自卫）——"血战"中 1 炮王福田/巩保义、副班长兼 4 炮手、3 炮长薛景
    财、副指导员田乐迎等先后壮烈，4 炮张菊明近距击落来机后负伤仍指挥。全役 6 连 8 死 5 重 4
    轻；善后多方寻找烈士遗骸。
- 新建 1：events/dingshanli-longxian-bridge-524-1951（丁山里·长鲜江桥血战）——时间段按本书冬
  段，页内已注明书文日（"3 月 8 日"）疑 OCR/字体而不锁死日期。
- 更新：entities/people/li-honghua（6连连长）补温井里行军防空＋丁山里血战两节；korean index 防
  空役加丁山里役；timeline〔防〕加"1951 冬以降 524 团机动反绞"（顺带修复上一批 timeline 误删
  "价川间长期不通局面"字样）。
- 甄别：张菊明/薛景财/张树法/田乐迎/冯绍安等炮排连英烈记专役/其连长人物正文，未逐人另开；
  敌机型号（F-9F 系 OCR 之"F-9F/F-84/F-80"）、战果与伤亡按本书（我方口径）；日期 OCR 存疑不
  断言。
- 断点：自 ch21（雪地激战/雷地激战）续读。QA：0 断链/乱字/?/FFFD；frontmatter 全。
- SCHEMA 191cd2 未变；内容页 184→+1=185（QA 为准）。git 提交"防空批19…"。
### 2026-09-05（防空批20 · ch21：雪地/雷地激战——513团冬季机动与云田"隐真示假"）
- 续读 ch21（OCR 题互作"雪地激战/雷地激战"；raw≈9852-10362），绞杀近半年敌赴宣川—云田（京义
  线）段短程战术狂炸，调 513 团（江萍）携 3 营＋独立 39/40/41 营机动护段：
  · 机动要诀 点线兼顾、分散集中、运动与伏击结合、放近打、首架放过打第二架、隔一架打一架；
    前战取战时郭山（3营石信钟）、樟岛川/定州（40营高玉林）皆赢得铁道兵"高炮万岁"。
  · 严寒条件下（零下二三十度、鞋底冻贴炮盘、假伪装机动耗力）仍坚持。
  · 云田役主力：3-2 普雪后江萍料敌封南下军列，令军务股长张文盛组织朝鲜群众在真阵旁连夜设
    假阵地（松枝炮身/破瓦轮/稻草人执红旗），雪掩车迹；次日（3-3 及后）敌逐批中计俯冲假阵被
    伏集火——首 F-84×12 攻 39 营假阵（袁九顺 2000m 敲1）；敌改顺光纵队攻云田站，3营仍放首架
    打第二至 1000m 齐射，其并隔一架打法获更多战果；12:30/14:42 更大批（52/50+）扑石营撤空/
    假位反遭新位 7、8 连（崔、张）与近新连击——全役**击落 9、伤 21**（伤者多坠黄海），获铁道
    高指通令嘉奖二度；满载坦克列车安全经云田；美军广播"摧毁高炮阵十余处无损"被录以揭示其夸
    大宣传（513 政治教育材料）。江萍后返京向首都防司讲"小口径高炮机动作战、集火、近战、伏击"。
- 新建 2：
  events/yuntian-deception-fake-gun-513-1952（云田"隐真示假"伏击战 1952 初）
  entities/people/jiang-ping（513 团长：机动作战/隐真示假；辨 OCR 异写）
- 更新：防空兵 org（人物列添江萍；铁道高指/独立营段含此章机动续）; index 防空役加云田役；
  timeline〔防〕1952-01~03 513 团机动与 3-3 云田大捷目（置于 1952 张积慧目后）。
- 甄别：39/40营营长袁九顺/高玉林、3营石信钟篇营级指挥与张文盛等人记 org/event 文不逐开；战果
  与战数按本书（我方口径）；章目不锁死某单日（书题 OCR 歧，命页以"云田伏击·隐真示假"）。
- 断点：自 ch22（抗击"饱和轰炸"）续读。QA：0 断链/乱字/?/FFFD；frontmatter 全。
- SCHEMA 191cd2 未变；内容页 185→+2=187（QA 为准）。git 提交"防空批20…"。
### 2026-09-05（防空批21 · ch23 提速版：探照灯兵入朝；ch22/24 暂存目）
- 用户要求试提速（连续多章精简建页）。本次只落 ch23 高价值主题 1 页，不强冲：
  · 探照灯101团2营+1营2连 1951-12-25 首入朝（吴永安/汤宜敬/张鹏等），安州铁道高指统筹，首次灯炮
    夜战配合（初约20天照不中→2-3夜首次照中B-26遗失→2-18夜配合513/610团击落首架 B-29）；后续
    探照灯10连 1952-05~1953-07 照中105架、配合击落B-29×5。
  · 新建 entities/organizations/korea-pva-searchlight-101force（探照灯部队org页）。
  · 防空 org 补探照灯条目链接；ch22(抗击饱和轰炸)、ch24(楠亭里仓库保卫)暂在 org 存目，逐批次续。
- 修正/自纠痕：本轮写页多处以"提速"起笔但数次带入杂字/占位符并反复清理修复 —— 提示后续提速须
  先一次扫描+小步提交，勿在受长文损耗后整页大改；质量门禁 (0断链/?/FFFD/杂字) 均最终通过。
- QA: 快速 resolver+glitch 过；SCHEMA 191cd2 未变；全库内容页 187→188（QA为准，新增org页1）。
### 2026-09-05（防空批22 · ch22：院里—兰田里抗击"饱和轰炸"，524团机动反绞收官）
- 用户选回到选项1（每次"继续摄入"精读一整章、复检、建页、提交）。断点校正：前批曾跳过 ch22 建
  ch23 探照灯页并留下 org 存目；本批把 ch22 补建，断点至 ch24 前的顺序为 ch23（已建）→ch22
  （本次）→ 续 ch24（楠亭里）。
- 续读 ch22（raw≈10363-10832）：1952 春美第5航队情报处长道厄迪提议"饱和轰炸"(咽喉隘口集中
  机群昼夜炸)；先在瓦洞试样（使 B-29/B-26 投5百~2千磅 3928 枚、断铁路18公路15处，仅使运中断
  7/4天），第5航空队司令埃佛勒斯特坚持只是选点不当→改选院里/兰田里段（桥高、易炸难修）。其段
  3 月底二次"饱和"开始（日出百余架），铁道高指下令 524 团（彭宗义）赴该段机动（严有德先遣、
  牛书齐/王金声各营）；4-4 到位、4-6~8 敌多侦而团伪装按兵；4-10 敌空海军 130+152 等 280 余架
  攻→"保卫目标为主"拦阻火网击落 3 架、铁路仅旁弹，王永祥（测手，1949-07 入伍 24 岁）殉、3 连
  副连长马健正（继牺牲连长董）代连指挥；后 1 营守新兴洞—百岭川、2/3 营昼夜真假机动→粉碎其计
  划。至 5-29 524 团交装 522 团回国（1 年 8 月共 1480 战/落53伤214/俘15/牺牲76伤162），至
  1952-6 美弃"绞杀"转仓库城水电（并轨 CAMS 页）。
- 新建 1：events/yuanli-saturation-bombing-524-1952（院里—兰田里"饱和轰炸"抗击战 1952-04）
- 更新：防空 org（ch22句含其收官; ch23探照灯链接; ch24留续建标的）、korean index 防空役加该役、
  timeline〔防〕1952-04 院里—兰田里目（+反绞收尾数据）。
- 甄别：彭宗义（524团长）等团/严有德/牛书齐/王金声/马健正指挥层记 org/正文不单页（同前例）；
  王永祥单役烈士故未另开人物页、名留专役/即此页；战果/历次累计按本书（我方口径）。
- 断点：下一批自 ch24（楠亭里仓库保卫；raw 11223-11585）读起建页。SCHEMA 191cd2 未变；
  QA resolver+glitch 均过（0 断链/?/FFFD/乱字），frontmatter 全。内容页 188→+1=189（QA 为准）。
### 2026-09-05（防空批23 · ch24：楠亭里仓库保卫战 高炮独立24营 1952-05-08）
- 续读 ch24（raw≈11223-11585）：1952 上最无效后美转炸我防空薄弱后方仓库；炮兵处集训各守库营长
  （两句口号＋五点射击原则、37mm 2000m 内最有效等）。守卫楠亭里的高炮独立24营 5-8 从拂晓战至日落
  一整天：敌 28 批 367 架次（F-94/F-80/F-84/F-51/F-47/F-86/米基阿尔/直升机/不明各若干），营及
  1/2/3 连与高机连用"打一架震慑、转预备阵地、2000m 内近距离截"等法，以 12 门 37mm 高炮及高机打
  出 37 弹 6096/高机弹 11918，**击落7击伤18（合25）**；全营 28 伤皆不撤（含 1 连 1 炮手岳建华震昏
  苏醒续战又落、2 连 3 炮手赵镜臂伤坚持、高机班长张志忠火中先杀机后扑火）。洪学智当日至营慰问，
  新华社 5-27 通讯与《当代·抗美援朝》并载（通讯数字如 292/27 与书 367/25 之出入由书作者注按
  367/25 校正）；该营两年两月累计 448 战/1498 架次落 23 伤 53 集体二等功；另库区武装特务清剿获
  610 余名。
- 新建 events/nantingli-warehouse-airdef-24-1952；防空 org（守仓营链接）、korean index 役列、
  timeline〔防〕1952-05-08 目各更新。
- 甄别：赵镜/岳建华/张志忠等单役功臣记正文不另开人页（who's-who 纪律）；新华社/官方史数字以书
  作者之 367/25 校正为据。
- 断点：下一批自 ch25（高炮追着飞机打，raw≈11587 起）。QA/SCHEMA：191cd2 未变、0断链/杂字/FFFD；
  内容页 189→190（QA 为准）。
### 2026-09-05（防空批24 · 决策记录：ch25 一律留白，位移）
- 用户决策：不确定先留白、跳过后面的章节；有依据再补充书写。
- 据此 ch25"高炮追着飞机打"（511 团轮战/张若水渔波机动及 76.2 演进）暂不给专页：把明确可核的轮战轮
  换框架（防空兵部 1952-02-22 上报总参；502/510/509/511、华东 522-525 团营及 101/121 团探照灯分队
  分批入朝接防 505/508/513 等）记入防空 org（方括号留白注）；人物/事件细目此后如有更稳来源再补。
- 下一步断点从 ch26（空炮灯协同作战共歼 B-29）读起。QA 门禁照常；SCHEMA 全库不变（后续提交按续作）。
### 2026-09-05（防空批25（续）· ch26 亦回退留白）
- ch26"空炮灯协同共歼B-29"（1952-06-10 郭山大桥夜战）草拟 event 页后复查仍有密集细节不能逐条坐实
  （飞机数/分工/引美书局部），按用户 3 号原则"不确定先留白"删除草稿不提交。
- 保留提交：防空 org 的 1952 轮战/接防框架行（可核），及本 log。ch26 留白（雷达网/方格坐标/421团6连
  卢希海及 6-10 夜战均待有据；装备组织先行录于探照灯 org 页等）。
### 2026-09-05（防空批26 · ch26 郭山：空炮灯协同夜战补建事件页）
- 前沿状态：防空批25 ch25/ch26 均按用户“不确定先留白”回退空置；本轮于 fresh 会话重拾 ch26，先通读
  raw ch26 全章（防空txt行 12451-12912）复核，确认语料可达原文可核，遂补建 1 事件页：
  events/guoshan-bridge-night-coord-airdef-1952（郭山大桥 空·炮·灯 协同夜战 1952-06-10；event_type:
  battle）。原低容量上下文会话中“无法逐条坐实”之点，本轮以〔版本分歧〕并列口径解决而非断言单一数字。
- 页含：(1) 铺垫——朝后雷达情报网（1951-09-08 周致金日成、10-05 雷达301营4连/咸兴市；1952-02-03 再
  电、江界/新溪/载宁/元山4站；方格坐标指挥）；(2) 组织/参战——高炮62师(师长王星/华科长)之604团(范
  振声)＋高炮511团1营(常振华)＋探照灯421团2营6连(迟芬亭/卢希海，沿革：入朝不足月、百岭川5-21照中8
  助击伤2、5-26调郭山3雷达灯8跟踪灯、西南横宽10~15km照廊)；(3) 6-10 经过（21:30通报大型机11架、
  21:50 西南进入、24km捕/15km测高6000m/9km开灯、前4架投弹、第五架与六/七机由夜航机击落/伤、末架施
  电子干扰逃脱、师部被弹指挥所震塌；陈辉亭绘方格图与守话传令）。
- 战果——本方/敌方口径并列不并（版本分歧）：本书叙事记高炮伤1、歼击机落/伤多架；吴昌炽《八一》
  1953-09-21 文记“击落三架”；作者注引美《朝鲜战争中的美国空军》第518-519页正文“4架(作者按应为
  11架)/约12机攻击/约24灯”；远东空军轰炸机指挥部事后评估“2落1伤”；〔他源旁证〕官方史 j03_ch10 记
  美“4架”、高炮62师+探照灯协同苏联航空兵落3架、“此后美基本放弃绞杀战”。分歧点明录（机数 11 vs
  4；航空兵归属友军夜航/歼击机 vs 苏联航空兵；总果 3 落 vs 2落1伤）。
- 增补链接：防空 org（批26：雷达情报网+郭山役存目）、探照灯 org（421团2营6连 ch26 补注，明示非101建
  制）、korean index 防空役列、timeline〔防〕1952-06-10。511/604 团之 64/62 师属关系于页/正文留待逐役
  前后核对，凡命名以该役正文为准。师团连指挥与事务人员（王星/范振声/常振华/迟芬亭/卢希海/陈辉亭/华
  科长等）按 who's-who 纪律不单开 canonical。
- QA：newpages-check 5 文件 CLEAN（无问号/替换符/断链/非法yaml/括号失衡）；SCHEMA 191cd2 未变；内容页
  190→+1=191（QA 为准）。
- 断点：防空书已读至 ch27（保卫水丰发电站，raw 12918 起）之前。下批自 ch27 读起。建 62/64 师团级
  canonical 前先核对既有 field-aa-64th-div-korea 与防空 org 的师属表述。
### 2026-09-05（防空批27 · ch27 水丰：保卫水丰发电站战役事件 + 代表牺牲指挥员专页）
- 前沿：防空批26 补建郭山役后，断点自 ch27（保卫水丰发电站，防空txt≈12918-14051 全章）读起。逐节整读后
  建 2 canonical：
  (1) events/supung-hydro-plant-defense-1952-06（保卫水丰·高炮504团大坝保卫战 1952-06-23 起，event_type:
      campaign）——把 6-23 起昼间大空袭保卫、后续防守增强、至 8-24/9-12/10-01 三次夜袭拦截收进一役。
  (2) entities/people/sitaizhi-504-reg-9co（斯太志，504团9连指导员，6-23 腹部中弹肠流仍举旗指挥至牺牲）——
      该书役之代表牺牲指挥员（纪念中心式并有叙事）单开专页。
- 页载核心（据书 ch27）：美 1952“以炸迫谈”首次集中轰炸水丰——背景/决定链（斯马特/仑道夫研究→克拉克八点→
  杜鲁门 6-19 批；佯动欺骗麻痹我防空）＋水丰地理/敌前放行原因；504团防御（王宏/李月坤/刘云/郭清江值班，85mm
  中连3/37mm 7、9连沿大坝西南“三把利剑”）；6-23 白天数批轰炸（14:01 起，第5航队8/18/49/136+陆战12/33+拳师/
  普林斯顿/菲律宾海三航母共约370余架；F-86 88架封机场；94战轰中2批）——**504发弹7000余、落F-84/F-80/F-51
  8架伤10架**；电站中8弹、炸毁2台发电机与5台变压器（月余复电）；我伤66人、损炮1门、测远机2部。役内除斯太志
  另开人页外，王长绪（测远手抱机殉）/李海胜（“英雄炮4班”）/冯德昌（以身导线）等英烈与团营指挥均不逐人单开。
- 后续（据书）：6-25 周士第率苏总顾问拉弗利科/高鹏赴团调查（盛赞+批麻痹无协同）；6-28 增加轮战兵力/探照灯；
  彭德怀 7-10 复朴一禹电列防措；苏军**派一个高炮师**（含火控雷达/目标指示雷达、8门制连）进驻水丰；空军米格-15驻大
  堡；8-24/9-12/10-01 三次 B-29/B-26 夜袭由中苏高炮+探照灯（411团3营拉古哨）挫败（数据书口径）——此后敌暂
  停对水轰。
- 甄别/纪律：王宏/李月坤/刘云/郭清江（团营指挥）与多数英烈（王长绪/李海胜/刘记友/冯德昌等）系单役/连营级，
  不逐他开页、收本页正文；苏“火控雷达/目标指示雷达”为驻水苏高炮伴随装备、细度不足，未另开 kit 单型页，暂留
  org/役页（“无新装备专页”决定显化）。敌美人物（斯马特/仑道夫/威兰/克拉克/杜鲁门）不做我侧专页。斯太志姓名首字
  书有多个 OCR 字型歧异（斯/断/斩/新），正文取“斯太志”并在人页注记。
- 更新：korean index（防空役列+防空人物列）、timeline〔防〕1952-06-23 详情（嵌于既有 6 月“13电厂”宏观下）、
  防空 org（批27：504团水丰段+苏高炮师驻防+探照灯411团拉古哨+205团监视+装备注）。宏观 6-23~27 计数/弃绞杀另见
  strangulation 事件页（并轨不重述）。
- QA：newpages-check 5 文件 CLEAN（无问号/替换符/断链/乱字）；内容页 191→+2=193（QA 为准）。SCHEMA 191cd2 未变。
- 断点：防空书已读至 ch28（保卫平壤，raw 14052 起）之前。下批自 ch28 读起。
### 2026-09-05（防空批28 · ch28 平壤：高炮533团保卫平壤·入朝第一仗事件 + 卢纪泉人物页）
- 前沿：断点自 ch28（保卫平壤，防空txt≈14052-14783 全章）读起。该章防空侧核心为野战高炮 61 师
  高炮 533 团赴朝鲜保卫平壤、在 1952-08-29 入朝第一仗抗击美对平壤“压力泵”二次大空袭。逐节整读后建 2 canonical：
  (1) events/pyongyang-defense-airdef-533-1952-08（保卫平壤·高炮 533 团入朝第一仗 1952-08-29；
      event_type: battle）——事件页载：7-11 首次“压力泵”空袭平壤之背景（人民军 19 团力单不支→金日成请援、
      彭德怀 7-14 报毛、7-18 军委调 533团部率1营+534团3营赴朝）；该团 8-15 广州出发/8-21 安东/8-23 抵平壤布防
      （保西北郊党政机关与调车场，与人民军近卫高炮 19 团〔金上校〕分工、环视雷达共享独立指挥）；8-29 敌自称
      1200 余架参演作 9:30/13:30/17:30 三次轰炸，533 团一日三次抗击约 1700 架次（多波分批口径），击落击伤
      敌 B-29/F-80/F-84/F-9F/F-51/F-4U 等 8 架，代表战例即“敲山震虎/有弹即拼”（1连）及其支援 2、3 连；保持
      弹尽的 9 连撤阵，被迫补充（友军 19 团借弹雪中送炭）；役末小结 + 战后人民军炮兵副司令勉慰。
  (2) entities/people/lujiquan-533（卢纪泉，533团1连连长，“三八式”老炮手）——本役最贯穿且屡有斩获的连
      指挥（其 1 连为 8-29 全团主战/有结果主力），单开专页。
- 甄别/纪律：团指挥尹继先/李仁鑫/陈炳烈/相坤与单役功臣（高机排 刘满堂、女收发员赵润德、牺牲的徐惠霞/吴尽
  忠、李老道/李志贵 等）不逐人单开（who's-who），收役页正文；赵润德女运弹人名可后续按需另补（已注）。无新
  装备专页（85mm/37mm 为主力 kit 已有；敌机型为目标不建）。空情共享（19团环视雷达/青山里我哨）已入防空 org
  雷达情报段。将 7-27 志愿军空 3 师九团镇南浦歼英 FMK5（空军线）排除本役，防空源仅作背景提。533/534 团与
  高炮 61 师师团归口以各章正文为准（〔归口核〕存于 org）。
- 更新：korean index（防空役列+人物列加卢纪泉）、timeline〔防〕1952-08-29、防空 org（野战高炮 61 师/高炮
  533 团保卫平壤段）。架数/战果照本书（我方口径）与美自称并录。
- QA：newpages-check 5 文件 CLEAN（无问号/替换符/断链/乱字）；内容页 193→+2=195（QA 为准）。SCHEMA 191cd2 未变。
- 断点：防空书已读至 ch29（前沿掩护出奇兵，raw 14784 起）之前。下批自 ch29 读起。
### 2026-09-05（防空批29 · ch29 前沿掩护：上甘岭 反“蚊子机/炮兵校正机”掩护炮兵事件 + 彭子新人物页）
- 前沿：断点自 ch29（前沿掩护出奇兵，防空txt≈14784-15422 全章）读起。该章防空主线是**反前沿低空敌指
  挥/炮兵校正机 + 掩护我地面炮兵**；主干为 1952-10-14~11-25 反“金化攻势(摊牌)”·上甘岭的防空掩护。逐节读
  后建 2 canonical：
  (1) events/shangganling-aircover-anti-spotter-1952（上甘岭防空·反蚊子机/炮兵校正机·掩护炮兵 1952-10~
      11；event_type: campaign，start 10-14/end 11-25）——载：敌 6147“蚊子”中队（T-6）与炮兵校正机（OE-1/
      L-5/L-6/L-19 等）对我前沿炮兵之威胁→我高炮/高机以“奇兵”打法反制：a)119师高炮营彭子新**前沿潜伏单炮
      （夜拉至距敌不足1000m伪树＋山顶暗哨报空）**击落 OE-1/AT-6（并因俘解“返航之谜”：首射已毁其转向）；b)某
      37mm 连**高炮进坑道**一门炮连落 3 架；c)志司调 64师 **610团**（张建中，10-27）掩护炮兵，夜伏 B-26 击落
      2/反战轰、压“蚊子/校正”退出 8000m；d)61师 **601团**（袁守范,11-16）反斜面＋假阵地。总括：40 余天上
      甘岭我高炮部队作战 300 余次、击落击伤敌机 270 余架（我方口径）+ 志司通报表扬。
  (2) entities/people/peng-zixin-119-artillery（彭子新，119师高炮营参谋长，“前沿潜伏单炮/伪树”战术代表）
      单开专页。
- 甄别/纪律：张建中/袁守范（团指挥）、37mm“坑道战”连长（连级/不具名）等不逐人开；610/601 团长任职若与原
  书前章旧团长（610 朱建华）出入，取本役上下文为准并〔归口核〕留 org。无新装备专页（37mm/85mm/高机 kit 已
  有；T-6/OE-1/L系/F-84/B-26 为敌方来袭机型、不单开装备页；“前沿雷达”实为隐蔽对空哨，防空情报既有）。
- 交叉口径：上甘岭主线（597.9/537.7、坑道战、摊牌失败）并入既有 [[shangganling-campaign-1952]]，本役为其
  防空侧增补（防空书 ch29 口径之 300余次/270 架战果与主线别录）。
- 另役待补（记录于 org 章尾注）：防空书 ch29 尾部 1953-01 老秃山（芝山洞西/丁字山 205 高地）之反作：我
  23 军高炮营击落并活捉美第58战斗轰炸机联队副联队长杰爱尔斯上校之侦察 F-86、审讯泄敌轰炸计划敌被迫取消对
  我老秃山空袭——下一批可建专页。
- 更新：korean index（防空役+人物列加彭子新）、timeline 上甘岭主 bullet 加防空侧、防空 org（ch29 反前沿掩护
  段）。战果照书（我方口径）。
- QA：newpages-check 5 文件 CLEAN（无问号/替换符/断链/乱字）；内容页 195→+2=197（QA 为准）。SCHEMA 191cd2 未变。
- 断点：防空书已读至 ch30（激战在大宁江上，raw 15423 起）之前。下批自 ch30 读起。

### 2026-09-05（防空批30 · ch30 大宁江：高炮512团保卫大宁江桥 campaign 页）
- 断点自 ch30（激战在大宁江上，防空txt≈15423-16049）读起。逐章整读后建 1 campaign canonical：
  events/daningjiang-bridge-512reg-1952-11（高炮 512 团保卫大宁江桥 1952-11-01/06；event_type: campaign，
  start 11-01/end 11-06）——反“金化/上甘岭”受挫后敌远东空军在 A/B 线重开铁路封锁、以安州大宁江桥/岭美洞
  便桥为重点。页载：11-1（敌约 3 批 158 架〔战轰〕＋诱导打法；512 团团长高树志先断 F-86 诱、留弹集攻
  俯冲机；各连护桥，11-1 落 7 伤 9、铁桥 3 孔便桥 11 孔连夜修通，敌因烟未照实）→ 11-6（敌 143＋26 F-86+
  16 架；1 营机动至桥北防 I；落 8 伤 7、命中便桥 1.9%，活捉美 58 战轰联队 69 中队中尉巴托）——两日合计
  **落 15 伤 16、江桥不废**。代表人事迹收正文（1连3炮长陈风山对敌恨/续组；电话班长李秋来与阎国祥泅江接线
  交“最后党费”；各连炮手/测手“火线入党/单眼操炮/单臂装填”等）。
- 甄别：512 团长高树志等营指挥/及 上述班长等为单役·连营级 & 全员叙事在正文已足，不另开 person（who's-who
  纪律）；本轮上下文吃紧，若需对代表人物（如李秋来/陈风山）单页可于后续批次 fresh 会话再补（上报明示）。
  [[wu-changchi|吴昌炽]]（铁道高指）统筹，已有专页。无新装备专页（既有 kit；敌 A/B/战轰/B-26/F-86/女妖侦察为
  机型不单建），被俘巴托不立我方人页。
- 更新：korean index（防空役列）、timeline（1952-11 上甘岭后敌重开 A/B 封锁续段上追加此役反封锁）、防空 org
  （批30：512 团守大宁江段；沿用 61 师 533 之前〔归口核〕警示）。
- QA：newpages-check 4 文件 CLEAN（无问号/替换符/断链/乱字）；内容页 197→+1=198。SCHEMA 191cd2 未变。
- 断点：防空书已读至 ch31（异想天开的“购买计划”，raw 16060 起）之前。下批自 ch31 读起。

### 2026-09-05（防空批31 · ch31 抗登陆/安州购买计划：敌谋/守备前置章，org 注；不建战役页）
- 断点自 ch31（异想天开的“购买计划”，防空txt≈16059-16411）整读。属敌侧谋划与战备前置章，防空本线无正面
  空战、无新 行动/装备/代表人物 canonical（敌“以空购买安州运输漏斗〔孟中洞〕”计划与 8-52/登陆判断为背景；
  我方为 1952-12 毛“抗登陆”指示后之反空袭/抗登陆战备布防——以吴昌炽报志司增 512团/502团1营/独立41营/523
  团1营+610团+独立61营 等守安州四个火车站/十几座桥，探照灯421团2连+411团1连组照射、新增 2 部情报雷达与 10
  对空哨+炮连观察员构网），于是本批仅对防空 org 增补该“抗登陆前反空袭布防”结构注（敌我力量敌强我弱、强调一
  以顶十/同时反空降抗登陆），不断章造页。
- 布防与敌谋细节已录 org（防空批31注）供 ch32 安州六昼夜战役之背景。宏观敌登陆判断/反登陆另见官方主干与他源。
- QA：防空 org（1 文件）CLEAN（无问号/替换符/断链/乱字）；内容页仍 198（本批未新增 canonical 页，QA一致）。
  SCHEMA 191cd2 未变。
- 断点：防空书已读至 ch32（安州六昼夜激战，raw 16412 起）之前。下批自 ch32 读起建（已布局拟述防空侧面之六昼
  夜正面战，行动/代表人物/无新装备等将彼时判明后按需开专属页）。

### 2026-09-05（防空批32a（暂停）· ch32 安州六昼夜激战：读 1-9夜~1-10 昼，未写入，转 new-session 续）
- 断点自 ch32（安州六昼夜激战，防空txt≈16412-17740 全章约 1330 行、单日各数千字符）起。因本长会话已连续多轮高密度
  建页（ch26-31 各 1-2 canonical/wiring），上下文逼近安全裕度，按“上下文耗尽→读至断点、写放下批”纪律：本次**只
  读未写**，主动停止以防该章的巨型单日正文在低预算下重演 ch25/26 低质草稿回退。逐日续读/建页应于 fresh 会话重接。
- 已读（供引擎 resume 锚点）：
  · ch32 开篇（第六章）于 1953-01-09 夜起（“远东空军购买安州”计划开始；铁道高指司令[[wu-changchi|吴昌炽]]指挥）。
  · **第一日（1-9 夜）**：敌 B-29 两批西南/西北炸大宁江桥、两批西南/东北炸清川江桥实行“购买”；吴昌炽令打拦阻
    射击（“看不见也要打，把敌拦在投弹圈外”）；512团（高树志）初对前 3 架打偏，改选火网/第四架变航路投偏未中
    目标区；21 时后 12 架 B-29 分炸孟中洞/新老安州站，610团+523团1营以 7 次拦阻火网；探照灯照中一架但 502团 1
    营未与协同/丢射击机会（吴昌炽电话骂解泽霖，其 1营改后迅速捕捉）；后高指命“上空有我机、高炮停射”，夜航机
    攻击未中、敌弃弹返航。此夜战历时 2 小时、拦阻未给敌重创，孟中洞落 160 余枚、大宁江桥坏 1 孔。
  · **第二日（1-10 昼）**：晴；12:34 起 60 架 F-86 拉白烟高空/诱我射击（我高炮不理会）；约 12:46 起 F-84/F-80
    150 余架分西南/东北两方向 2000m 入侵。512团2、3营+502团1营集中火力打散队形、各连打俯冲点；**502团1营1连
    （连长邢绍洲，阵地设于大宁/清川江间 300m 山头，射界佳对双桥威胁最大/成敌重点）**击落一架又一架——读至
    16531 止。
  · 时间/单位/阵位与曾录 org 之“抗登陆前反空袭布防”吻合（512/502·610/523/41·探照灯/雷达哨）；本役将是大宁江
    保卫之后安州反封锁的收束大战。
- 后续锚：续读应从 txt 16532（第二日/1-10 战斗主体）+ 历第三至第六日之正文，全章读毕定其 campaign 页码是否
  为“安州六昼夜 1953-01-09~14”（含可能称第十军民之小高炮等新队与代表人物——彼时再按需开专属页）。勿在低预算
  下续写此章。
- QA：本批不改任何页面、不新增 canonical（内容页仍 198，SCHEMA 191cd2 不变）。
- （提示）ch33（战场奇迹——探照灯照落敌机，raw 17741 起）与 ch32 相邻，fresh 会话续 ch32 后才入 ch33；两章或
  有衔接（探照灯在六昼夜中闪光）宜顺序整读。

### 2026-09-05（防空批32 · ch32 安州六昼夜：战役页 + 邢绍洲人物页；部分日深描留 fresh 续补）
- 断点自 ch32（安州六昼夜激战，防空txt≈16412-17740）起。该战为停战前敌对我抗登陆前最重集中空袭的反制收束。
  逐日脊柱+结尾官方战果小结令本书可核全战役框架，遂建 2 canonical：
  (1) events/anzhou-sixdays-1953（安州六昼夜·反“购买计划”空袭，1953-01-09~15；event_type: campaign）——载敌为
      瘫痪我抗登陆后勤枢纽安州“运输漏斗”〔新安州/岭美洞跨清川·大宁江、孟中洞〕发动日夜不歇大空袭（“购买计
      划”，动用远东空军约 54% 兵力、1166 架次战轰）；我铁道高指（吴昌炽）指挥野战高炮 512/502/523/610/605 团
      及独立 41/46/61 营、探照灯 421/411 团等苦战 **6 昼夜打 9 战 → 击落 15 架/击伤 40 架**；毁清川/大宁江桥
      16 孔、便桥 35 孔（铁道兵抢修）；消耗 85弹 29594＋37弹 36921＋高机弹 34678 发，损坏炮 10 门等，伤 146／
      亡 72。役页另含每“日”脊柱（第1日=1-09夜起，各日日期/敌批数/代表连）、敌“清川以北探照灯不可小觑”自承、
      吴昌炽大会致辞/慰问（藏族战士智花仁谦三等功）等。
  (2) entities/people/xing-shaozhou-502（邢绍洲，野战高炮 502 团 1 营 1 连连长）——其连设大宁/清川江间 300m 山头
      （对双桥/孟中洞威胁最大成敌重点；书另称该带为“两年来十二连轮守、敌称安州上甘岭”钉子），安州六昼夜全役
      贯穿指挥，单开专页。
- 甄别/纪律：各连营指挥与班长英烈（523团2连连长袁绍礼、炮/接线/自衛等）多为单役连级，收役页正文不逐开;502团
  2/3 营等另有侧重故邢单独页。被俘/RB 乘员不立我方人页。无新装备专页：85/37 及探照灯/雷达装备均既有于库。
- 诚实标注：本会话在超长连续批次后上下文已近尽，故 ch32 第 1-10 后连续夜昼细描（1-11 及诸连中段，raw 约至
  17300 前）未逐字核录，役/人页以〔异文核〕/〔续读〕处明记、不臆造细节；如需逐步精读其深描应在 fresh 会话接
  续（另见 ch32a 暂停 log 之间段锚点）。
- 更新：korean index（防空役+人物列加邢绍洲/役）、timeline〔防〕1953-01-09~15、防空 org（批32 役态）。
- QA：newpages-check 5 文件 CLEAN；内容页 198→+2=200。SCHEMA 191cd2 未变。
- 断点：防空书已读至 ch33（探照灯照落敌机，raw 17741）之前。下批续读 ch33 及 ch32 中部未核深描。

### 2026-09-05（防空批33 · ch33 探照灯照落敌机：夜战反护航小型机战例事件页 + org 注）
- 断点自 ch33（战场奇迹——探照灯照落敌机，防空txt≈17741-18140 全章）读起。该章防空主线为 1953 春敌 B-29
  夜轰时派 F-80/F-84/F-94 护航小型机随行压制探照灯/高炮，我探照灯部队以“迎头/散光/模拟跟踪/反干扰”进阶出
  “照落小型机”战例（约 3 个月单独照落 F-80/F-94/F-84/F-84E 4 架）。逐节整读后建 1 canonical：
  events/searchlight-direct-blinding-escort-1953（battle：探照灯照落敌机·夜战反护航，1953-03~06）——载：
  ·421团7连（大宁江）：3-15 夜压缩开灯距/四灯光迎头照落偷袭 F-84（人机俱焚）；4-12 夜多雷达灯锥形照落 F-94
   撞山——一月内 2 架，获志司通报表扬。
  ·401团8连（郭山）：5-3 20:04（B-29 轰郭山桥伴 3 架）以散光/迎头多站接光照落 1 F-84（落草庄里），6 月初再
   照落 1 F-84（中端里）——8 连两度获东北防司通令嘉奖。
  ·战术：敌小型机“怕迎头强光照眼/失明”，我定为保存己方、照落敌机的常训课目；结果敌“谈灯色变”、迫其减少
   夜间攻击探照灯/高炮。
- 归纳/甄别：本试仅开战例事件页；无新装页（探照灯装备已有，且 org〔探照灯〕段落本既有）与无专属人物（7连连
  长/站长与 8 连今未具名、个人不单开）。组织侧（成钧安东防空区 1953-05-03 建、吴昌炽任安州前方指挥所主任、
  第 3 批轮战 542/531/515/501 团接防、安州-水丰-安东三区重点配系〔水丰3层/大孤山6层/安州11层火力〕、探照灯
  421/401/411/431 与雷达 302 营布势等）结构史料存防空 org〔批33〕/可视需要后续在 fresh 建簿。
- 更新：korean index 防空役列、防空 org（批33 探照灯夜战注）。
- QA：newpages-check 3 文件 CLEAN；内容页 200→+1=201。SCHEMA 191cd2 未变。
- 断点：防空书已读至 ch34（最后的狠招——轰炸不设防的水库，raw 18140 起）之前。下批自 ch34 读起（继以 ch35
  胜利的句号收尾）；ch32 中部未核深描与上句组织史料亦可在 fresh 按 log 续。

### 2026-09-05（防空批34a（读记）· ch34 最后的狠招——轰炸不设防的水库 已读；防空专属 canonical 空，停于 ch35 前）
- 断点自 ch34（最后的狠招——轰炸不设防的水库，防空txt≈18140-18584）通读。该章为停战前敌“以炸民生/水坝
  相逼”的战争破坏叙事，防空印本主题无我方正面高炮/探照灯专役（水坝处均不设防）——页级无防空 canonical可从
  防空源得出，本章不新造防空役页。
- 已读书内容要点（按 ch34 供续补或择要成文）：
  · 1953-02-02 艾森豪威尔国情咨文撤台湾中立化（放蒋反攻大陆/两战）；毛 2-07 政协回应对；西方（英等）反对扩
    战。/我方抗登陆 8100 条坑道720公里等海防大纵；高炮/照部署如 org。/敌“购买安州”失败+登陆无望后，克拉克
    援意远东空军炸**约二十余座不设防水库/水坝**（5月上旬/8月两节选择5月插秧期）逼荒饥与断运输。
  · 炸德山水坝（5-13，58 联队 F-84×59投千磅弹/低空无人防、5-15决口，冲垮防水堤/京义铁轨基/顺安机场等）；
    慈山水坝（5-15/16，36+90 架次 F-84，5 命中决口 600m 毁三桥）；旧院街水坝（5-21/29 B-29，朝军民提前放水
    降低水位故不垮）；龟城/德尚水坝（6-13/14 F-84×54/41，水下炸坝顶中 N 处仍无决口，朝军民随炸随修/备土抢
    修保住）——书角度强调美“害民生/毁交通补路”之举与朝中抢修。
  · 敌方牵制空军“猎航组”（320+F-86、万米云上设伏袭我起降机）诱我疏备被打亏后空联司加强警戒；其中 4-07 空
    15 师 43 团韩德彩低油追击击落“双料王牌”费席尔（第 51 联队，被俘）——属空军线（已在 timeline〔空〕4-07
    记），防空源引录作背景。
- 本批不动页（防空 org/索引已足）；内容页仍 201。SCHEMA 191cd2 未变。
- 断点：防空书还余 ch35（胜利的句号，防空txt≈18585 起至书末约 19450）收尾；其上 ch32 中部未核逐日深描、ch34
  这“炸水库”叙事是否要就（朝中抢修抑敌报）作一防空源补充单页可 fresh 自定——现上下文极度吃紧，建议在新会
  话接 ch35（其内容适合作防空源纪年收束与总叙校验）后结束这卷防空专书主题的批续。

 ### 2026-09-05（防空批34b·ch35 胜利的句号：1953-07-20 安州 击落 F-86F 大捷事件页；防空专书主题收尾） - 断点：防空书收官 ch35（胜利的句号，raw≈18585-书末）已读到 7-20 决战与书末段。防空侧收束为一役： events/anzhou-0720-f86f-1953（battle：1953-07-20 安州 敌 F-86F 报复之击落大捷）。 - 载：1953-05 底 F-86F（第8/18联队，时速约1048/升限15200、可携2×1000吨弹机载雷达）入朝；6-07 水丰（504团/ 苏炮营伤 3 败之）、6-30 盖家坝（541团旧装 76.2/日75/S12.7 伤 1、先例）、7-10 安州云下（515团章明加大提前量 落 1 伤 1）为打 F-86F 先后铺垫（底）；7-20（金城后敌最后报复，27 批 196 架次）清川江桥空袭中，安州高炮（510/515/ 523/542/610 团与独立 41/42/43 营，吴昌炽指挥）对来 24 架 F-86F **击落 8 架、击伤 4 架**（含 542团1营 12时正 144 发 1 分钟落 3；敌此后再未犯安州至停战）——防空书收束为“胜利的句号”。 - 关联补：org〔批35〕注并入，见役页；金城/停战（07-27）等背景不另建防空侧页（官方主干他源）。 - 甄别：章明（515团长/原512参谋、安州六昼夜经手）等团长单役不另开人物页（7-20 后如需可后续按需）。无我方新 装备页（F-86F 作敌型记录；我旧装取胜为“复用”战例）。 - 〔注〕：本批仍于超长 TUI 会话低预算环境；已尽纪律用最小验证块建页。防空专书（35×章防空路线）至此从 190→202 canonical 的内容页级摄入基本走完主骨架；ch32 中部逐日细描与书末少量旁段未逐字核记录，若需可在 fresh 会话按 log 续。 - QA：newpages-check 3 文件 CLEAN；内容页 201→+1=202。SCHEMA 191cd2 未变。 - 断点：防空书已通读全书（ch1-35）主要骨架；下一批（若继续）宜在 fresh 会话补 ch32 逐日中段 + 建书末（ch35 后附总叙/图表等）收束或改取另一源（如卷空军/官方）的分线。

### 2026-09-05（防空批36·ch32 安州六昼夜 逐日深描 fresh 重读细补；更新页非开新 canonical）
- 断点：防空主营干已读毕（ch1-35）。本批为 fresh 会话按 log 补 ch32 中部遗留：整读 ch32（raw txt 16444-17754）逐字核录各日深描正文，回补既有 events/anzhou-sixdays-1953 页新增 delimited `## 补充资料（防空书 ch32 逐日深描细分）` 节，不另开 canonical/新页。
- 载（逐日；全按 raw 逐字）：第二日 1-10 = 昼（12:34 F-86×60 诱射探阵→12:46 F-84/F-80×150 两向 2000m；502团1营1连 邢绍洲 300m 山头遭围攻，2炮手张文 25 分 138 发、4炮手张士德牺牲“代我向钢都敬个礼”〔该团原保卫鞍钢〕、卫生员张光斌扑弹牺牲；512团护江桥 8连“引信刻度20直接瞄”首架命中、副连郑克俭护伤员牺牲、连长吴绍洲重伤送院、指导员杜瑞祥持旗）+ 夜间（19:30 F-84×12/F-4U×6/B-29×5 入清川江口施电磁干扰；探照灯技师盛继良关“中放”开关破扰首次反干扰照落战；苏军夜航机凌空打爆第三架 B-29）——当日高炮落 B-29×1+F-84×3 伤 4、友军夜航落/伤 B-29 各 1。1-11 大雪暂停轰炸=休整日（校正读序：非战斗日）。第三日 1-12 昼：23批256架三向；523团1营2连袁绍礼、502团1连邓文标/庞林处置定时炸弹、502团3连（刘景洲/孙忠/刘宗印/朱万富英烈）、512团6/8连、8连天津学生干部代连长刘亚尘“一炮走红”43分落1——当日落伤5、11阵地被攻、伤77损炮7。1-12 夜：两名南朝鲜特工化装伤兵投簧火指引 B-26×2“斩首”铁道高指洞穴指挥所未遂；吴昌炽搜山设防并发电调整部署（512/605 大宁江桥岭美洞、502 团（含价川 2/3 营）孟中里东南、610/611/523团1营+独立41/46营清川江桥新老安州，14 日 6 时备毕）。第四日 1-13 昼两波：110架(F-80/F-84)＋第二波 29批140架 F-80/F-84/F-9F；**523团1营2连“假阵地”换 2 架**（参谋长牛得山设假、营长武天杰、2连袁绍礼首齐放落1＋3连王玉祥 2000m 敲1）；512团5连连长汪金棠 500 发炮弹迫敌弃弹获团长高树志表扬；当日落2伤4、13阵地攻、伤46、85炮损1、两桥炸18孔；晚 61营清川江南→大宁江南、502团2/3营价川中坪入位。第五日 1-14 四面 250 架（F-80/F-84/F-9F/F-51）：敌借烟幕钻我中高炮顶空死区大角度反扣新战术；**512团长高树志“打/轰跑场上 F-84 指挥机”**（2营长安平）+专打贪生怕死被 F-86 驱赶强攻之 F-80（8连刘亚尘齐放击落、俘飞行员自认南韩不值命拼）;解泽霖护 1连命 2/3 营支援（24门小高炮两发撞爆敌机油舱）——当日落2伤3、两桥炸17孔；1连连长邢绍洲头部重伤送野战医院、副连李洪亮代连长；团/高指定“不下 1连阵地”（人在炮在阵地在，以 597.9/537.7 坑道坚持为精神参照；4挺高射机枪+3营支援掩护）；“近战歼敌、放近打”原则重申。第六日 1-15 共约 300 余架四面（东南 F-9F×82）：512层层接力打散、追打清水上级指挥机遁走；502团3营截护 1连打 F-9F 栽江；电话员巴庆禄 6天第12次抢修接通；1连（李洪亮）配 4 高机连退 7 次冲击后移西松里/松风里东南大坝休整。收束：敌“购买安州”11 天计划 6 天夭折止损；美公开评论（《空中威力》170/173 页引）认“对空防御占优势/处处探照灯照夜间B-29/空中突击带冒险性/高炮火像百老汇礼花”；我方铁道高指战斗总结全文（9 战落15伤40、两桥毁16孔便桥35孔、耗85弹 29594+37弹 36921+高机弹 34678、损炮10 等、伤146亡72）+《防空军大事记》引文同口径。
- 甄别：此为本役当日深描补录（页已在上部“逐日脊柱”含总括），**不新开 canonical**：已述团连指挥/英烈（高树志/袁绍礼/吴绍洲/郑克俭/杜瑞祥/刘亚尘/牛得山/武天杰/王玉祥/汪金棠/李洪亮/盛继良/邓文标/庞林/巴庆禄 等）随役随叙、不逐人另开 person（上“甄别/纪律”一致）；502团1营1连/邢绍洲既有人物页不重开；敌 F-84 指挥机/俘飞行与《空中威力》引文均记于役页正文。装备无新增（85/37/高机/探照灯/雷达已有）。
- 更新：events/anzhou-sixdays-1953 页加补充资料节全文；页尾〔异文核〕注同时更新（注明 1-11 为雪休整日、六战役日排定）。index/org/timeline 已在该役原建时接线（防空批32），本批无需重接。
- QA：newpages-check 1 file CLEAN；glitch-scan 全命中为合法白名单 token（型号/wikilink slug/yml 键）无问号/替换符/括号失衡类泄漏；SCHEMA 191cd2 未变；内容页仍 203（无新增页）。
- 断点：防空书 ch1-35 主干 + ch32 逐日深描至此皆完整；下一步可 fresh 补书末（ch35-after 附总叙/装页）或转其它分线。

### 2026-09-05（防空批37·书末衬底溯源——防空书 全 35 章+主线已毕，仅余书末衬底；加史源分注于既有 sources 页，无新建 canonical）
- 断点：防空书（《抗美援朝防空作战实录》）正文至 ch35 已全（防空批34b）＋ch32 逐日深描已回补（防空批36）。本批读到 raw 19450 行书尾，确认其后仅为书末衬底无正文：**主要参考书目**（他源 3 种：《当代中国·抗美援朝战争》；《朝鲜战争中的美国空军1950-53》1961；《空中威力》1957——即各事件页所引美方公开评论之源）＋**「参考回忆片断」25 篇**（参战老兵回忆索引，揭示全书实为这些回忆撮集之纪实、系单侧亲历者口径的结构性根因）＋图片启事。
- 更新：源页 sources/kangmeiyuanchao-fangkong-zuozhan-shilu 新增「书末衬底：主要参考书目与参考回忆片断」节，把 25 篇中可溯者以表格回链到既有事件/org 页（邢绍洲→anzhou-sixdays、牛得山524团→yuanli/dingshanli、郭清江水丰→supung、金波平壤→pyongyang533、夏文进郭山→guoshan、苗树人长甸→yalu-triple、牛万里辑安→jian-mampo、阮松涛奥勃莱→feiliujiang、张菊明→dingshanli、张金凯优待吉本斯→shunchon-aug24、陈文义阳德→yongdok、蔡子悟/汤道成探照灯→防空org 等），并注不另开 canonical。
- 甄别：本批为书尾溯源增补，**无新行动/装备/代表人物 canonical 开页**（衬底不出现既有页外的新战斗/新装备/可立人物；25 篇作者多即既有役页中团连指挥，随役随叙不作新 person）。书主线至此判定**摄入完整**。
- QA：newpages-check 1 source file CLEAN（自加表内 wikilink 全解析；`warn non-SCHEMA key source_kind` 与 glitch hw-punct 行59 TOC 为历史既有、非本次所示）；SCHEMA 191cd2 未变；内容页仍 203（改既有源页、非新增文件）。
- 断点：防空书整本（35 章正文+spine+书末衬底）已全；后续若需新增 canonical 应为另取一源分线（该库既有 空军线 yingjichangkong 或 官方 CAMS 主干线可作下一来源续摄入）按用户指令开页——本条为应对「继续摄入」之书内已穷、非臆造新页。

### 2026-09-29（冷战线批1·新来源⑬ Michael Dobbs《One Minute to Midnight》（古巴导弹危机 1962）开新战争线）
- 来源：/mnt/share/test/One minute to midnight… (Dobbs Michael).epub
  SHA256 36ab4e41012e43b4f072cf4c3aa5e13c014ddcce9d08ea1bde1eeea3d1067c86（与库内既有 hash 全不同，新源）。
- 提取：EPUB 本地解包（zipfile）＋ HTML 正文抽取（未 OCR）→ raw/papers/one-minute-to-midnight-dobbs/
  {one-minute-to-midnight-dobbs.epub, one-minute-to-midnight-dobbs.txt}（79 文档、约 100.9 万字符，
  含 split 分节标记；图片页仅取图注）。
- 判读：本书为**古巴导弹危机**（Cuban Missile Crisis 1962）分钟级叙事史，非本库既有四战（二战/朝鲜/越南/海湾）
  之一 → 按库规**不塞入既有战争线**，新建**冷战线**（核对抗/危机决策）：
  wars/cold-war-cuban-missile-crisis/{index,timeline}。**未改 SCHEMA.md**（沿用既有 type: war / event /
  entity / source；冷战线 = 新战争线，Schema §1 明列可扩展至不同时期战争）。**无 SCHEMA EXTENSION PROPOSAL。**
- 新建（canonical，共 33 个文件）：
  · sources/one-minute-to-midnight-dobbs（来源页；sha256/provenance/结构/性质）
  · wars/cold-war-cuban-missile-crisis/{index, timeline}
  · events（6）：cuban-missile-crisis-black-saturday-1962-10-27（顶点全景）；u2-shootdown-cuba-1962-10-27；
    u2-maultsby-siberia-incursion-1962-10-27；b59-submarine-forced-surface-1962-10-27；
    cuban-missile-crisis-naval-quarantine-1962；cuban-missile-crisis-resolution-1962-10-28
  · entities/equipment（6）：r-12-missile、r-14-missile、fkr-cruise-missile、jupiter-mrmb、
    u-2-reconnaissance、uss-oxford-agtr-2
  · entities/organizations（5）：operation-anadyr、soviet-43-missile-division、excomm、
    jcs-cuba-invasion-plan-1962、sac
  · entities/people（14）：rudolf-anderson、charles-maultsby、vasily-arkhipov、valentin-savitsky、
    nikita-khrushchev、fidel-castro、che-guevara、issy-pliyev、igor-statsenko、
    john-f-kennedy、robert-kennedy、robert-mcnamara、maxwell-taylor、curtis-lemay
- 更新（既有页）：
  · entities/equipment/sa-2-guideline：wars 增 cold-war-cuban-missile-crisis；sources 增
    one-minute-to-midnight-dobbs、us-electronic-warfare-history-vol2-price；补古巴 1962-10-27 击落细节
    （Banes/Gerchenov、Spoon Rest/Fruit Set、下令链 Grechko/Garbuz）；updated→2026-09-29。
  · index.md：战争入口增冷战线；状态节增〔冷战线〕条。
  · concepts/electronic-warfare-cold-war-1946-64：分卷承接增古巴线相参。
- 甄别：不新开跨战争重复页——SA-2 复用既有 canonical（只增补，不另建）；U-2 新建（原库无 U-2 页，检查后确认）；
  敌情人物只建对危机有实质作用的（Khrushchev/Castro/Pliyev/Statsenko/Kennedy 兄弟/McNamara/Taylor/LeMay/
  Anderson/Maultsby/Arkhipov/Savitsky/Guevara），未为一次性配角建页。
- 史料处理：按原书口径记录；作者明示的不确定（赫鲁晓夫对卡斯特罗电文之解读 "correctly or wrongly"、B-59 核鱼雷
  情节源自 Orlov 四十年后回忆）均**照录并标注来源**，不代为坐实；「战果/数字」标原书口径。
- QA：newpages 检查——全部新页 YAML 解析 OK；35 个新/改文件内 wikilink 全部解析（0 断链）；
  SCHEMA 191cd2 未变；raw 已存（原 .epub ＋提取 .txt）；内容页 203 → +33 = 236。
- 断点：本批为冷战线**首批**（源页＋战争线主干＋黑色星期六核心事件/装备/组织/人物骨架）；本书十四章
  之逐章细目（ch4-7 封锁/情报/核弹头细节、Afterword 后续）未逐字深描，可后续按「继续摄入」续补。

### 2026-09-29（冷战线批2·来源⑭ Allison & Zelikow《Essence of Decision》2nd ed.——分析框架+档案修正；无新战争线）
- 来源：/mnt/share/test/Essence of Decision Explaining the Cuban Missile Crisis (2nd Edition) (Graham Allison, Philip Zelikow).epub
  SHA256 25fe96687e966189d33013e40a80dacf5c645db7a0ce3ab559087e95870569fe（与库内 hash 不同，新源）。
- 提取：EPUB 本地解包（zipfile）＋HTML 正文抽取（未 OCR）→ raw/papers/essence-of-decision-allison-zelikow/
  {….epub, ….txt}（17 文档 / 约 112.4 万字符）。
- 判读：本书为**决策分析经典**（Allison 1971 初版 / 1999 二版）——以古巴导弹危机为案例提出三模型
  （理性行动者／组织行为／政府政治），并据 1990s 美苏解密档案**修正第一版史实**。归入**既有冷战线**
  （wars/cold-war-cuban-missile-crisis，批1 已建），**不新建线**；**未改 SCHEMA.md**。
- 新建（canonical，5 文件）：
  · sources/essence-of-decision-allison-zelikow（来源页；sha256/结构/论点/性质）
  · concepts/three-models-government-behavior（三模型分析框架；跨战争/跨事件通用概念）
  · concepts/anadyr-deployment-motives（苏部署动机四假说：古巴保卫/冷战术/导弹力量/柏林 + 危机前信号与误判）
  · events/cuban-missile-crisis-turkey-deal-secret-channel-1962-10-27（土耳其交易公开/秘密双轨）
- 更新（既有页）：events/cuban-missile-crisis-resolution-1962-10-28（加 sources；补苏方 Presidium 决策内情：
  赫氏“为拯救世界必须退却”、Dobrynin 电报抵达时序、Pliyev 被申斥、令苏机停飞）；
  events/cuban-missile-crisis-black-saturday-1962-10-27（加 sources + 三模型关联）；
  wars/cold-war-cuban-missile-crisis/{index,timeline}（加 sources；index 增“分析框架”节与来源；
  timeline 增危机前信号〔析〕条：1962-02/09-04/09-11/09-13/09-19/09-28、5 月动机四假说、土耳其双轨）；
  根 index.md（来源列表增来源⑬⑭、状态节增〔冷战线增补〕条）。
- 甄别（复用/不重复建页）：**不新开** war/event/entity 重复页——Dobbs 批1 已建的 6 事件/6 装备/5 组织/
  14 人物页**全部复用**，本批只补来源与内容；不拆出“Allison 版”平行页（一实体一权威页）。新增仅 2 concept
  （本书独有之分析框架与四假说综合）＋1 event（土耳其秘密通道，Dobbs 页仅略述、本书提供公开/秘密双轨
  与 Bundy 备忘详证，故独立成页并双向链接）。
- 史料处理：两源并列、不强行统一——10-28 撤弹“先于/后于美方加码”之辨（本书据苏档案：赫氏在得知美已
  愿撤土耳其导弹**之前**即选择撤弹；称更贴切类比为《罗生门》而非“Trollope Ploy”）以〔析〕标注来源，
  与 Dobbs 叙述并置；数字/引文按原书口径。
- QA：全部新/改文件 YAML 解析 OK；wikilink 全解析（0 断链）；无重复 canonical 标题；SCHEMA 191cd2 未变；
  raw 已存（原 .epub ＋ 提取 .txt）；内容页 236 → +5 = 241。
- 断点：冷战线现有两源（Dobbs 叙事 + Allison/Zelikow 分析/档案）。本书三模型之其余案例细节（ch4 组织
  细节、ch6 发现/选择之政治全文）未逐字深描，可后续按「继续摄入」续补。

### 2026-09-29（冷战线批3·来源⑮ CIA 官方史《The CIA and the U-2 Program, 1954–1974》——U-2 项目线 + 古巴侦察权威修正）
- 来源：/mnt/share/test/CIA-and-U2-Program.pdf（用户提示：OCR 版，字词或有识别错误）
  SHA256 1012a192f78920dc4370312a48ca3c4a987b50e8ff6dde2712f3d4e001ef53ff（新源）。
- 提取：pdftotext -layout（CIA PDF 自带的 Paper Capture OCR 文本层，未重跑 OCR）→
  raw/papers/cia-and-u2-program-pedlow-welzenbach/{….pdf, ….txt}（272 页 / 约 58.5 万字符）。
  OCR 甄别：识别错字多（如 Volume→voiume、program→program、人名/型号偶错位），引用时对可疑字词标〔OCR〕
  并按上下文校订；部分段落有解密删节（E.O. 12958 §1.5(a)(c)(d)(g)，正文以 ■■■/空白表示），照录不填补。
- 判读：CIA 历史参谋部官方专史（U-2 项目 1954–74）。归入**既有冷战线**（不新建线）——本书之古巴 1962 u-2
  侦察章节属该线；其 U-2 项目起源/发展部分为**新装备项目线**（concept/event/org），亦挂于冷战线。
  **未改 SCHEMA.md。**
- 新建（canonical，4 文件）：
  · sources/cia-and-u2-program-pedlow-welzenbach（来源页；sha256/结构/性质/OCR+删节说明）
  · concepts/u2-aquatone-program（U-2/AQUATONE 项目：缘起、CL-282、保密与掩护、分队制、总统否决权、
    GRAND SLAM、IDEALIST/NIMBUS 代号、OXCART、DS&T 遗产）
  · events/grand-slam-u2-powers-shootdown-1960-05-01（GRAND SLAM 任务、1960-05-01 Powers 被 SA-2 击落、
    自毁装置仅毁相机之澄清、苏营三弹齐射误击友机、巴黎首脑会议破裂）
  · entities/organizations/cia-office-of-special-activities（CIA 特别行动处 OSA；Ledford 1/6 损失率评估、撤编）
- 更新（既有页，据 CIA 档案修正/细化）：
  · entities/equipment/u-2-reconnaissance：加 sources；增“项目与型号背景（CL-282/AQUATONE/IDEALIST/U-2C/
    NASA 掩护/OXCART/U-2R）”；危机作用节增〔CIA 史修正〕——**1962-10-12 古巴 U-2 侦察责任由 CIA 移交
    国防部**、**10-14 首飞发现导弹者为 SAC 飞行员（非 CIA）**、Anderson 所驾为 **CIA 借予空军之 U-2C**、
    9 月收紧航线（in-and-out/避 SAM/云量<25%）、IDEALIST 1961–62 在古巴共飞 **459 小时**、卫星因轨时不利
    而无法替代 U-2 高分辨照相。
  · events/u2-shootdown-cuba-1962-10-27：加 sources；〔CIA 史〕补机源（CIA 借予之 U-2C）与指挥权移交背景、
    危机间 CIA 飞行员未再飞古巴。
  · wars/cold-war-cuban-missile-crisis/{index,timeline}：加 sources；index 增“高空侦察与 U-2 相关事件”节；
    timeline 增 10-12（指挥权移交）〔CIA 史〕条、修订 10-14 与 10-27 条目之〔CIA 史〕注。
  · 根 index.md：来源列表增来源⑮；状态节增〔冷战线增补〕条。
- 甄别（复用/不重复建页）：既有 [[entities/equipment/u-2-reconnaissance|U-2 装备页]]**复用并增补**（不另建
  “CIA 史版 U-2”）；SA-2 页已含 1960/1962 两例，本批以链接互参不重写。新建仅 1 concept＋1 event＋1 org
  （均为本书独有之项目史/官方事件细节）。
- 史料处理：与既有源并列——1962-10-14 发现导弹一事，Dobbs 记 Heyser（CIA 系统飞行员）执飞，CIA 官方史
  明确该次为**空军（SAC）飞行员**执飞（因 10-12 责任已移交国防部）；两说并置并各标来源，不擅断
  （差异或因“飞机归 CIA、飞行员归空军”之双重身份/不同统计口径）。
- QA：全部新/改文件 YAML 解析 OK；wikilink 全解析（0 断链）；无重复 canonical 标题；SCHEMA 191cd2 未变；
  raw 已存（原 .pdf ＋ 提取 .txt）；内容页 239 → +4 = 243。
- 断点：冷战线现有三源（Dobbs 叙事 / Allison-Zelikow 分析 / CIA U-2 官方史）。本书更早章节（战后 RB-47
  渗透、Suez、Lebanon、亚洲 Detachment C/G、OXCART ch6）未逐章深描，可后续按「继续摄入」续补。

### 2026-09-29（冷战线批4·来源⑯ Aid & Wiebes《Secrets of Signals Intelligence during the Cold War and Beyond》——SIGINT 概念与机构线）
- 来源：/mnt/share/test/Secrets of Signals Intelligence during the Cold War and Beyond (Matthew M. Aid,
  Cees Wiebes (eds.)).pdf  SHA256 068990c5c3f9bc7033675aa9cc7d8f716fcab4464c0610ba4143b876eadb81ba（新源）。
- 提取：pdftotext -layout（ABBYY FineReader 8 扫描 OCR 文本层，未重跑 OCR）→
  raw/papers/secrets-sigint-cold-war-aid-wiebes/{….pdf, ….txt}（363 页 / 约 104 万字符）。
- 判读：冷战 SIGINT 史学开创性论文集（Cass Studies in Intelligence）。建立**情报学科/机构线**，与既有
  电子战线互补（EW=对抗，SIGINT=收集）；古巴、朝鲜、越南各线均可挂接。归入冷战线体系，**未改 SCHEMA.md**。
- 新建（canonical，5 文件）：
  · sources/secrets-sigint-cold-war-aid-wiebes（来源页；sha256/结构/10 章/核心论点）
  · concepts/sigint（SIGINT 定义与三分类 Comint/Elint/Fisint + 九大内在特性 + 数据）
  · concepts/ukusa-alliance（英美加澳新 SIGINT 联盟 BRUSA 1946/UKUSA 1948）
  · entities/organizations/nsa（NSA：SSA/OP-20-G→ASA/CSA→AFSA→1952 NSA；规模 30k→65k；70 站网；
    CRITICOMM；146 殉职/60 越南/USS Liberty 34）
  · entities/organizations/gchq（GCHQ：Bletchley→Eastcote→Cheltenham；初期对苏原子弹）
- 更新（既有页）：concepts/electronic-warfare-cold-war-1946-64（加 SIGINT 互参节）；
  wars/cold-war-cuban-missile-crisis/index（加 SIGINT 情报机构节 + 主要来源）；
  根 index.md（来源⑯ + 状态节〔SIGINT 线〕条）。
- 甄别（不重复建页）：Sigint 与既有 Price 卷二之 ELINT/EW 记录**互补不重复**——本批只建“收集/破译/机构”
  层面新页；Elint 交集处互链（[[concepts/sigint]]↔[[concepts/electronic-warfare-cold-war-1946-64]]）。
  第 4-9 章（加 CSE/西德 BND/法/北欧/荷兰/荷兰-印尼）为**国别 SIGINT**，本批未逐章建页（留待续摄或按需）。
- 史料处理：数字（人员/站数/报告量/破译量/殉职数）按原书口径照录；OCR 错字按上下文校订。
- QA：新/改文件 YAML 解析 OK；wikilink 全解析（0 断链）；无重复 canonical 标题；SCHEMA 191cd2 未变；
  raw 已存（原 .pdf ＋ 提取 .txt）；内容页 243 → +5 = 248。
- 断点：国别章节（加/西德/法/北欧/荷兰/荷兰-印尼）与 ch10 结论未逐章深描，可后续按「继续摄入」续补。

### 2026-09-29（冷战线批5·来源⑰ Taubman《Secret Empire》——越顶侦察全景（U-2/SR-71/CORONA 卫星）线）
- 来源：/mnt/share/test/Secret empire Eisenhower, the CIA, and the hidden story of Americas space
  espionage (Taubman, Philip).pdf  SHA256 d9d7fcf7715ee95416bb2fafbcd0740818088f222f640e5b2ce4640b023af85e（新源）。
- 提取：pdftotext -layout（Internet Archive 扫描 OCR 文本层，未重跑 OCR）→
  raw/papers/secret-empire-taubman/{….pdf, ….txt}（约 1.09 万行 / 108.8 万字符）。
  OCR 甄别：错字多（如 "Chapter Fight"="Chapter Eight"、"ANCT"="AND"）；对可疑处标〔OCR〕按上下文校订。
- 判读：记者视角的越顶侦察史（U-2→SR-71→CORONA 卫星；艾森豪威尔—CIA 秘密体系）。归入冷战线体系，
  新建“越顶侦察·卫星线”；**未改 SCHEMA.md**。
- 新建（canonical，4 文件）：
  · sources/secret-empire-taubman（来源页；sha256/结构/核心叙事与判断/OCR 说明）
  · concepts/corona-reconnaissance-satellite（CORONA 照相侦察卫星：Sputnik 冲击→立项、Discoverer 掩护、
    Agena、胶片回收、覆盖 vs 清晰度、古巴危机“完全无用”判断、导弹差距核实）
  · events/discoverer-xiv-first-film-recovery-1960-08-19（1960-08-18 发射/08-19 空中钩取胶片舱成功；
    与 Powers 宣判同日；判读首见“六至七条宽条纹”）
  · entities/organizations/cia-directorate-science-technology（CIA 科技处 DS&T；Bissell→Wheelon）
- 更新（既有页）：concepts/u2-aquatone-program（增“与卫星线之衔接”节：CORONA/Discoverer/DS&T 互链 +
  Taubman 之“卫星在古巴危机无用”注）；wars/cold-war-cuban-missile-crisis/index（增“越顶侦察·卫星线”节 +
  主要来源 + sources）；wars/cold-war-cuban-missile-crisis/timeline（增“越顶侦察·卫星（旁注）”节 +
  sources）；根 index.md（来源⑰ + 状态节〔卫星线〕条）。
- 甄别（复用/不重复建页）：**不另建**平行 U-2 页（复用 [[entities/equipment/u-2-reconnaissance|U-2]] 与
  [[concepts/u2-aquatone-program|AQUATONE 项目]]，只做互链增补）；SA-2、CIA OSA 等既有页仅互链不重写。
  新建仅卫星/DS&T 三页（本书核心且库内此前无）。
- 史料处理：**重要侧证**——Taubman（据 Wheelon 回忆）称“CORONA 在 1962-10 古巴危机中完全无用（回放太慢）”，
  与 CIA U-2 史“卫星因轨时不利无法替代 U-2”之记载**相互印证**，本库并列标注来源，不擅断。
- QA：新/改文件 YAML 解析 OK；wikilink 全解析（0 断链）；无重复 canonical 标题；SCHEMA 191cd2 未变；
  raw 已存（原 .pdf ＋ 提取 .txt）；内容页 248 → +4 = 252。
- 断点：本书更早/更晚章节（兰德 ch3、U-2 早期越苏 ch7-9、SR-71/A-12 细节、Epilogue）未逐章深描，
  可后续按「继续摄入」续补。

### 2026-10-05（电子战技术概念层·来源⑱ Adamy《EW 101》——技术参考资料模式摄入）
- 来源：/mnt/share/test/EW 101  a first course in electronic warfare (Adamy, David)
  (z-library.sk, 1lib.sk, z-lib.sk).pdf（注意实际目录为小写 /mnt/share/test/）
  SHA256（PDF）e080727ee8aaea1aa7b595bc697f17c2380983c2189bac6164f2d2fed8b42275（新源，库内无重复）。
- 提取：pdftotext -layout（Internet Archive 扫描，344 页，文本层完好，未跑 OCR）→
  raw/papers/ew-101-adamy.{pdf,txt}（约 1.478 万行 / 71.3 万字符；
  提取文本 SHA256 30b55351d5e0895ecfaabcf990acc59b81e9da83fff309d3c2b2588609feade2）。
- 摄入定位（按用户指示）：**technical reference 模式**——优先提取具有长期研究价值、可跨战争复用的
  技术概念/原理/分类/参数关系/公式/作战意义，增量补齐本库**此前缺失的电子战技术概念层**；
  **不**机械按章建页；**不**以教材性技术说明代替具体历史事件的史料证据；历史事实/装备运用/时期术语
  仅在本书明确提供证据时摄入（本批判断：该书为入门技术教材，无足量一手史料，故未据其新增历史实体/事件）。
- 新建（canonical，11 文件）：
  · sources/ew-101-adamy（来源页；sha256/11 章结构/关键公式索引/局限说明）
  · topics/electronic-warfare-technical-foundations（**专题枢纽；topics/ 首次启用**）
  · concepts/ew-link-equation-and-db-math（dB 数学、单向链路方程、扩散/大气损耗、灵敏度与有效距离、
    雷达距离方程链路化、干扰信号差、球面三角与多普勒/观测角）
  · concepts/ew-antenna-parameters（波束定义、增益-波束-面积关系式、极化技巧、类型选型表、抛物面权衡、相控阵）
  · concepts/ew-receiver-architecture（九类接收机 Table 4.1/4.2 分类与能力矩阵）
  · concepts/ew-processing-and-threat-id（威胁识别逻辑、PRI/DOA 等参数、去交错、人机界面）
  · concepts/emitter-location（定位目的与精度 Table 8.1、精度预算与校准、测向/定位技术 Table 8.3、
    幅度/Watson-Watt/干涉仪/多普勒/TOA/TDOA）
  · concepts/jamming（干扰四分类、J/S 方程（通信/远距/自卫）、烧穿距离、覆盖/欺骗、RGPO/RGPI/逆增益/
    AGC/VGPO、对单脉冲雷达欺骗手法）
  · concepts/radar-decoys（诱饵类型与三任务、RCS 反射增益公式 −39+10logσ+20logF、被动/主动、有效 RCS 随几何变化）
  · concepts/lpi-signals（LPI 手段、跳频/chirp/直接序列扩频及探测-截获-定位-干扰）
  · concepts/ew-simulation（建模/仿真/仿真注入三分法、注入点分级、威胁与天线方向图仿真、保真度）
- 更新（既有页）：根 index.md（新增“专题研究”入口节；来源⑱ 条；状态节〔电子战技术概念层〕条；
  “尚未建立 topics/”改注为已启用）。各概念页相互 wikilink 并与既有电子战线（WWII/冷战早期/SEAD/SIGINT）
  及装备页（Shrike/HARM/SA-2/QRC-160/ALQ-119 等）互链。
- 史料处理：技术概念页均标“非史料”；J/S、烧穿、RCS 反射增益等**公式录入**但不据以断言任何历史战果；
  教材图表 OCR 错乱处（如 Table 4.2 能力矩阵、部分行内公式）以正文叙述核对，未据乱码臆造数值，
  已在来源页“注意与局限”注明。
- QA：11 新文件 YAML 全解析 OK（修正来源页标题未加引号的冒号问题 1 处）；wikilink 全解析（0 断链，
  修正初稿 4 处断链/误链：radar-decoys 的 ad、lpi-signals 的 frequency-hopping、
  ew-antenna-parameters 的 dipole/dish-antenna 及 1 处嵌套括号链接）；无重复 canonical 标题；
  SCHEMA.md 未改动（sha256 191cd20f951e… 未变）；raw 已存（原 .pdf ＋ 提取 .txt）。
- 断点：本书为纯技术参考，**无逐章续摄需求**；后续如需可再据其补 Eq/图（如 Table 4.2/8.3 完整矩阵）。

### 2026-10-05（电子战技术概念层·续·来源⑲ Adamy《EW 102》——技术参考资料模式摄入）
- 来源：/mnt/share/test/EW 102 A Second Course in Electronic Warfare (David Adamy)
  (z-library.sk, 1lib.sk, z-lib.sk).pdf  SHA256（PDF）3a609e246feaec28103f9fa23c0b39d5a04a77893a2eaee4ea2547d4af82aa8b（新源）。
- 提取：pdftotext -layout（Adobe Acrobat 生成，291 页，文本层完好，未跑 OCR）→
  raw/papers/ew-102-adamy.{pdf,txt}（约 1.098 万行 / 52.0 万字符；
  提取文本 SHA256 658fd6c8396eab083eb41fdcb6223960a2ec222f964d1ca7a9940a707b355fbb）。
- 摄入定位（按用户指示）：**technical reference 模式**（同来源⑱ EW 101 批次）——优先提取可跨战争
  复用的技术概念/分类/参数关系/公式/作战意义，增量扩展本库电子战技术概念层；不机械按章建页；
  不以教材性技术说明代替史料；历史事实/装备运用/时期术语仅在本书明确提供证据时摄入（本批判断：
  该书为入门技术教材，无足量一手史料，故未据其新增历史实体/事件）。
- 新建（canonical，8 文件）：
  · sources/ew-102-adamy（来源页；sha256/7 章结构/关键公式索引/局限说明）
  · concepts/ew-threats-and-guidance（威胁定义与类型、四类制导方式、频段三套划分、威胁雷达扫描
    （圆周/扇扫/光栅/圆锥/单脉冲/仅收扫描）与调制（截获/跟踪/引信参数）、通信信号威胁）
  · concepts/radar-characteristics（雷达功能与分类、雷达距离方程三形式+dB 形式、脉冲调制与脉冲压缩、
    CW/脉冲多普勒/FM 测距、MTI/AMTI、SAR（距离/方位分辨、聚焦阵））
  · concepts/lpi-radar（LPI 三途径与三层级、LPID/安静/随机信号雷达、bandwidth advantage/相干检测、
    range detection ratio/告警时间图数）——与通信侧 lpi-signals 互补
  · concepts/infrared-electro-optical-ew（IR 频谱分带、黑体辐射、IR 制导导弹/导引头/调制盘（旭日/
    车轮/多频/曲辐条）、IRLS 探雷算例、FLIR/IRST、夜视三代、激光指示/告警、IRCM）
  · concepts/ew-against-communications（HF 电离层/单站定位、VHF/UHF 三传播模型（自由空间/双径/
    菲涅尔区/刀边）、背景噪声、数字通信（调制/BER/kTB/带宽）、通信干扰、对跳频/DSSS 干扰量化、
    纠错码、扩频发射机定位）
  · concepts/emitter-location-accuracy（定位三途径、角度测量技术与精度、TDOA/FDOA 精确定位、
    RMS/CEP/EEP 度量（1.037σ）、误差预算与平方和合成）——深化来源⑱的 emitter-location
  · concepts/satellite-communication-links（EIRP/G-T/Q 术语、噪声温度体系（天线/馈线/接收机+级联
    首级主导）、链路损耗（扩散/大气/雨雾/法拉第）、链路性能、与 EW 链路方程的关系、下链/上链干扰）
- 更新（既有页）：topics/electronic-warfare-technical-foundations（**重构**为完整技术层入口，纳入
  上述 7 新页，sources 增 ew-102-adamy）；根 index.md（专题研究入口加列新页；来源⑲ 条；状态节
  〔电子战技术概念层·续〕条）。
- 史料处理：技术概念页均标“非史料”；雷达距离方程、J/S、kTB、噪声温度、CEP/EEP 等**公式录入**但
  不据以断言任何历史战果；教材图表 OCR 错乱处（频段表/Table 5.3/部分行内公式）以正文核对，
  未据乱码臆造数值，已在来源页“注意与局限”注明。
- QA：8 新文件 YAML 全解析 OK；wikilink 全解析（0 断链）；无重复 canonical 标题；SCHEMA.md 未改动
  （sha256 191cd2… 未变）；raw 已存（原 .pdf ＋ 提取 .txt）；本批 EW 102 新增 8 页（1 source＋7 concept），
  与来源⑱ EW 101 批 11 页互链，构成完整电子战技术概念层。
- 断点：本书为纯技术参考，**无逐章续摄需求**；EW 101/102 全书七/十一章技术主线已覆盖。

### 2026-10-05（电子战技术概念层·通信专项·来源⑳ Adamy《EW 103》——技术参考资料模式摄入）
- 来源：/mnt/share/test/EW 103 - Tactical Battlefield Communications Electronic Warfare
  (David L. Adamy) (z-library.sk, 1lib.sk, z-lib.sk).pdf  SHA256（PDF）
  423dd47c1e65f7bd2a5486990909b7fc23ae946075a637e76b131a7d42ef0daf（新源）。
- 提取：pdftotext -layout（PDFsam 拼接，348 页；文本层完好，未跑 OCR。提取时 pdftotext 报大量
  "Bad annotation destination" 警告，属 PDF 书签噪声，不影响正文）→
  raw/papers/ew-103-adamy.{pdf,txt}（约 1.413 万行 / 63.3 万字符；
  提取文本 SHA256 23fca8edbad6d652c58636f8ad2691d58308da4b5c7e74544477c673287426e9）。
- 摄入定位（按用户指示）：**technical reference 模式**（同来源⑱⑲）——优先提取可跨战争复用的技术
  概念/分类/参数关系/公式/作战意义；不机械按章建页；不以教材性技术说明代替史料；历史事实/装备
  运用/时期术语仅在本书明确提供证据时摄入（本批判断：入门技术教材，无足量一手史料，未据其新增
  历史实体/事件）。
- **重叠判定（关键）**：EW 103 与 EW 101/102 在**天线、接收机、传播模型、J/S、LPI、定位精度**上
  系统重叠 → **优先增量更新既有概念页**，仅对**通信搜索/截获/定位**等新主题建新页，避免重复建页。
- 新建（canonical，4 文件）：
  · sources/ew-103-adamy（来源页；sha256/9 章结构/关键公式索引/重叠与局限说明）
  · concepts/communications-search-and-poi（Ch6：POI 定义、三类搜索策略（一般/定向/顺序甄别）、
    能量检测接收机（积分-倾倒/相关/机载码片/二元滑动窗/并行）、信号环境与角度覆盖、无线电视距
    D=4.12(√H_T+√H_R)、LPI 搜索、look-through、自相残杀、窄带搜索算例）
  · concepts/communications-intercept（Ch8：COMINT vs 通信 ESM、截获链路方程 P_R=P_T+G_T−L+G_R、
    定向/非定向截获、机载/非视线截获、强信号中截获弱信号、LPI 截获）
  · concepts/communications-emitter-location（Ch7：三角定位/单站定位 SSL(<30MHz HF)/方位仰角、
    精度定义与 CEP 近似 CEP=1.17·d·tan(RMS)、站点与北向基准、Watson-Watt/多普勒/干涉仪测向、
    TDOA/FDOA 精确定位（isochrone/isofreq）、误差预算、扩频辐射源定位）
- 增量更新（既有页）：
  · concepts/ew-against-communications（增“通信信号与干扰（据 EW 103 增量）”节：模拟 β/数字带宽
    Table 2.1/MSK、数字信号结构、组合 LPI、手机信号（FDMA/TDMA-GSM/CDMA）、通信干扰补充（J/S 一般式/
    33%/脉冲/处理增益/部分频带/stand-in/干扰手机）；修重复编号；sources 增 ew-103）
  · concepts/ew-link-equation-and-db-math（增“刀边衍射 KED 与天线有效高度”节；sources 增 ew-103）
  · concepts/ew-receiver-architecture（增“灵敏度、动态范围与系统配置”节：S=kTB+NF+RFSNR、I&Q、
    码片检测、动态范围、遥控接收系统；sources 增 ew-103）
  · concepts/ew-antenna-parameters（增“通信天线类型”节：鞭状有效高度/对数周期/抛物面盘/DF 阵列偶极子
    匹配网络增益损失；sources 增 ew-103）
  · topics/electronic-warfare-technical-foundations（补“通信 EW 专项（据 EW 103）”节；sources 增 ew-103；
    来源说明增 EW 103）；根 index.md（专题入口列新页；来源⑳ 条；状态节〔通信专项〕条）。
- 史料处理：技术概念页均标“非史料”；截获链路、通信 J/S、CEP 近似、无线电视距等**公式录入**但不据以
  断言任何历史战果；教材图表 OCR 错乱处以正文核对，未据乱码臆造数值，已在来源页“注意与局限”注明。
- QA：4 新文件 YAML 全解析 OK；wikilink 全解析（0 断链）；无重复 canonical 标题；SCHEMA.md 未改动
  （sha256 191cd2… 未变）；raw 已存（原 .pdf ＋ 提取 .txt）。
- 断点：本书为纯技术参考，**无逐章续摄需求**；EW 101/102/103 三部技术主线已覆盖。

### 2026-10-05（电子战技术概念层·新一代威胁·来源㉑ Adamy《EW 104》——技术参考资料模式摄入，EPUB）
- 来源：/mnt/share/test/EW 104 Electronic Warfare Against a New Generation of Threats
  (David L. Adamy) (z-library.sk, 1lib.sk, z-lib.sk).epub  SHA256（EPUB）
  0368d07b6247973d7b27563fa073ce84cf27ff460d3b104233a2af170262f979（新源）。
- 提取（**EPUB 流程**，按 Skill 第 4 节）：本地 unzip 解包 → OEBPS/Text/part0000–0019.xhtml 共 20 段，
  剥离 script/style/tag、按 block 标签重建换行、html.unescape，**保留章节顺序**；跳过封面/版权/目录等
  非正文（仅保留其文本供导航核对）。未跑 OCR。→ raw/papers/ew-104-adamy.{epub,txt}
  （提取文本 SHA256 8f5913aaddb7722ee02a08db0e90177be540c074410d4d9dc15f3a495d556955；约 68.8 万字符）。
- 摄入定位（按用户指示）：**technical reference 模式**（同来源⑱⑲⑳）——优先提取可跨战争复用的技术
  概念/分类/参数关系/公式/作战意义；不机械按章建页；不以教材性技术说明代替史料；历史事实/装备运用/
  时期术语仅在本书明确提供证据时摄入。本书**确有**据开放源转录的新一代威胁型号参数，已照录并**明确
  标注系本书据开放源、非一手史料**；未新增历史实体/事件。
- **重叠判定（关键）**：EW 104 与 EW 101/102/103 在**传播模型、J/S、天线、接收机、截获/搜索/定位、
  干扰/诱饵、IR**上系统重叠 → **优先增量更新既有页**，仅对**频谱战概念层、雷达电子防护、DRFM、
  ES vs SIGINT** 等新主题建新页，避免重复建页。
- 新建（canonical，5 文件）：
  · sources/ew-104-adamy（来源页；sha256/11 章结构/关键公式索引/开放源性质说明）
  · concepts/spectrum-warfare-ems（Ch2：EMS 第五作战域、连通性四要求、网络中心战、传输安全 vs 消息
    安全、赛博战 vs EW（ES/EA/EP↔间谍软件/拒止/防护）、隐写术、链路干扰与抗干扰）
  · concepts/radar-electronic-protection（Ch4：雷达 EP 技术 Table 4.1 及对抗（超低旁瓣/旁瓣对消/匿隐/
    单脉冲/抗交叉极化/脉冲压缩/RGPO/AGC/Dicke-Fix/PD 雷达 EP/相干干扰/频率捷变/PRF 抖动/寻的干扰）；
    PD 处理增益=CPI×PRF、距离/多普勒模糊、低/中/高 PRF；威胁系统升级据开放源；EW 影响小结）
  · concepts/digital-rf-memory（Ch8：DRFM 框图、宽带/窄带、对脉冲压缩/频率捷变/前沿跟踪的对抗、
    相干干扰（处理增益 28.4 dB 算例）、复杂假目标、时延需<脉冲间期、约 50 ns 捕获、需 DRFM 的雷达技术小结）
  · concepts/electronic-support-vs-sigint（Ch11：ES vs SIGINT Table 11.1、COMINT/ELINT、天线/距离/
    接收机/搜索/处理差异）
- 增量更新（既有页）：
  · concepts/jamming（增“雷达干扰技术分类（据 EW 104）”节：阻塞/点/扫频点/欺骗+各手法；sources 增 ew-104）
  · concepts/infrared-electro-optical-ew（增“照明弹战术/跟踪器/干扰机（据 EW 104）”节：诱离/迷惑/稀释+
    定时/光谱；rosette/交叉线阵/成像跟踪器；热砖/DIRCM 激光干扰机；sources 增 ew-104）
  · concepts/radar-decoys（增“部署型式/保真/舰船诱饵”节；sources 增 ew-104）
  · concepts/ew-against-communications（增“数字通信链路与抗干扰余量（据 EW 104）”节；sources 增 ew-104）
  · topics/electronic-warfare-technical-foundations（补“概念/条令层”节，纳入频谱战/ES vs SIGINT；
    威胁与信号源加雷达 EP；对抗加 DRFM；sources 增 ew-104；来源说明增 EW 104 四册）；根 index.md
    （专题入口列新页；来源㉑ 条；状态节〔新一代威胁〕条）。
- 史料处理：技术概念页均标“非史料”；书内据开放源转录的威胁型号参数（S-300/SA-10/12/6/8、MANPADS、
  AAA 升级等）照录于雷达 EP 页并标注“本书据开放源、非一手史料”；公式录入但不据以断言历史战果；
  EPUB 文本质量好，未见 OCR 乱码问题。
- QA：5 新文件 YAML 全解析 OK；wikilink 全解析（0 断链）；无重复 canonical 标题；SCHEMA.md 未改动
  （sha256 191cd2… 未变）；raw 已存（原 .epub ＋ 提取 .txt）。
- 断点：本书为纯技术参考，**无逐章续摄需求**；EW 100 系列四册（101–104）技术主线已全部覆盖。

### 2026-10-05（电子战技术概念层·空间 EW·来源㉒ Adamy《EW 105》——技术参考资料模式摄入，PDF）
- 来源：/mnt/share/test/Ew 105 Space Electronic Warfare (Artech House Electronic Warfare Library)
  (David L. Adamy) (z-library.sk, 1lib.sk, z-lib.sk).pdf  SHA256（PDF）
  7ee807af6cc7fc3b51daa577902b59a6b93d89be4d771992cd8dd01edfc014e6（新源）。
- 提取：pdftotext -layout（zip-deflate 编码，228 页；文本层完整，未跑 OCR。提取时打印
  "Bad annotation destination"/"xref num not found" 警告，属 PDF 结构噪声，不影响正文）→
  raw/papers/ew-105-adamy.{pdf,txt}（约 7,292 行 / 32.8 万字符；
  提取文本 SHA256 43f626ac996136caeae0491fefe07cf02187b1b6ee3afa0eb4d7c2b53ce34758）。
- 摄入定位（按用户指示）：**technical reference 模式**（同来源⑱–㉑）——优先提取可跨战争复用的技术
  概念/分类/参数关系/公式/作战意义；不机械按章建页；不以教材性技术说明代替史料；历史事实/装备运用/
  时期术语仅在本书明确提供证据时摄入。本书提供少量史实（1960 西方开始发射成像/SIGINT 卫星；NRO 1994
  出版、2016 解密其侦察卫星项目史），仅简要摄入；**大量算例系演示用合成数据**（作者反复声明“非真实
  系统”），已明确标注；未新增历史实体/事件。
- **重叠判定**：EW 105 与既有页在**传播模型、J/S、球面三角、天线**上有重叠，且 Ch4（大气内传播）
  与 EW 103 高度重合 → **优先增量更新**；本书**独有空间 EW 方向**为主要增量，建新页。
- 新建（canonical，8 文件）：
  · sources/ew-105-adamy（来源页；sha256/10 章+3 附录结构/关键公式索引/合成数据说明）
  · concepts/orbit-mechanics-for-ew（Ch3：开普勒六根数、开普勒第三定律 a³=CP²、静止/GPS/低轨、
    SVP、球面三角形求地心角/方位/距离/仰角、地平线距离 C=arccos(RE/(RE+H)) 与表 3.3）
  · concepts/space-radio-propagation（Ch5：空间 LOS 损耗 32.44+20logd+20logF、盘天线增益/波束宽度、
    大气损耗随仰角、天线失配 ΔG=12(θ/α)²、极化损耗（法拉第旋转/圆-线 3dB）、雨衰 0°C 等温线）
  · concepts/satellite-links（Ch6：链路几何、上行（指令/拦截）、下行（遥测/数据/用户/干扰）、敌对链路）
  · concepts/satellite-link-vulnerability（Ch7：截获/欺骗/干扰（上/下行）、下行/上行截获、下行/上行
    干扰 J/S、卫星链路 EP（纠错/多数编码/扩频·跳频 vs DSSS）、0dB J/S+25% 误码判据）
  · concepts/satellite-observation-duration（Ch8：地平线距离、地心视角、地球自转 0.25068°/min、
    观测时长公式 T=P[2arccos(RE/a)][1+cos(i)cos(lat)]、多普勒 ΔF=FVcosθ/c）
  · concepts/intercept-from-space（Ch9：LEO 截获雷达信号（地心角→链路距离→各损耗→灵敏度 S=kTB+NF+RFSNR
    →链路余量→地平线判据→可观时长）、窄波束截获、GEO 截获）
  · concepts/jamming-from-space（Ch10：空间干扰通信网/数据链/雷达、远距雷达 J/S 公式、天线失配、
    低 RCS 杠杆（10m²→10⁻⁴m² 使 J/S −0.5→49.5 dB）、时长 12.2min、静止轨道降 40dB）
- 增量更新（既有页）：concepts/satellite-communication-links（增“卫星链路几何与链路类型（据 EW 105）”
  节；sources 增 ew-105）；topics/electronic-warfare-technical-foundations（补“空间 EW”节，纳入 7 新页，
  来源说明增 EW 105 五册；sources 增 ew-105）；根 index.md（专题入口列空间 EW；来源㉒ 条；状态节
  〔空间 EW〕条）。
- 史料处理：技术概念页均标“非史料”；书内**大量算例标注为演示用合成数据（非真实系统）**；少量史实
  （卫星项目史）按原书照录；公式录入但不据以断言历史战果。PDF 警告为结构噪声，正文完整。
- QA：8 新文件 YAML 全解析 OK；wikilink 全解析（0 断链）；无重复 canonical 标题；SCHEMA.md 未改动
  （sha256 191cd2… 未变）；raw 已存（原 .pdf ＋ 提取 .txt）。
- 断点：本书为纯技术参考，**无逐章续摄需求**；EW 100 系列五册（101–105）技术主线已全部覆盖。
### 2026-10-22（十月战争线·来源㉓ Rabinovich《The Yom Kippur War》——骨架批，PDF 扫描）
- 来源：/mnt/share/test/The Yom Kippur War  the epic encounter that transformed the Middle East
  (Rabinovich, Abraham) (z-library.sk, 1lib.sk, z-lib.sk).pdf　SHA256（PDF）
  5a434a195a13d06c1323964611847e37c4a8366dcf73a388291177392777628b（新源，库内无同 hash）。
- 提取：pdftotext -layout（596 页 Internet Archive Scribe 扫描件，未跑 OCR）→
  raw/papers/yom-kippur-war-rabinovich/{yom-kippur-war-rabinovich.pdf,.txt,.paged.txt}
  （正文 147 万字符／23,364 行；paged 版按扫描页加 [[PAGE n]] 标记便于定位）。
  文字层质量：正文页可用（无 U+FFFD），但照片/地图页与运行页眉严重混杂，地图地名与路线不可依
  文字层判读——本批建页凡涉地名/象征均只取正文叙述，未从地图文字层取名。
- 章图：据印刷目录与正文首标题重建 38 章＋Prologue 的章—扫描页对照，写入 sources 页表格
  （ch1 p24 … ch38 p478；图版页 18–19/26/31 章间、296–308 等为纯图片页）。
- 新建（6 文件）：
  · sources/yom-kippur-war-rabinovich（来源页：provenance/章页对照/来源性质/时间折算规则）
  · wars/yom-kippur-war/index（新战争线索引：南线/北线/空中/情报/超级大国/装备/部队/人物/地点分栏）
  · wars/yom-kippur-war/timeline（主时间线：1973-09-22 定 D 日 → 1974 脱离接触；日期均据原文，
    只给星期处按 10-06=星期六换算并标注）
  · events/operation-badr-1973（埃军渡河战役：零时 14:00、炮火首分钟万余发、第一波 4,000 人/720 舟、
    23,000→32,000 人、22:30 十二桥开通、每师约 72 Sagger＋535 RPG）
  · concepts/dovecote-plan（以军静态防御预案与 10-06 失效）
  · concepts/operation-tagar（对埃 62 个 SAM 阵地的四波次集群攻击预案与 10-07 取消）
- 增量更新：events/yom-kippur-1973-air-sam-ew（既有 Price 卷III EW 页）：frontmatter 加 wars/sources，
  正文加"补充资料（第 1 批）"节（不先发制人的政治否决与天气、Tagar 取消、Dougman 5 仅毁 1 阵地
  损 6 架、头两日 35 架/前四日 49 架与 500 辆坦克、大马士革空袭、48 架直升机被击落 20 架）。
- Index：根 index.md 战争入口增十月战争条、来源条增㉓、状态节增十月战争线一条；
  战争索引中尚未建页的条目暂以纯文本列出（不预置断链）。
- 已读并在本批取用的章：Prologue、ch3–ch5、ch7–ch14、ch16–ch25、ch26–ch29（取用部分）、
  ch30–ch34（取用部分）、ch37/ch38（越接触/Agranat/萨达特访以/1977）。
- 断点（下一批起读）：**南线 10-08 以军反攻失败（ch12 末、ch20–ch21 尚未细读）、10-14 埃军装甲
  反攻（ch29 中段）、Abirei Lev 渡河与 Chinese Farm 全章（ch30–ch31 只读首尾）、Abirei Lev 破出
  （ch33–ch34 部分）、苏伊士城（ch35 后段）、核警报（ch37）**；北线 **Kuneitra 缺口（ch19–ch20）、
  Nafakh 之战（ch21）、赫尔蒙山（ch16）、戈兰反攻（ch24–ch25）**、伊拉克远征军（ch25）、
  美苏空运（ch26）、Agranat（ch38 已读）。另 ch1/ch2/ch6 尚未读（战前政治与社会背景）。
- 异常／甄别：本书为以色列视角叙事史，阿拉伯官方战史缺位（作者自述），阿方数字多为回忆录转述；
  战果数字一律标"据本书"；出版社日期 2004（版权页），Schocken Books。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 295；新页 newpages-check 无字节问题
  （仅 source 页 SCHEMA 允许的 provenance 键告警）；wikilink 全部解析（0 断链）；
  glitch-scan 仅报专名/型号（模型白名单外英文），无乱码、无占位符。

### 2026-10-22（十月战争线·第 2 批：南线 10-08 反攻失败＋北线戈兰全战役）
- 来源同批 1（[[yom-kippur-war-rabinovich]]，sha256 5a434a19…），无新增原始资料；本批只做逐章建页。
- 本批读章：ch17、ch19、ch20、ch21、ch22、ch23、ch24、ch25、ch26（政治段）、ch28、ch29、ch31、ch34（渡河段）。
- 新建（9 页）：
  · events/yom-kippur-1973-idf-counterattack-failure（10-08 Hizayon/Hamutal：Gonen 擅改埃拉扎尔限定、
    Sasson 越权令、Adini 营 21 辆返 14 可用 7 亡 19、Yaguri 营 18 辆返 4、Sharon 拒借兵、假"已渡河"情报、
    傍晚后撤止损；Adan 师损约 50 辆）
  · events/dougman-5-1973（60 架 F-4、仅毁 1 个阵地、6 架被高炮击落、Ivri 的"推迟两小时"评估）
  · events/kuneitra-gap-battle-1973（第 7 旅四天防御：177 对 1,400 辆、土台射击、10-09 Kahalani 重占土台、
    谷底 260 辆、四天叙军在戈兰弃逾 800 辆）
  · events/nafakh-base-battle-1973（Force Zvika、Tiger Company Reshet 设伏、Sarig 旅 Katsbiya、
    Barak 营 Ramtania 被击退、Ben-Shoham 与副旅长阵亡、Zurich 堵路）
  · events/israeli-hermon-fall-1973（55 人中 13 死 31 俘、叙第 82 伞兵营、设施完好被夺）
  · events/golan-heights-campaign-1973（战役总览：兵力、日序、作者三条解释）
  · events/golan-counteroffensive-1973（10-10 九小时决策—越紫线；Eitan/Laner 两师；Sasa 受阻；
    伊拉克远征军 10-12 介入与 10-13 战斗；175 mm 炮击 Mazeh 机场）
  · events/october-14-1973-egyptian-armor-attack（六路 400–500 辆、埃损 150–250 辆、
    Yoel Gonen 旅独损 12 辆、Mamoun 崩溃）
  · events/operation-stouthearted-men（Abirei Lev：Matsmed/Deversoir、Luke 报告 750 人渡河、
    Gilowa 15 辆、舟桥 8 小时、滚轮桥待 10-19）
- 更新：wars/yom-kippur-war/index（南/北线/空中各节建链接、批次说明改写）、
  wars/yom-kippur-war/timeline（10-08/10-11/10-12/10-14/10-15/10-16 各条细化并加内链；
  删去重复的"基辛格抵莫斯科"一条；10-16 01:35 渡河加日期口径注）、根 index.md（来源㉓条补第 2 批）。
- 未建（按门槛暂缓，非遗漏）：Chinese Farm 独立页（ch30 只读首尾，下一批细读后建）、
  破出与第三军团合围（ch33–34 段）、苏伊士城（ch35）、核警报（ch37）、美苏空运（ch26）、
  338 决议（ch35）、Agranat（ch38 已读可建）、伊拉克远征军（暂并入戈兰反攻页）、
  全部人物页与装备页（本批不出独立实体页，凡涉及人名/型号只在事件页内叙述）。
- 异常／甄别：个别日期本书只给星期，已按 10-06=周六换算并在页内注明；叙军 1,400/720/800 辆、
  埃军 400–500 与 150–250 辆等数字均标"据本书／以方估计"；地图页文字层仍不可用（未从图取名）。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 304（+9）；新页 newpages-check CLEAN、
  glitch-scan 仅报专名/型号英文；无乱码字符、无问号占位、无占位符、无多余代码围栏；
  wikilink 全解析（根 index 的 [[log.md]] 为既有约定例外）。

### 2026-10-22（十月战争线·第 3 批：Chinese Farm、西岸破出、空运、海战、渡河决策）
- 来源同批 1（yom-kippur-war-rabinovich，sha256 5a434a19…），无新增原始资料。
- 本批读章：ch27（海战与埃方决策段）、ch28（渡河决策全章）、ch30、ch31（Chinese Farm 与桥）、
  ch32、ch33（破出与伏击）、ch34（Tirtur 夜袭与滚轮桥）、ch37 首段（10-18—19 农场陷落）。
- 新建（5 页）：
  · events/chinese-farm-battle-1973（走廊之战：Reshef 旅 97 辆损 56、亡 128；Morag 营单骑贯穿 Tirtur；
    第 890 伞兵营夜袭 41 亡百余人伤；10-18 农场陷落，场上埃军 118 辆毁＋15 辆弃、以军 56 辆毁）
  · events/operation-abirei-lev（10-17 苦湖北端伏击歼埃第 25 装甲旅 50–60 辆；10-18 空军打 Tsach 开路、
    Adan 师西进 22 英里至 Geneifa；10-19 Reshef 旅攻补给中心；至此合围第三军团）
  · events/us-soviet-airlift-1973（苏空运 10-10 起；美方 10-13 决定军机直飞、亚速尔中转；
    尼克松"不能让以色列输"；苏 7 个空降师戒备；美援起始日两说并存不代择一）
  · events/yom-kippur-1973-naval-war（拉塔基亚导弹艇对决、Styx 射程两倍下靠干扰取胜、
    埃叙舰队此后不再出港；Ras Arib 19 艘渔船、Ardaka 蛙人炸艇、曼德海峡被封锁）
  · events/decision-to-cross-1973-10-12（Gonen 被 Bar-Lev 架空；10-12 内层内阁"先等埃军装甲进攻"；
    Zamir 当场所收伞兵电报；同日开罗因阿萨德求援被迫把进攻定于 10-14）
- 更新：战争索引（南线/决策/海上/超级大国各节建链接，批次说明）、
  主时间线（10-06 增海战条、10-10/10-12/10-16/10-17 细化并加内链）、根 index.md（来源㉓条补第 3 批）。
- 未建（按门槛暂缓）：苏伊士城事件（ch35–36）、338 决议（ch35）、核警报（ch37）、Agranat（ch38）、
  伊拉克远征军独立页（仍并入戈兰反攻页）、places/ 与人物/装备实体页（本线仍未开，下一批起开）。
- 异常／甄别：美空运起始日 ch26 与 ch34 互相参差，已在页内并列标注；"Chinese Farm"名称由来
  本书未解释，未推考；埃军损失数字标为以方估计。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 309（+5）；新页 newpages-check CLEAN；
  无乱码／问号／占位符；wikilink 全解析；索引中一处换行导致的链接断裂已修复。

### 2026-10-22（十月战争线·第 4 批：停火外交＋赫尔蒙/Missouri＋停火后续战，并开概念与地点层）
- 来源同批 1（yom-kippur-war-rabinovich，sha256 5a434a19…），无新增原始资料。
- 本批读章：ch25 末（175 mm 炮与 Leja 段复核）、ch30 后段、ch31（埃方决策段）、ch32 起首、ch33、
  ch34（基辛格莫斯科行、赫尔蒙再夺、Missouri）、ch35（停火与续战全章）。
- 新建（7 页）：
  · events/un-security-council-resolution-338（10-19 夜萨达特转向：沙兹利请撤四旅被拒、
    "不撤回一个士兵"、致阿萨德函与无回信；约旦第 40 装甲旅入叙、Um Butna 打乱 10-19 反攻；
    基辛格—勃列日涅夫四小时谈成草案、12 小时生效、四个小时电报乱码；10-22 18:52 停火）
  · events/chermon-missouri-final-battles-1973-10（戈拉尼自西坡强攻赫尔蒙：亡 55 伤 79、
    两度攻山合计亡 80 伤 136；Nadel 伞兵空降叙方赫尔蒙 1 死 4 伤；Missouri 强攻 Raviv 旅损 22 辆）
  · events/ceasefire-violations-third-army-encirclement-1973-10（Shimshi 营被围一夜损 9 辆坦克 2 亡；
    10-23 达扬批准"自由行动"，Magen 师切断第三军团最后公路，围困约 3 万人；叙利亚 10-23 放弃大反攻）
  · concepts/israeli-intelligence-failure-1973（"概念"的判断内容、维持机制、外部情报失效、追责与作者判断）
  · concepts/yom-kippur-1973-equipment-comparison（坦克／反坦克／防空／渡河／海上对照，只收本书明确数值）
  · entities/places/golan-heights、entities/places/suez-canal-bar-lev-line（军事地理两页）
- 更新：战争索引（南／北／情报／超级大国／装备／地点各节建链接，批次说明）、
  主时间线（10-20 至 10-23 逐日细化并加内链）、根 index.md（来源㉓条补第 4 批）。
- 勘误/甄别：本书 ch25 记"175 mm 炮击 Mazeh 机场"与"拟炮击大马士革城区被叫停"，本批未改；
  停火时刻以 ch35 的 18:52 为准（另有"日落之后生效"的表述，两处并存于页内）；
  Scud 发射数三说并列（萨达特 2／沙兹利 3／以方 1）；埃军 10-14 损失、叙军坦克损失均标为以方估计。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 316（+7）；新页 newpages-check CLEAN；
  无乱码／问号／未配对的方头括号；wikilink 全解析。

### 2026-10-22（十月战争线·第 5 批：苏伊士城、核危机、脱离接触、Agranat、战果评价，并开人物层）
- 来源同批 1（yom-kippur-war-rabinovich，sha256 5a434a19…），无新增原始资料。
- 本批读章：ch36（苏伊士城全章）、ch37（核警报全章）、ch38（战后与结论全章）。
  至此 ch7—ch38 全部读完；仍未读 ch1、ch2、ch6（战前背景与消耗战）。
- 新建（9 页）：
  · events/suez-city-battle-1973（Zaken 坦克营 21 辆沿主干道"阅兵"式入城→第二个十字路口遭
    楼顶手榴弹与小巷 RPG 交叉火力；车长几乎全数中弹；Goldblatt 徒步重整；Yoffe 营困守警察局；
    Gonen 电台口述路线、Amit 中途停笔改向北走；铁路桥无守卫突围；以军亡 80 伤 120；
    Brik 最后一枪、Yaguri 营伤亡率 150%）
  · events/nuclear-alert-1973-10-24（勃列日涅夫信、23:41 DEFCON 3、八项具体措施时序、
    第六舰队 60 对苏 97 艘、Murphy 自估 40% 开战概率、政治局"不会发动第三次世界大战"、
    勃列日涅夫选择不回应、埃及 08:00 撤回求兵请求）
  · events/km-101-and-disengagement-1973-74（尼克松"最后通牒"两点、第三军团成为外交支点、
    10-28 01:30 km 101 帐篷握手、11-11 协议三点、日内瓦 12-21、埃以 1974-01-18、
    叙以 1974-06-05、萨达特私信）
  · events/agranat-commission-1973（Ashkenazi 独自举牌到 5,000 人、五人与六人的责任名单、
    梅厄与达扬免责理由、辞职链、埃拉扎尔/戈嫩/Zeira/Tal/Hofi 去向、作者对沙龙的定评、
    埃叙一侧的清算）
  · concepts/yom-kippur-1973-outcome-assessment（领土终局、装备损失、四组伤亡口径并列、
    "埃及赢了。以色列也赢了"、Starry 报告与美军装甲兵改革、空军地位反转与 1982 贝卡）
  · entities/people/{moshe-dayan,golda-meir,david-elazar,anwar-sadat}（人物层首批，只写本书内容）
- 更新：战争索引（新战役末尾与战后节、人物与地点建链、批次说明）、主时间线（10-24 细化、
  新增 10-25 与 10-27—28 两节、1973-11—1974 补 1974-02/1974-05—06）、根 index.md（第 5 批状态）。
- 甄别/口径：
  · Agranat"六人名单"含 Elazar、Zeira、Shalev、Bandman、Gedalia、Gonen（原文 "six heads"）；
  · Reshef 旅伤亡原书作 "more than goo"，按 300 记并标注 OCR；
  · 以方伤亡 2,656 死／7,250 伤为本书数；阿方两套口径（西方分析者 8,528／19,540 与以方估计
    15,000／35,000）并列，不加权、不相加；
  · 1974-05 叙以协议本书未给具体日期，时间线仍不写 05-31。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 325（+9）；新页 newpages-check CLEAN
  （人物页原有非 SCHEMA 键 role 已删）；log.md 尾随空格已清理。

### 2026-10-22（十月战争线·第 6 批：补读 ch1／ch2／ch3／ch6，建战前背景层）
- 来源同批 1（yom-kippur-war-rabinovich，sha256 5a434a19…），无新增原始资料。
- 本批读章：ch1（Footprints in the Sand，布达佩斯堡 Ashkenazi 线）、ch2（The Man in the Peasant Robe，
  萨达特 1970—1973 线）、ch3（Dovecote，教义与 Bar-Lev 线）、ch6（Summer Lull，欺骗与 D 日选择）。
  **至此 ch1—ch38 全部摄入完毕。**
- 新建（4 页）：
  · events/sadat-road-to-war-1970-73（1970-12 达扬 20 英里后撤建议被拒、1971-02 首次公开和平表态、
    Jarring 问卷、1971"决定性一年"、1972-07-08 驱逐苏联顾问与 Rafael 备忘录、1973-02 Hafez Ismail
    康涅狄格密谈、基辛格"事实是你被打败了"、萨达特人物刻画）
  · events/summer-lull-and-deception-1973（勃列日涅夫 6-23/24 深夜提案、达扬 5-21 与次月两次矛盾表态、
    Merrick 备忘录"五成以上"、Galili 两次提醒、1973-07 沙龙退役换戈嫩及其为人、埃及欺骗委员会与
    仅四人知情、Granite 2 演戏、阿萨德立场、约旦侯赛因、D 日选定的潮汐/犹太历/斋月逻辑与本书反驳）
  · concepts/idf-doctrine-and-bar-lev-line（六日战争前后教义未改、"敌人不得有收益"悖论、埃拉扎尔
    1971-01-01 推翻情报评估、1972 春"放五个师进西奈再关门"的思想实验与其后的"不会有战术后撤"、
    Bar-Lev 线实为 20—30 人小堡串、沙龙与 Tal 主张、沙龙离任时关闭 30 座中的 14 座）
  · entities/people/hafez-al-assad
- 更新：战争索引（新增"战前（1970—1973）"节、阿萨德建链、批次说明）、
  主时间线（新增"1970—1973（战前背景）"十二条，原"1973 年（战前）"改题"1973 年（临近战火）"）、
  根 index.md（第 6 批状态）。
- 甄别：ch1 的 OCR 与叙事未提供可核的堡名清单，本批不从地图文字层取地名；"Budapest 堡距运河 10 英里"、
  "52 人守军/其他数字"仍以既有 events/nafakh 等页所记为准，未在本批重写。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 329（+4）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK（无 U+FFFD、无字面问号、wikilink 全解析）。

### 2026-10-22（十月战争线·第 7 批：人物层第二批八页）
- 来源同批 1（yom-kippur-war-rabinovich，sha256 5a434a19…），无新增原始资料；本批为纵深人物页，
  全部取材于已读章节（ch3、ch6、ch8、ch10、ch19、ch21、ch30、ch35—ch38），未引入外部传记。
- 新建（8 页，均在 entities/people/）：
  · eli-zeira（"概念"的辩护者的自述逻辑、Shalev/Bandman 支持链、与 Tal 的正面冲突、
    赎罪日晨办公室三问、战后咨询业与"The Source 是双面间谍"之说）
  · shmuel-gonen（六日战争战功与恐吓式治军（一次处分 82 人、掷麦克风）、Adan"Gorodish 在 IDF 里没有位置"、
    1973-07 接任南部军区、10-10 被 Bar-Lev 架空的"平级调开"细节、战后丛林十三年）
  · haim-bar-lev（Bar-Lev 线起源、10-10 接管南线、与 Elazar 共同决定渡河时机、战后回内阁）
  · avraham-adan（战前对 Gonen 的判断、10-08 师损约 50 辆、渡河后的"阿丹的战争"、
    力主废止第一次停火、战后与 Ben-Gal 论"数量本身具有质量"）
  · ariel-sharon（1970 主张封塞堡垒、离任时关 14/30、10-10 抗命推进、渡河"领导但不是发起人"、
    Gilowa 主张事后可证有理、Missouri 争议被 Shazly 认可、战后告别讲话与委任被撤）
  · saad-el-shazly（1973-08-21 亚历山大港接叙方代表团、Granite 2 演戏与"I was sickened by the duplicity"、
    10-19 请撤四旅被拒、战后驻英大使/流亡/软禁）
  · avigdor-kahalani（10-07 拂晓 Hermonit 岭的开场，含"狮子准备进食"与 Killion 的对话）
  · zvika-greengold（Force Zvika、Tapline 与 Reshet 路夜战、与 Ben-Shoham 越野进抵 Nafakh 外围）
- 更新：战争索引人物节改为"已建页/尚无页"两段并全部建链、批次说明补第 7 批。
- 甄别：沙龙的"143/146 师"编号、Gonen 处分人数、Shazly 自传引文均照原书表述；本书未给的年份/职务
  一律不补（如 Bar-Lev 战后政治生涯、Kahalani 战后经历本页留空并注明）。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 337（+8）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK（无 U+FFFD、无字面问号、wikilink 全解析）。

### 2026-10-22（十月战争线·第 8 批：装备层九页）
- 来源同批 1（yom-kippur-war-rabinovich），另沿用 Price 卷III 既有 SA-6/SA-2 两页作对照；无新增原始资料。
- 新建（9 页，均在 entities/equipment/）：
  · at-3-sagger（3,000 码射程＝RPG 十倍、有线制导需全程压线、亮红尾焰、手提箱发射、
    每师 72 具、沙兹利"从后方抽调集中到突击部队"、战后坦克消亡论与"先开火远距离开火"教范）
  · rpg-7（射程为 Sagger 十分之一、300 码内仍能击穿、每师 535 具、被俘伞兵小队 13 具、
    Brik 首日衬衣着火、苏伊士城巷战、以军改用缴获 AK/RPG）
  · centurion-shot（高车体在起伏地形的反斜面优势 vs 苏式低矮车体俯角不足、射速与命中率、
    2,000—3,000 码交战距离、装甲兵占阵亡一半）
  · t-55、t-62（俯角缺点、T-62"和 T-55 一样脆弱"、三发命中才停一辆、数量本身具有质量）
  · gilowa-raft（10 分钟充气、15 辆并列 5 辆一筏每筏 1 辆坦克、沙龙主张与事后评价、
    舟桥 8 小时、滚轮桥待 Tirtur 打通、埃军渡河器材对照）
  · gabriel-missile（Styx 30 英里＝Gabriel 两倍、干扰＋高速接近破解、首次导弹艇对决）
  · sa-6-in-1973（导弹伞、Dougman 5 因无法定位 SAM-6 而失败、1982 贝卡 19 阵地毁 15 重创 3、82:1）
  · sa-7-strela-2（导弹伞组成、102 架损失中高炮与导弹各半、本书未给肩扛参数）
- 更新：战争线装备节重排为"综合对照／防空／装甲／反坦克／工程渡河／海上／飞机"七组并全部建链；
  装备对照页关联节改为型号专页清单。
- 甄别：新页只收本书明确数值（3,000 码、30 英里、72 具、535 具、10 分钟、15 辆/5 辆/1 辆、8 小时等），
  口径/装甲/射高等本书未给者一律留白并注明"本书未给"，未从其它来源补入。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 346（+9）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK。

### 2026-10-22（十月战争线·第 9 批：建制层九页）
- 来源同批 1（yom-kippur-war-rabinovich），无新增原始资料；全部取自已读章节。
- 新建（10 页，均在 entities/organizations/）：
  · egyptian-third-army（南段军团、司令 Wasel、每师 72 Sagger＋535 RPG＋57 炮＋90 无坐力炮；
    第 25 装甲旅 10-17 被歼；10-19 Wasel 电话称"技术困难"；3 万人被围；Nadeh 日记）
  · egyptian-second-army（中段军团、司令 Mamon 10-14 精神崩溃、第 21 装甲师、战后改任文职省长）
  · idf-7th-armored-brigade（177 对 1,400、土台反斜面、10-09 夺回 Hermonit、谷底 260 辆、
    叙军四天弃车逾 800 辆）
  · idf-188th-armored-brigade（南段、Ben-Shoham 与副旅长阵亡、Tamir 营 30 辆几乎全歼）
  · idf-sharon-division（143／146 两种编号并存照录、Reshef/Raviv/Mordecai 部、渡河与被牵制）
  · idf-162nd-division（Nir/Amir/Keren 旅、10-18 西进 22 英里、切断第三军团最后公路、苏伊士城）
  · idf-sinai-division（Mendler 师、Dovecote 的 300 辆坦克骨干、10-04 该日下午本应进阵地而 Gonen 推迟到 17:00）
  · idf-890th-paratroop-battalion（任务由苏伊士湾两栖突袭临改为 Refidim 空运；Chinese Farm 夜袭
    亡 41 伤逾百；战后士兵自认"彻底失败"）
  · syrian-7th-division（Abash 少将、北段主攻、战后一说阵亡一说病故）
  · iraqi-expeditional-golan-1973（10-12 介入、10-13 激战、10-23 反攻计划取消后回国）
- 更新：战争线"部队与组织"节重排为以／埃／叙／其他四组"已建页／尚无页"并全部建链。
- 甄别：沙龙师编号 143/146 在本书不同章节并存，照录不合并；890 营、第 25 旅等番号照原书；
  本书未给的伊拉克部队师旅番号与兵力、叙军第 46/51 旅以下编成，一律不补。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 356（+10）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK。

### 2026-10-22（十月战争线·第 10 批：人物层第三批十一页，人物层收官）
- 来源同批 1（yom-kippur-war-rabinovich），无新增原始资料。
- 新建（11 页，均在 entities/people/）：
  · benny-peled（埃拉扎尔的第一个电话、07:00 戈兰云底 240 m 报告、空军战后评价）
  · amnon-reshef（10-06 12:20 讨论仍是"雷谢夫旅应付渡河埃军"、Tasa 见敌机俯冲、
    Chinese Farm 与"全军伤亡最多的旅逾 300 人"、安息日威士忌段落、战后"佯攻开罗打第二军团"主张）
  · yitzhak-hofi（因表忧虑换来增援 vs 戈嫩接受"低概率"、经 Eitan 向 Ben-Gal 传警、
    战后摩萨德局长）
  · avigdor-ben-gal（"令人敬畏的存在"、孤儿出身/以军队为家、Yanush、10-06 10:00 集合营连长、
    战后论"数量本身具有质量"）
  · uri-ben-ari（Bar-Lev 到任对他是"恩典"、与 Gonen 共同主张先集结再进攻、为苏伊士城设"不得遇严重抵抗"前提）
  · yitzhak-ben-shoham（10-07 与 Greengold 越野进抵 Nafakh 外围、阵亡与电台误传、副旅长同役阵亡）
  · ahmed-ismail（1973-08-21 亚历山大港会谈、Granite 2 指令、拒撤第 25 旅恐重演 1967 溃逃、
    改令北上与第 21 师会合、沙兹利激烈反对）
  · ahmed-gamasy（潮汐与犹太历选定 D 日、主张"作战停顿"后打山口、10-19 反对撤军、
    km 101 主权与 11-11 签字）
  · saad-mamoun（10-01 才知 D 日、抗议并请辞被拒、10-14 精神崩溃细节与沙兹利推迟后送）
  · ahmed-wasel（10-19 凌晨 3 时电话"技术困难"、"那么这个旅就完了"与听天由命祷词）
  · zvi-zamir（10-06 凌晨"天黑前"99.9% 与接线员过节对话、"来源"36 小时前已发暗语、
    10-24 夜报告无苏军动向）
- 勘误：曾误建 entities/people/amnon-reshef-reshef.md（重复条目），已删除，无页面链向该路径。
- 更新：战争线人物节改为以／埃／叙／美苏四组"已建页／尚无页"，11 人均已建链；批次说明补第 10 批。
- 甄别：马蒙 10-14 崩溃细节取 ch32 原文（11 时"在休息"→下午军团部告以实情）；伊斯梅尔与加马西的
  职务区分照原书；凡本书未给的军衔/年份不补。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 367（+11）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK。

### 2026-10-22（十月战争线·第 11 批：飞机层六页＋地点层六页）
- 来源同批 1（yom-kippur-war-rabinovich），无新增原始资料。
- 新建（12 页）：
  · entities/equipment/f-4-phantom-ii（沙姆沙伊赫两架 Phantom 对 26 架 MiG、Dougman 5 出动 60 架损 6、102/277:6/432）
  · entities/equipment/a-4-skyhawk（Yadlin 首战盘旋、Ramat David 中队被有意排除在 Tagar 外以备戈兰）
  · entities/equipment/mirage-iiicj（9-13 海岸外 8:1 空战、打下的是 Kelt、司令部中队长临阵补位）
  · entities/equipment/mig-21、mig-25-recon（10-18 柯西金向萨达特展示 MiG-25 战场照片）
  · entities/equipment/tu-16-kelt（10-06 远海发射 Kelt、一枚被 Mirage 打落、一枚落海）
  · entities/places/chinese-farm（水渠/堤埂/涵洞与抽水站地形、Tirtur 与 Lexicon 两路、Missouri 位置关系）
  · entities/places/deversoir（大苦湖北口、Matsmed 并用、两军团结合部、三词互指不细分）
  · entities/places/nafakh（指挥+后勤同址的风险、围栏外叙军射击、Ben-Shoham 与 Greengold 越野进抵）
  · entities/places/kuneitra（城与"缺口"分列、1974 撤出废墟 Kuneitra、叙方留作纪念碑）
  · entities/places/mount-hermon（以色列赫尔蒙/叙利亚赫尔蒙/山脊三义分列、55 人守军 13 死 31 俘、
    戈拉尼旅亡 55 伤 79、两度攻山亡 80 伤 136）
  · entities/places/ismailiya（第二军团司令部、马蒙崩溃现场、甜水运河与两座桥、Yoffe 营过铁路桥）
- 更新：战争线装备节"飞机"组与地点节全部建链，批次说明补第 11 批。
- 甄别：全部新页只取本书叙述，地图地名一律不从 OCR 文字层取名；性能参数（速度/雷达/射程）本书未给，
  逐页注明不补。赫尔蒙三义、库奈特拉城/缺口两义显式分列，避免混写。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 379（+12）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK。

### 2026-10-22（十月战争线·第 12 批：超级大国层六页＋埃及层三页＋地名汇总三页）
- 来源同批 1（yom-kippur-war-rabinovich），无新增原始资料。
- 新建（12 页）：
  · henry-kissinger（1973-02 康涅狄格密谈、"事实是你被打败了"、卫星照片"先削弱萨达特的手"、
    "摧毁第三军团是不存在的选项"、10-27 期限、DEFCON 3 主持、"quasi-victorious, not triumphant"）
  · richard-nixon（圣克利门蒂深夜会谈、核危机中睡过全程、次日的强硬记者会与基辛格皱眉、
    第三军团存续＝美国义务）
  · leonid-brezhnev（6-24 深夜提案、10-16 "提醒他，开罗离运河不远"、"他落得这个下场是活该"、
    10-19 凌晨 4 时被叫醒、"让他冷静一下"的不回应）
  · alexei-kosygin（10-16 取消会见丹麦首相、三天谈判、每周千辆坦克的补给限度与埃方已损 600 辆、
    10-18 摊开 MiG-25 照片、"这不理智"）
  · andrei-gromyko（10-16 的"阿拉伯人会被打败、萨达特会被赶下台"判断）
  · anatoly-dobrynin（10-24 21:35 电话口读信件、05:40 递交复信）
  · hosni-mubarak、hafez-ismail、ismail-fahmy（三者的会议／渠道／不请自来三处记载，
    并在页首显式区分 Ahmed Ismail／Hafez Ismail／Ismail Fahmy 三人）
  · entities/places/suez-city（26 万人口、消耗战搬空、主街双车道加铁轨、Adabiya 港、
    "不据 Gonen 口述路线重建街巷图"）
  · entities/places/golan-battlefield-sites（Hermonit 岭土台、Tel Saki、Ramat Magshimim、Reshet/Tapline/Yehudia 路）
  · entities/places/sinai-battlefield-sites（大苦湖北口、米特拉／吉迪山口、Refidim、Tasa、Um Butna、Adabiya）
- 更新：战争线人物节（美苏由"尚无页"改为"已建页"、埃及三页建链）、地点节改为三张汇总页、批次说明补第 12 批。
- 甄别：埃及三个"伊斯梅尔"姓名极易混，逐页页首加区分说明；地名汇总页明确不从地图 OCR 取点名，
  Gonen 口述路线不作为街巷图依据。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 391（+12）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK。

### 2026-10-22（十月战争线·第 13 批：新来源㉔ Herzog《The Arab-Israeli Wars》，摄入 Book V）
- 新来源：Chaim Herzog《The Arab-Israeli Wars》(Arms & Armour 1982／Vintage 1984)，440 页 IA 扫描、
  pdftotext 未 OCR；sha256 79cea61f…。原始 PDF 与全文/分页文本存 raw/papers/arab-israeli-wars-herzog/。
  本书覆盖 1948—1982 七段战争，**本轮只摄入 Book V（1973）**；Book I—IV、VI、VII 未读。
- 新建（10 页）：
  · sources/arab-israeli-wars-herzog（结构、页码表、OCR 质量与系统性误拼、双主源用法）
  · concepts/yom-kippur-1973-egyptian-orbat-herzog（80 万兵/2,200 坦克/150 阵地/50 沿运河；
    第二军团 18·2·16 师、第三军团 7·19 师；10 座桥、每师 4—5 英里正面、首波 8,000 人、
    首分钟 10,500 发、渡河仅 208 阵亡；与 Rabinovich ORBAT 差异表）
  · events/bar-lev-forts-defense-1973（16 堡 436 人、Budapest 18 人与 16+16 辆敌装甲被毁 15 辆、
    Quay 堡七日守至 10-13 举托拉经卷投降、Ketuba 堡 Or-Lev、作者"折中产物"之评）
  · events/idf-counterattack-1973-10-08-herzog（Elazar 计划原文、轴线偏东致自东向西撞进埃军、
    Amir 12 辆/Nir 18 辆被毁撤出仅 4 辆、Sharon 一天南北空跑、与 Rabinovich 因果链并列）
  · events/crossing-and-corridor-herzog（以军西岸道路代号 Test/Havit/Vadaut/Sakranut/Vitamin/Asor/Sarag/Akal
    与六高地代号；钻进埃第 16 师后勤区；Matt 01:35 渡河与"院子"；Dayan"我们试过了"与 Gonen 回答；
    第 25 装甲旅 96/86；预制桥 190 码 12 辆坦克拖行、架桥亡 100 人）
  · events/northern-front-herzog-1973（叙军 1,500 辆、三步兵师＋两装甲师编成与师长名；188 旅 57 辆对 600 辆；
    Force Zwicka 挡第 90 装甲旅 20 小时；Yossi 蜜月归队 13 辆伤车；眼泪谷 500 辆；
    Tel Shams 三次失败与 'Yoni' 救人；伊拉克 3 装甲师与 Laner 的"盒子"80 辆；约旦 40 旅 28 辆；
    重夺赫尔蒙 8,200 英尺、Golani 亡 51 伤 100；北线总账 772 死/2,453 伤/65 俘）
  · events/air-naval-war-herzog-1973（SAM 射程 55,000/33,000/24,000 码与 150 阵地/50 沿运河；
    空战 334:5、阿方 514 架含 58 架自伤；Kelt 25 发 20 被击落；拉塔基亚 25 分钟、达米埃塔 40 分钟、
    Ras Ghareb 19 艘渔船、以海军亡 3 伤 24）
  · concepts/yom-kippur-1973-herzog-assessment（"军事胜利属于以色列、政治收益属埃及与美国"；
    苏伊士战线战略转变源于北线决定；与 Rabinovich 评价并列对照表）
  · entities/people/motti-ashkenazi（两书合并：战前哨所/脚印、布达佩斯堡、战后举牌到 5,000 人）
- 更新：战争线索引新增"第二来源：Herzog 的平行叙述"节并改主要来源；主时间线三处加〔据 Herzog〕数字；
  根 index.md 新增来源㉔与战争入口标注、修掉 [[log.md]] 断链。
- 甄别：两书冲突数字（Budapest 守军 18 vs 55、空战 334:5 vs 277:6、第 25 旅 96 vs 50—60、
  赫尔蒙守军 1+13 vs 55、Golani 伤亡、叙军坦克 1,500 vs 1,400）**全部并列并标明出处，未合并、未取中**；
  地图页 OCR 不可判读，一律不从地图文字层取地名；本书无脚注，引用以"小节＋PDF 页"标注。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 400（+10）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK。

### 2026-10-22（Herzog 摄入·第 2 批：BOOK II 1956 西奈战役——新开战争线 wars/sinai-campaign-1956）
- 来源同批 13（Herzog《The Arab-Israeli Wars》sha256 79cea61f…）；本批读 Book II（PDF 页 128—165，38 页）。
- 新建 11 页（**全部标"单源未校"**——本战争线目前只有 Herzog 一个来源）：
  · wars/sinai-campaign-1956/index（缘起：1951-07 阿卜杜拉被刺、1952 自由军官政变、1955 捷克斯洛伐克军售
    530 装甲车/500 炮/200 机、Ras Nasrani 封锁蒂朗、1956-07-26 运河国有化、塞夫勒密谋三段式保险设计；
    兵力对比表；政治结局与 UNEF；利德尔·哈特"一件艺术品"之评）
  · wars/sinai-campaign-1956/timeline（10-29 至 11-07 逐日，含 15:00 P-51 割电话线与 17:00 空降）
  · events/mitla-pass-battle-1956（395 人空降、P-51 十二英尺割线、沙龙旅 65 英里穿越、
    Themed 13 辆坦克只剩 2 辆、Nakhle、Gur 少校山口七小时战、亡 38 伤 120 对埃军约 200、
    达扬指控沙龙以"巡逻"之名打"战斗"为 subterfuge）
  · events/abu-ageila-battle-1956（"刺猬"三道沙脊、Adan 中校受挫于 Archer、Daika 山口迂回切断补给、
    Ruefa 水坝夜战每一辆坦克被命中、第 10 与第 37 旅失败与 Galinka 阵亡、本书的三项归因）
  · events/rafah-gaza-battles-1956（Golani＋第 27 装甲旅、半履带触雷成"静止燃烧靶"、17 门反坦克炮被火箭筒
    逐一击毁、达扬"俄国电影式拥抱"、阿里什军医院与通信兵之死、385 辆缴获、加沙 1 万守军与 Ali Montar 一战对比）
  · events/sharm-el-sheikh-and-tiran-1956（第 9 旅 200 辆/1800 人 150 英里驼道、Wadi Zaala 推车、
    Wadi Kid 两码宽、Ras Nasrani 空要塞、91 营夜攻失利与"电话线原封未动"的细节、09:30 海峡打开）
  · events/suez-intervention-anglo-french-1956（英法 11-01 才起航、只炸机场不支援以军、
    两次否决安理会停火、舰炮口径受限、11-06 登陆与英政府在压力下让步）
  · concepts/sinai-campaign-1956-strategy、concepts/unef-1956、entities/people/rafael-eitan
- 更新：根 index.md 新增 1956 战争入口与来源㉔条目改写（Book II 已完成，余 Book I/III/IV/VI/VII）。
- 甄别：本书对英法行动叙述简略且明显以色列视角（"英法空军从未支援以军""英国政府让步"），
  页面已在该处显式标出立场；UNEF 页并存本书内部两种表述（十年有效 vs 加沙被逼退）不调和；
  未从地图 OCR 取任何地名；本书页码与页眉混入正文处按上下文剥离。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 410（+11）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK。

### 2026-10-22（Herzog 摄入·第 3 批：BOOK III 1967 六日战争——新开战争线 wars/six-day-war-1967）
- 来源同批 13（Herzog sha256 79cea61f…）；本批读 Book III（PDF 页 166—215，50 页）。
- 新建 10 页（全部"单源未校"）：
  · wars/six-day-war-1967/index（1967-05 危机链：苏联"11 个旅"情报、吴丹撤 UNEF、关闭蒂朗、
    法国背身、拉宾 48 小时失能、全国团结政府、侯赛因"买保险"、纳赛尔三重误算；空袭首日数字；
    三战场导览；总损失表 764/338/141/285/6,000+/15,000 vs 10,000/800 辆坦克；1967-06-19 内阁决议；
    对纳赛尔的四点批评；军官军士占伤亡 23%）
  · wars/six-day-war-1967/timeline（4-07 至 6-10 逐日，含 07:45、08:00、16:00、20:00 等时刻）
  · events/six-day-war-sinai-1967（双方完整 ORBAT 表含师长姓名；Force Shazli；"公开调动"欺骗；
    El Jiradi 数度易手；Um-Katef 直升机机降＋背后夹击"史上最复杂战斗"；Yoffe 9 小时 35 英里沙丘；
    Shadmi 九辆坦克（四辆被拖）封米特拉；混入埃军纵队全歼一营；埃第 125 装甲旅完好遗弃与旅长答词；
    3,000 码六小时对射；加沙第三天凌晨；沙姆沙伊赫"封锁并不存在"）
  · events/six-day-war-jordan-jerusalem-1967（约军 8 步兵旅＋2 装甲旅；艾希科尔经 Odd Bull 传话；
    Ben-Ari 十九条年后重攻 Radar Hill；拉特伦首次得手；弹药山四小时；08:30 三营攻；10:00 西墙；
    Khatib 向本书作者陈述；纳布卢斯市民误迎；三桥尽控；约方 6,000+ 与以方 285）
  · events/six-day-war-golan-1967（1,500—2,500 英尺断崖、Tel Abu Nida 3,600 英尺；叙 8 旅＋2 装甲＋2 机步；
    Tel Fakher 白刃战"仅三人未伤"、以身搭桥过铁丝网；推土机全部被击中；Mandler 单轴强攻；
    14:00 未战占 Kuneitra；Peled 南段直升机跳跃）
  · events/six-day-war-air-strike-1967（Hod 其人：非 RAF 出身、捷克首批飞行员；309/340 机型明细；
    约叙伊连锁；416 架含 393 架地面；58 架空战）
  · events/uss-liberty-incident-1967（34 死 164 伤；本书"美方未通报"的归责，**显式标注为以色列官方立场**，
    不代替美方说法，未写入本书以外的调查结论）
  · concepts/six-day-war-outcome-1967（纵深首次获得；四个成功要素；"把缺陷扫到地毯下→影响 1973"；
    纳赛尔四点批评；1967-06-19 归还西奈与戈兰的内阁决议；波德戈尔内与喀土穆"三不"）
  · entities/people/mordechai-hod、entities/people/uzi-narkiss
- 更新：根 index.md 新增 1967 战争入口、来源㉔条目改写（Book II/III 已完成，余 I/IV/VI/VII）。
- 甄别：本书作 1967-06-05 约军开火时刻写作"1.00 hours"（排版/OCR 歧义），页面按上下文作"上午"并注明；
  1967 页与既有 1973 线的人物（Gonen/Sharon/Elazar/Narkiss/Hod）与 1973 线全部互链；
  地图页（西奈/西岸/戈兰各一张）文字层不可判读，未取任何地名。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 420（+10）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK。

### 2026-10-22（Herzog 摄入·第 4 批：BOOK IV 1967—70 消耗战——新开 wars/war-of-attrition-1969-70）
- 来源同批 13（Herzog sha256 79cea61f…）；本批读 Book IV（PDF 页 216—247，32 页）。
- 新建 9 页 + 改造 1 页既有页（全部"单源未校"）：
  · wars/war-of-attrition-1969-70/index（起点 1967-07-01 而非 1969；纳赛尔三阶段"防御性恢复→攻势防御→解放"；
    以军火炮劣势与"间接路线"；Eilat 号完整叙事；Bar-Lev 线完整决策史（Gavish 守水线→Adan 15 人 7 英里
    预警哨设计→沙龙/Tal 反对→Bar-Lev 裁定→1969-03-15 建成）；卡拉梅；242 决议两条原文直译；
    "飞行炮兵"；苏联 1970 年进驻的技术细节；纳赛尔"借停火前推导弹"与基辛格自认"我们最初犹豫鼓励了他"；
    停火后加固与 1972 折中"26 座中约 10 座封堵"→"概念模糊将在 1973 年头几小时索取代价"；
    总代价以方亡 500 余、伤 2,000）
  · wars/war-of-attrition-1969-70/timeline（1967-07-01 至 1970-09-28，只收书中带日期者）
  · events/war-of-attrition-egyptian-front-1967-70（分阶段叙事：堤道伏击/中线试探/攻势防御两次齐射/
    解放阶段总参谋长 Riadh 阵亡/苏联进驻后 3-5 月以方伤亡/停火后整备）
  · events/karameh-operation-1968（约军亡 40、PLO 约 200、以军亡 28 伤 69 与装备损失；后果链到黑九月）
  · events/israeli-deep-raids-1969-70（Sud 321 直升机 220 英里突袭、蛙人与 A-Dir 两栖装甲突袭 30 英里/
    12 哨所、绿岛、Shadwan 岛、Ras-Arab 吊运 7 吨 P-12 雷达、"飞行炮兵"决策与 1973 代价）
  · events/black-september-jordan-1970（本书只一段总结，未给伤亡数字，页内明示不补）
  · concepts/bar-lev-line-origins（与 Rabinovich 版逐项对照表：15 vs 20—30 人、7 英里、26/10 vs 30/14 座，
    不判断孰对）
  · concepts/soviet-air-defence-egypt-1970（SAM-2 土垒机动+齐射、60,000 英尺、SAM-3 四部双联 8 发斜距 18 英里、
    ZSU-23、20×45 英里"盒"与 18 英里椭圆区、"下一步是向运河跳跃推进"这一 1973 前兆）
  · concepts/resolution-242-1967（两条原则英文原文直译，标注本书未讨论定冠词争议）
  · events/eilat-sinking-1967（**既有 Price 线页**）：补 Herzog 节——HMS Zealous 1,710 吨、17:32、14.5 海里、
    三发时序、199 人中 47 死/90 伤、以及以军 10-25 轰击苏伊士炼油厂的报复；两书并列不合并。
- 更新：根 index.md 新增消耗战战争入口、来源㉔条目改写（Book II/III/IV 完成，余 I/VI/VII）。
- 甄别：本书对"五国介入黑九月"只有一段总结，页面明确标注未给伤亡/逐日；242 决议只引英文原文
  并声明本书未涉定冠词争议；Bar-Lev 线数字与 Rabinovich 冲突处一律并列表。
- 检查：SCHEMA.md sha256 191cd20f…（未变）；内容页 429（+9，另改造 Eilat 页）；新页 newpages-check CLEAN；
  whole-wiki QC 为 OK。

### 2026-10-22（Herzog 摄入·第 5 批：BOOK VI 1976 恩德培——不单开战争线，挂事件页）
- 来源同批 13（Herzog sha256 79cea61f…）；本批读 Book VI（PDF 页 348—359，12 页，全文无余）。
- **决策：恩德培不是战争，不建 wars/ 线**，直接建事件页＋政策页＋人物页，并在根 index 单列"反恐行动线"。
- 新建 4 页（"单源未校"，并**显式标注以色列官方视角**——作者 Herzog 时任以色列驻联合国代表，
  本书节录了他在安理会的辩护发言）：
  · events/entebbe-raid-1976（约 130 行，全书最详单页之一）：法航 139 的 4 劫机者（2 巴德-迈因霍夫＋2 PFLP）、
    256 乘客＋12 机组、53 名在押犯要求（以 40／西德 6／肯尼亚 5／瑞士 1／法国 1）、拉宾起初否定方案、
    佩雷斯坚持不屈服、Gur"除非我确信可行否则不建议"、**Shomron 06-28 无令自行规划**（"挑选"的联想）、
    07-01 17:00 总参陈述（"五成"与 100%/10 人伤亡的估计分歧）、为何只有周六夜、
    黑色奔驰＋两辆 Land Rover 的欺骗（源自空军训练乌干达时的家庭录像）、
    07-03 15:20 内阁讨论中授权 15:30 起飞、07-03 飞行 7 小时、暴雨后放晴看见着陆灯、
    鹅颈灯、100 码处两名乌干达哨兵、50 码处下车步行、"15 秒"击毙四名恐怖分子、
    Yoni 颈部中弹、第二架 7 分钟后落地、60 名乌干达兵自二楼逃走、击毙乌干达兵 35、
    13 名恐怖分子近距离击毙、15 名投降者被关、不在恩德培加油改内罗毕、
    **23:01 着陆／23:58 首机起飞＝57 分钟／42 分钟后末机离场并击毁 8 架 MiG**；
    评估段："短剑而非大锤"、"没有安全余量"、与 1980 年美国伊朗救援失败对照、
    **明确否认"乌干达与维多利亚湖有特工"的所有说法**。
  · concepts/israeli-counterterrorism-policy（佩雷斯四条政策宣示原文要点；1972 Sabena 97 人获救/2 枪手、
    1974-05 Maalot 22 名儿童、1978-03-13 滨海公路 30 余名乘客、苏黎世 Kloten；数字照录不校）
  · entities/people/dan-shomron（**跨 1956/1973/1976 三线**：1956 三路翻越山口、35 英里正面、六比一劣势；
    1973 西奈装甲旅、"全旅只剩 17 辆坦克仍于 14:00—午夜推进 30 英里"取 Adabiya；
    1976 恩德培指挥官；1982 段留待 Book VII）
  · entities/people/jonathan-netanyahu（1967 Tel Shams 夜救 Yossi 的 'Yoni'；1976 恩德培阵亡）
- 改造：events/six-day-war-golan-1967.md 新增"Tel Shams 与 'Yoni' 的夜救（10-12—13）"一节并互链；
  根 index.md 新增"反恐行动线"入口，来源㉔ 状态改为"Book VI 已摄入、余 Book I/VII"。
- 甄别：本书未给以方阵亡总数与人质死亡数，页面明示不补；Sabena 与 Maalot 的月份照录未校；
  Book VI 大量文字在扫描页边缘被截（如 "8 Ugandan Air Force MiGs" 处页码串入正文），已按语义复原并只在
  明显可疑处标注。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 433（+4）；新页 CLEAN；whole-wiki QC 为 OK。

### 2026-10-22（Herzog 摄入·第 6 批：BOOK VII 1982 黎巴嫩战争——新开 wars/lebanon-war-1982，15 页）
- 来源同批 13（Herzog sha256 79cea61f…）；本批读 Book VII 全文（PDF 页 340—379，含 Summary 与全书 Conclusion）。
- 新建 15 页（全部"单源未校"；**每页顶部标"以色列视角"**——作者为以色列前驻联合国代表，
  本书对沙龙/贝京政府多为辩护语调，但对萨布拉—夏蒂拉与凯汉委员会的追责结论照录）：
  · wars/lebanon-war-1982/index（约 190 行）：1981 扎赫勒—"法国室"—击落 Mi-8—SAM 前移的导火索链、
    1981-07-24 停火与其三种解释、停火期 240 余次行动、1982-06-03 Argov 遇刺（凶手属阿布·尼达尔系而非 PLO）、
    06-04 空袭、06-06 11:00 越界；40 公里（25 英里）目标；四条南北向地理带与 2,046/2,814/717 米高程；
    PLO 15,000 人／100 余辆 T-34／130-155 mm 炮／一次 40 发 Katyusha；叙军 30,000 人／200+100 辆坦克；
    以军八个师级集群；三路计划与"贝叙公路是战略钥匙"；Drori／Ben-Gal／Eli Geva 指挥；
    逐日主线；**损失对照表（以 480 死/2,600 伤/11 俘/50 坦克/1 Skyhawk+2 直升机；叙 370 死/1,000 伤/~250 俘/
    350-400 坦克/86 机/5 直升机/19 个 SAM 连；PLO 约 1,000 死/6,000 俘）**；
    "以色列史上第一次占尽优势开战"、"1982 年以军是迄今最好的一支"；以及本书**最重的一段自我批评**
    （若 PLO 撤离后即撤出贝鲁特，就不会与屠杀有任何关联；"咬下超过自己能咀嚼的量"）。
  · wars/lebanon-war-1982/timeline（1981 春—1983 年中，只收书中带日期者；明示本书成稿于 1983 年中、
    其后进展本书未述）
  · events/operation-peace-for-galilee-1982（06-06—06-14：Qasmiya 登陆、绕 Beaufort、Arnoun/Hardale 桥、
    Jezzine 首次遇叙军重兵、达穆尔 1976 年被屠的旧事、Ein Hilwe、平民撤离海滨的两次、"以军为避平民伤亡
    而使自己冒险"的作者承认）
  · events/beqaa-valley-sam-battle-1982（06-09 14:00：**19 个连全毁/4 个重创/以方零损失**；29:0 空战；
    第一周 86:0；Peled→Ivri 的十年准备；"两个技术体系而非飞机对导弹"；叙军"教条被摧毁"；
    以及以空军内部"不能据此评判俄制装备"的反省）
  · events/siege-of-west-beirut-1982（06-22 Aley-Bahmadoun 60 小时、以方亡 28 伤 168；断水断电的国内争议；
    08-04 有限进攻；08-12 11 小时空袭与里根电话、沙龙在内阁只剩一名部长支持；14,000 人撤离/8,000 人赴八国/
    Arafat 迁突尼斯；"咬下超过自己能咀嚼的量"）
  · events/sabra-shatilla-massacre-1982（**本书只有一句描述屠杀本身**："数百名手无寸铁的男女老幼"，
    无伤亡统计、无来源——页面已显式说明"须引第二来源"；但完整保留：09-15 协调入营、
    **内阁批准在长枪党入营之后才作出**、09-17 Drori 要求撤出、40 万人集会（占人口 10%）、
    凯汉委员会七人名单与三项建议、沙龙改任不管部长、Arens 接任）
  · events/israel-lebanon-agreement-1983（以方三项要求、放弃预警哨、Saad Haddad 争议、1983-05 协议要点、
    "钥匙在叙利亚手里"、阿萨德"不理解以色列政治的细微之处"的评语、Awali 河重部署的悖论、
    本书写作时的四点前景判断）
  · concepts/plo-in-lebanon（15,000 人编成与 7 个部署区、"国中之国"、一百多个从未遵守的协议、
    公寓地下室改弹药库与"活盾牌"的指控〔标为以色列视角〕、缴获可装备 5 个旅、Za'ater 之战损失为对以损失的六倍、
    "RPG 儿童"、1983 年法塔赫叛乱与 Sartawi 被刺）
  · concepts/lebanon-war-1982-assessment（本书列举的十项军事成就；"情报为何把 PLO 装备估少十倍"的未解之问；
    政治目标落空；最重的自我批评；拒绝下历史结论；全书 Conclusion 对以军/阿军的总评）
  · concepts/reagan-plan-1982（内容要点与四方反应；日期本书未给，页面标明）
  · entities/people/amir-drori（1973 Golani 旅长、重夺赫尔蒙山负重伤→1982 北方军区司令；09-17 要求长枪党撤出）
  · entities/people/david-ivri（1973 年 Peled 的副手→1982 空军司令→1983-04 副总参谋长）
  · entities/equipment/merkava（Tal 设计、"保险公司"昵称、生存力；**所有性能参数留白标"本书未给"**）
  · entities/equipment/t-72（9 辆被毁、"被击中即爆、乘员无逃出时间"、年产 3,000/驻东德 1,000）
  · entities/equipment/sa-5-1983（射程 300 km、覆盖特拉维夫/塞浦路斯东半部/安曼、苏军人员操作与围栏治外法权、
    苏方三重动机；与 1970 年埃及 SAM-3 部署对照）
- 改造 4 页既有页（**新来源触及既有实体 → 扩写而不另开页**）：
  · entities/people/ariel-sharon.md —— 新增 1982 节：国防部长、09-14 命令进西贝鲁特、09-15 协调长枪党入营、
    08-12 后被指越权且内阁只剩一人支持、凯汉建议辞职但改任不管部长；frontmatter 加 wars/sources。
  · entities/people/rafael-eitan.md —— 新增 1982 总参谋长节（纪律水准、"平静的信心"、与沙龙同开发布会）。
  · entities/people/avigdor-ben-gal.md —— 新增 1982 东段司令节（绕 Karoun 湖西岸击叙第 1 装甲师右后侧翼、
    全歼一个旅、叙损失约 150 辆、装甲营误入叙军村镇靠炮兵救出、停火线距叙边界 5 km）。
  · entities/people/dan-shomron.md —— 清除"待 Book VII 补"的占位，改为"本书未记其 1982 职务"（诚实留白）。
- 更新：根 index.md 新增黎巴嫩战争入口，来源㉔ 状态改为"**只剩 Book I（1948）尚未摄入**"。
- 修错：新建页与 amir-drori 中把既有页误写为 [[chermon-missouri-final-battles-1973]]（实际文件为
  ...-1973-10.md），已全库修正；equipment 页误加 SCHEMA 外字段 `category:`，已删。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 448（+15）；新页 CLEAN；whole-wiki QC 为 OK。

### 2026-10-22（Herzog 摄入·第 7 批：BOOK I 1948 独立战争——收官，新开 wars/war-of-independence-1948，20 页）
- 来源同批 13（Herzog sha256 79cea61f…）；本批读 Book I 全文（PDF 页 18—127，110 页，约 26.8 万字符，分 11 段读完）。
- 新建 20 页（全部"单源未校、以色列视角"；作者 1948 年任第 7 旅作战参谋/副旅长，多处为亲历证词，页内已标）：
  · wars/war-of-independence-1948/index（约 200 行）：英国托管末期的敌意与两万余人英属阿拉伯部队、
    Haganah 的武器清单（**步枪 10,500／冲锋枪 3,500／轻机枪 775／3 英寸迫击炮 34／2 英寸迫击炮 670，
    弹药仅够三天，重机枪反坦克炮火炮为零**）、65 万人口可动员 45,000 其中 30,000 只做地方防卫、
    阿拉伯联军编成与入侵分工、1948-05 以军九旅编成与"最重武器是 195 门 3 英寸迫击炮"、
    三阶段表、**阵亡 6,000（军人逾 4,000）＝人口 1%** 与作者的三重换算、两个各约 80 万难民问题框架。
  · wars/war-of-independence-1948/timeline（1947-11-29 至 1949-07-20，逐日只收书中带日期者）
  · events/：northern-front（加利利／Degania"IDF 第一门火炮上场"／Mishmar Hayarden／Sejera／Dekel／Brosh／Hiram 14 村至利塔尼）、
    jerusalem（Hadassah 车队亲历证词／Nebi Samuel 的时机失误／Kastel 与 Abd el Kader 之死／旧城 300 发子弹 36 人／
    1,190 平民捧经卷下山与 58 座会堂／Notre Dame 200 人近半伤亡与 Glubb 17:00 叫停）、
    latrun（四次进攻全记；**"计划很好，炮兵很好，装甲极佳，步兵可耻"**；缅甸路 06-10 通车与停火时限的因果）、
    southern-front（Kfar Darom 的 TNT 经匣袋、Yad Mordechai 180 人撤出与"争得五天"、Nitzanim、Negba 1,000 攻 140）、
    operation-danny（吕大 Dayan 第 89 营的"喧闹冲进又退出"、Glubb 不增援的辩护与"其实是对的"、Ibdis 18 人、Negba 200 伤亡）、
    operation-yoav（10-15 车队开火作为行动信号、Iraq El-Manshiyeh 仅 50 人回阵、Huleiqat 六山头与沙特兵咬人、
    贝尔谢巴 500 守军 09:00 投降、"山上的怪物"11-09 终被攻下、Taha Bey 与 Allon 的 Gat 会面）、
    operation-horev-and-uvda（Ruheiba 古道清沙、12-27 El Auja、入西奈与**英国最后通牒**、
    击落 5 架 Spitfire＋1 架 Tempest、Adan 挂手绘白旗抵 Um-Rashrash）、
    etzion-bloc（35 人 Palmach 排全灭、05-13 屠杀、作者对"守到最后一男一女"政策的成本核算）、
    altalena-affair（第 4 号命令 05-28、15 死、06-28 全军宣誓）、armistice-1949（四份协定与"六个月内签和约"的失效）
  · concepts/：haganah-palmach、plan-d-1948（**只写书中内容，并明示本书未涉 Plan D 文本争议与驱逐意图问题**）、
    arab-refugee-problem-1948（照录本书解释链＋引 Khaled al-Azm 与 Abu Mazer 两处阿拉伯文献原文，
    并列出"本书未处理"的四项留白）、arab-legion-1948（含对 Glubb 两次决策的辩护及"本书倾向"提示）、
    war-of-independence-assessment（Ben-Gurion 与丘吉尔/罗斯福/戴高乐并列等判断照录）
  · entities/people/：david-ben-gurion、yigal-allon、yigael-yadin、yitzhak-rabin、mordechai-makleff、
    moshe-carmel、shimon-avidan、haim-laskov、ezer-weizman、dov-joseph、david-marcus
- 改造 2 页既有页（跨卷同一人）：entities/people/david-elazar.md（补 1948 锡安山夜袭节＋frontmatter）、
  entities/people/uzi-narkiss.md（补 1948 锡安山佯攻节＋frontmatter）。
- 更新：根 index.md 新增独立战争入口，来源㉔ 状态改为"**七卷全部摄入完毕**"。
- 甄别（本批重点）：
  · Plan D：本书只当军事部署计划写，未引文本、未涉驱逐争议 → 页面明确声明"本书不足以支持任何一种判断"。
  · 难民问题：照录本书解释链与所引阿拉伯自认，同时列出四项"本书未处理"的留白，不代其补。
  · 日期：Etzion 首攻本书只写"1 月"→ frontmatter 用 1948-01 并在正文标"本书未给具体日"；
    Hiram 期间"21 日傍晚"与月份矛盾 → 页内标"本书此处日期有讹"，不作日期断言。
  · 我起草 timeline 时曾误插一条"04-25/26 德国札记本"（属 1973 卷 ch25 情节、与本卷无关），复核后已删除。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 448 → **476**（+28；本批新建 20 页，差额 8 页来自本轮补链与索引页计数口径校正，非重复建页）；
  新页 newpages-check CLEAN；whole-wiki QC 为 OK。

### 2026-10-22（Pollack 摄入·第 1 批：BOOK 全卷导论＋结论＋六国评估段——新建跨战争专题，19 页）
- 新来源㉕：Kenneth M. Pollack《Arabs at War: Military Effectiveness, 1948—1991》（Univ. of Nebraska Press 2004，
  Bison；EPUB 9,315,327 字节，sha256 111a4e23…）。
- 提取：EPUB 本地 zipfile 解包 XHTML→文本（无 OCR），全文 1,838,242 字符；按 split 文件切成
  seg-ch0_intro／ch1_egypt／ch2_iraq／ch3_jordan／ch4_libya／ch5_saudi／ch6_syria／concl，
  原文与分段文本存 raw/papers/arabs-at-war-pollack/。
- 本书性质（已在来源页与专题页显式声明）：**不是战史而是"军事效能"评估**，刻意压缩战役过程，
  故不能用于补战役细节；作者是美国防务分析者，写作目的之一是"为美国未来在中东的战争作准备"。
- 新建 19 页：
  · sources/arabs-at-war-pollack（书目、sha、提取方式、章节→split 映射、使用限制与常见 OCR 讹误清单）
  · topics/arab-military-effectiveness-pollack（跨战争专题入口：总诊断／四缺陷／六国表／战例／
    **已知数字冲突清单**／待建清单）
  · concepts/：arab-military-ineffectiveness-pollack（八种流行解释逐条检验＋四项常量缺陷＋
    "战术领导力最致命"）、military-effectiveness（定义与九个维度、须剥离的六个干扰变量）、
    unit-cohesion-question（Harkabi 说 vs Pollack 反驳的史学争论页）、arab-tactical-leadership、
    arab-information-management、arab-technical-skills、arab-maintenance-record
  · 国别：arab-legion-1948-pollack、jordan-1948-vs-1967-pollack（受控比较）、jordan-army-decline-pollack、
    syria-1948-galilee-pollack、syria-1973-golan-pollack、syria-1982-lebanon-pollack（含 Gabriel／
    Dupuy-Martell／Cordesman-Wagner 三方互斥评价并列）、iraq-1973-pollack、
    libya-military-effectiveness-pollack、saudi-military-effectiveness-pollack
  · events/was-al-khafji-1991（本库第一条海湾战争地面战页，也是少见的"阿拉伯军队对阿拉伯军队"战例）
- 更新既有页 6 处（新来源触及既有实体→扩写不另开页）：
  · events/operation-badr-1973 —— 新增"第二来源对照：Pollack"节（两军团编成与 14,000 人/200 辆加强步兵师、
  30 万人/2,400 坦克/2,300 门炮、435 架作战飞机、135 个 SA-2/3＋20—40 个 SA-6＋2,100 门高炮＋5,000 枚 SA-7、
  8,000 人首波、1 小时破堤、90,000 人/850 辆 18 小时、208 人、第三军团因"不得偏离计划"延迟 12 小时、
  以军 252 师两天损失 300 辆中的 200 辆）；并把"待建"链接改为实页。
  · events/october-14-1973-egyptian-armor-attack —— 新增 Pollack 的因果机制（Isma'il 'Ali 反对、
  萨达特因叙利亚求援压过其意见、Jebel Ataqah 技侦被毁、两个师变九处旅级攻击、步兵不下车、
  500 门炮"完全无效"、265 辆/不足 40 辆、10-17 第 25 旅 96 辆只剩 10 辆的另一口径、柯西金摊卫星照片）。
  · entities/organizations/iraqi-expeditionary-golan-1973 —— 补 Pollack 节与指向新概念页。
  · wars/yom-kippur-war/index —— 新增"第三来源：Pollack 的效能评估"节。
  · wars/{war-of-independence-1948,six-day-war-1967,lebanon-war-1982}/index —— 各加"效能视角（第二来源）"一行。
  · wars/gulf-war/index —— 战役清单加入海夫吉之战。
  · 根 index.md —— 新增跨战争专题入口与来源㉕条目。
- 甄别要点：
  · **数字冲突一律并列**（戈兰 10/8/10 vs 10/12/20；第 25 装甲旅 86 辆 vs 96 中只剩 10 辆；
    1982 贝卡 SAM 19+4 vs 17+12），已在专题页汇总成清单，不择优、不合并。
  · EPUB 为扫描件 OCR，存在系统性数字讹误（1g6o=1960s、i99i=1991、io,ooo=10,000、Soo=500、
    M-log=M109、ARCS=APC），凡数字与型号均回查上下文合理区间，不可判读者不写。
  · 本书"我们只写书中所述"——埃及国别总页、两伊战争、库尔德战争、利美冲突、乍得战役页均**未建**，
    已在专题页列入"待建"清单。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 476 → 495（+19）；newpages-check CLEAN（已删非 SCHEMA
  字段 `language:`）；whole-wiki QC 为 OK（期间修正 jordan 页一处字面问号为〔问号〕）。

### 2026-10-22（Pollack 摄入·第 2 批：第 1 章《埃及》1948—1967——国别总页，3 页）
- 来源同批 21（Pollack sha256 111a4e23…）；本批精读 seg-ch1_egypt 的 1948 战役＋效能评估、1952 建设、
  捷克军售、1956 战役＋评估、也门 1962—67、1967 战役＋评估＋"以空军作用"节。
- 新建 3 页：
  · concepts/egypt-military-effectiveness-pollack（国别总页，约 190 行）：**贯穿全期的能力曲线**
    （战术层 44 年几乎不变／战略层起伏），1948（40,000 人上限原因、5 个步兵营＋16 门 25 磅炮编成、
    Haganah 22,000 支步枪的对照、Asluj 两天不动、Mwawi 的三次收拢与"行军慢不是他的选择"）、
    1952 后建设（上校以上全部清洗、'Amr 的悖论、国防开支 3.9%→8.4%、80 名前国防军军官与 Frambecher）、
    1956（捷克军售完整清单、**主力被放在三角洲防英军、西奈只有 9 万中的 3 万**、Frambecher 方案 vs 实际部署、
    Adan 支队与两次"不敢冲锋只敢开火"的埃军反击、Umm Qatef 战至 11-01 总退却、
    **4 装甲师两天走不到 90 公里 vs 沙龙一天 150 公里**、坦克当活动碉堡、开战仅一半苏制坦克可用、
    西奈无一座维修工场、六名 Il-28 飞行员只有一人找到以色列）、也门、1967（7 个师 950 辆坦克的编成、
    第 7 旅 201 人伤亡中 153 人在 06-05、达扬"他们没有逃走"、撤退瓦解的真正触发点、
    第 4 装甲师 vs 第 125 旅的对照、Sharon"他们的军官是狗屎"、5% 地雷未解除保险、
    驳"Qahir 计划更好"、"他们大概有最好的战略，只是执行得很糟"、'Amr 的微观干预与 Shazli 不动、
    Murtagi 前线司令部被完全绕过、6 月 6 日总退却"决定对、方式不可原谅"）
  · concepts/six-day-war-air-power-debate（史学争论页：架次 268/614/652、对西奈 170/286/321、
    06-05 击毁 12—15 辆、美国调查组 8% 命中/2—3% 击毁、以方调查 15%、
    以及 Pollack 承认的"反航空兵作战近乎完美"与反事实推演；与 Herzog 页并列不冲突）
  · events/egypt-in-yemen-1962-67（本库第一次触及也门：7 万人五年、'Amr 的 Ramadan 攻势与 Murtagi 诸役
    "出色的常规作战"、但"从未弄明白怎么打游击队"、双重归因、与越南的类比；
    **明示本库尚未建 yemen 战争线**，暂只在专题与埃及页挂链）
- 更新 4 处：wars/{six-day-war-1967,sinai-campaign-1956,war-of-independence-1948}/index 各加"效能视角"行；
  topics/arab-military-effectiveness-pollack 的埃及行改为实链并把埃及从"待建"清单移除。
- 甄别：1948 年埃及兵力本书作"从未超过 40,000、初期 1 万"，与 Herzog 的"5,000 人远征军"口径不同，
  已在两页各自标明；1956 年本书对 Mwawi/纳赛尔的战略评价与埃及自我归因相反，按"本书判断"标注。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 495 → 498（+3）；whole-wiki QC 为 OK。

### 2026-10-22（Pollack 摄入·第 3 批：第 1 章《埃及》剩余——消耗战评估、1973 战前改造、1977 对利、1991，3 页）
- 来源同批 21；本批读 seg-ch1_egypt 的消耗战效能评估、1973 人事与战前准备（Egyptian Planning＋
  Rebuilding the Egyptian Military＋The Soviet Role）、1977 对利比亚边界战争、1991 海湾各节。
- 新建 3 页：
  · concepts/egypt-1973-preparation-pollack（约 130 行）：萨达特的人事（Isma'il 'Ali／Shazli／Gamasy／Mubarak，
    **本书对 Shazli 履历的负面评价**：1948 投降、1956 先撤、也门不佳、1967 最早逃离西奈）；
    "先评估自己再设计战争"（研究以军公开访谈、鼓励学希伯来语、认定以方弱点为怕伤亡／动员不耐／过度自信、
    自认强项是步兵与固定防御）；**"文化性毛病不能改只能绕"→ Jebel Ataqah 技侦站**（截收以军明语战报）；
    High Minarets 只做第一阶段（"运河加西奈十厘米"）；战略进攻＋战术防御；**整场攻势演练 35 次**、
    一人一任务、模型训练、80 个工兵单位两年每天两次破堤；1968 年起反复演习、1973 年 1—10 月 22 次；
    "只撤回一部分人"的集结伪装；**军官大学学历 2%→60%、士兵高中 25%→51%、全国一半工程师在军中**；
    机堡；官兵裂痕的修补与"鼓励为任务承担伤亡"；苏联角色与**1972 年"赶走苏联人"的真相**
    （留下技术／电子战／雷达人员，赶走作战顾问与作战部队）。
  · concepts/egypt-1991-gulf-war-pollack：1973 后的"社会福利化"与人员退化、美械化与政治化回潮；
    JFC-N 编成（第 3 机械化师、第 4 装甲师、第 20 突击团、空降旅，4 万人／400 辆）与"美方把第 1 骑兵师
    留作救火队"；**拒绝提前发起、火壕前等十小时、按已废弃目标的火力计划开炮、以"弹药配额用完"拒绝反炮兵、
    不获正式命令不改计划、无命令不进科威特城**；总评"十五年美援几乎没改善效能"。
  · events/egypt-libya-border-war-1977（两章合并叙述）：1976 年"未打之仗"（美方判断埃及因未准备而止步）、
    1977-07-21 as-Sallum 伏击与第 9 坦克营损失 50%、al-Adam 空袭两次都打砸、
    **07-24 萨达特在本可扩大战果时突然停火＝美国强力阻止**（怕埃及 1,000 公里推进失败动摇萨达特）、
    双方损失表（利 10—20 架 Mirage／30 坦克／30 装甲车／400 人伤亡；埃 ≤4 架／约 100 人）。
- 更新：concepts/egypt-military-effectiveness-pollack 补"消耗战评估"整节（10:1 空战损失比、
  每年只能培养 30 名飞行员、6—10 发 SA-2 才五成、65—80% 的 Bar-Lev 摧毁误判、飞行员静坐抗议、
  "不优雅但有效"的总评）与两处指向新页的段落；
  topics 页补战例入口与"战前改造／1991"两条；1973 索引与 gulf-war 索引各加链接。
- 甄别：1977 年战线本库尚无 `wars/egypt-libya-1977/`，页面明示"暂挂 war 字段、只在专题与国别页挂链"，
  不预置断链；埃及 1973 兵力／损失口径与 Rabinovich、Herzog 的差异仍按既有对照节标注，不合并。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 498 → 501（+3）；whole-wiki QC 为 OK。

### 2026-10-22（Pollack 摄入·第 4 批：第 2 章《伊拉克》1948＋库尔德战争＋1967／1973 教义，3 页）
- 来源同批 21；本批读 seg-ch2_iraq 的 1948 战役评估、1958 政变与建军、第一次库尔德战争全段
  （Qasim 的"饿死"战略、1963／1965／1966／1969 四次攻势与 Mt. Handrin 惨败）、
  1961—70 效能总评、第二次库尔德战争 1974—75（含 1975-03-06 阿尔及尔协议）、1967 年的缺席、
  1973 远征军的后勤与教义（集中兵力、火力至上）。
- 新建 3 页：
  · events/kurdish-wars-1961-75（约 105 行）：本书最完整的一条"本可打赢却打输"论证——
    库尔德人是"很差的叛乱方"（只会伏击与脱离、步枪不够人手、无重武器至 1969、射手差、Barzani 不是好将军），
    地形亦不利叛乱方，"土耳其与伊朗都反复粉碎过本国库尔德叛乱"；
    伊拉克战略层只检讨过两次，1965—66 就找对了答案（切断经伊朗的补给线），
    但**战术层无能**（不离公路、不设警戒、不巡逻、占低地、不能合成兵种、正面强攻、空军只炸村）；
    1974—75 反过来证明这一点：改"蚕食＋火力"、修 700 英里公路、焦土，加上
    **库尔德人自己改成死守硬拼**（原话：their tactics were hardly elegant, but with the cooperation of the Peshmerga they got the job done），遂胜；
    本书明言 1975 年协议数小时内伊朗即收回库尔德人的重武器，次日伊军进攻，04-02 封闭边界。
  · concepts/iraq-1948-pollack：兵力规模（一个师级部队跨 1,000 公里沙漠维持）、Mahmud 平庸但不全责、
    士兵不会用枪／纪律差／（除 ALA 志愿人员）缺投入、**初级军官不主动无想象力**＝战术失败主因、
    装甲车连屡因指挥官动作慢而晚到、遇问题只照原计划硬走或等上级；
    唯一可赞：凝聚力（Zefat、Katamon 山脊）与"至少够用"的后勤（弹药汽油大手大脚＝有余）。
  · concepts/iraq-doctrine-firepower：1967 缺席（第 3 装甲师在约旦东部未及展开、1/3 坦克不可用、
    Tu-16 找不到目标炸了农田、H-3 空战 21:≤3）、1973 远征军编成与精锐（Salah ad-Din）、
    **两大学习成果＝集中兵力＋火力至上**（后者直接带进 1980 年两伊战争），
    以及"尚未学到的部分"（10-12 两旅只用一旅、10-16 第 8 营不投入）。
- 更新：topics 页补库尔德战例入口与伊拉克三页索引；1948 索引加 iraq-1948 链接；
  1973 索引在伊拉克条后加"教义来源"链接；concepts/iraq-1973-pollack 增"教义来源"小节。
- 甄别：库尔德战争本库无 `wars/kurdish-wars-iraq/` 线，页面明示暂挂字段、不预置断链；
  全书对伊拉克 1948 年只有约两段，页面顶部明写"着墨远少于埃及与约旦"，不从 Herzog 补细节。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 501 → 504（+3）；whole-wiki QC 为 OK
  （初跑一条中文问句字面问号 → 改写为"—"后通过）。
- 断点：第 2 章余下＝两伊战争（1980—88）与 1991 年伊拉克部分；此后第 3 章约旦（1948—56 边境战、
  卡拉梅、黑九月）、第 4 章利比亚（乌干达、乍得）、第 6 章叙利亚（1976 侵黎）。

### 2026-10-22（Pollack 摄入·第 5 批：第 2 章《伊拉克》两伊战争 1980—88，2 页）
- 来源同批 21；本批读 seg-ch2_iraq 的 "The Iran-Iraq War, 1980-88" 全段（约 7.4 万字符）：
  1973—80 扩军与政治化、1980-09-22 先制空袭、入侵胡齐斯坦、1980-11—1982-05 伊朗四次反攻
  （Susangerd／Bostan／第二次 Dezful／Khorramshahr 收复）、"Explaining the Iraqi Defeat"、
  第一次巴士拉之战与伊拉克防御工程学、去政治化、伊朗的问题、
  "Resilient Iraqi Tactical Problems"、空战。
- 新建 2 页：
  · events/iran-iraq-war-1980-88-pollack（约 230 行）：本库**首次**触及两伊战争，但明示
    "不是通史、不评国内政治与化学武器的国际法层面（本书不足以支持判断）"。
    要点：照抄 1967 年却**完全无侦察**（靠伊朗逃亡军官、故意低估）、**不懂 HAB 机堡**、
    出动能力 40—70 架次／日而以色列用 700 架次一上午（"伊拉克人用 100 架次摊一整天"）、
    当日仅毁伊朗 2—3 架飞机、**次日即失去制空权**（伊朗出动 160 架次）；
    入侵计划是**1941 年英国一次参谋演习的仓促改写**（"一个英国师夺取胡齐斯坦"），
    两周只推进 20—65 公里、最快 5—6 公里／日；
    Khorramshahr 打了四周／8,000 伤亡／百余辆装甲，且**先抽走该装甲师的编内步兵**；
    坦克当活动炮台、行进间不能射击、Kharkeh 河被一个缺编坦克营挡住；
    伊朗四次反攻把伊军逐出胡齐斯坦（第 16 装甲师 300 辆损 200 辆，而伊军在完美陷阱下仍损 350 之近 100）；
    1982 后靠**筑垒（1987 年巴士拉六道同心圈）＋沙堤＋放水＋3,000 辆重装备运输车＋去政治化**守住；
    第 9 装甲师在第一次巴士拉之战后**被解散且再未重建**（全战争唯一）；
    本书的硬问题："问题不是伊拉克为什么能僵持，而是为什么这对它如此困难"；
    1983-10 就用化学战；战术层到战争结束未解决，高级军官只好把机动"提到战役层"自己指定反击路线。
  · concepts/iraq-depoliticization-1982：政治化清单（忠诚优先、频繁轮换、多套安全机构、微观管理、
    15 万人民军承担镇压）→ 1982 年**解职并处决 200—300 名**高级军官、召回数百名被退伍的能者、
    **撤销营以上政治军官**、停轮换、放开作战控制 → 点名七名浮出的将领
    （含 **Hisham Sabah al-Fakhri**，本书明说其表现"在整个战争中明显改善"，
    尽管他在 1982 年第二次 Dezful 曾"惊慌"）→ 改善停在战役层，战术层未动；
    本书因果排序＝政治→战役→战术。页内注明"政治干预才是主因"一句为**归纳而非原文直断**。
- 更新：topics 页国别表伊拉克行改写（1948／1973／教义／1982 去政治化），
  并新增"战例页"首条两伊战争（标注"本库唯一的两伊内容、非通史"）。
- 甄别：本书此处**内部日期不一致**（第一次巴士拉写"13-14 June"又写"July"），页面照录并标出；
  战争本库无 `wars/iran-iraq-war-1980-88/` 线，页面明示暂挂字段；
  伤亡、化学战使用规模等数字本书未系统给，页面不给总数。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 504 → 506（+2）；whole-wiki QC 为 OK。
- 断点：第 2 章余下＝1991 年（侵科、空袭战、共和国卫队、"Additional Observations"）；
  此后第 3 章约旦（1948—56 边境战、卡拉梅、黑九月）、第 4 章利比亚（乌干达、乍得）、
  第 6 章叙利亚（1976 侵黎）。

### 2026-10-22（Pollack 摄入·第 6 批：第 2 章《伊拉克》1991＋章末总评，3 页；伊拉克章完成）
- 来源同批 21；本批读 seg-ch2_iraq 的 "The Invasion of Kuwait"、"Iraqi Strategy for the War against
  the Coalition"、"The Air War"、"The Battle of Ras al-Khafji"、"The Iraqi Army on the Eve of the
  Ground War"、"The Ground War"、"The Stand of the Republican Guard"、"General Observations"、
  以及章末 "Iraqi Military Effectiveness, 1948-91"。
- 新建 3 页：
  · events/iraq-invasion-of-kuwait-1990：01:00 入侵；整个 RGFC（伊战后扩为 8 个师，新增 Tawakalnah
    机械化师与 Adnan 步兵师）；三条轴线＋特种部队师直升机机降夺机场与埃米尔宫；08:00 前控制首都；
    不到两天清剿完毕；空军"什么有价值的目标都没打中"且没拦截任何一架科威特飞机；
    **三个重装师约十小时 80 公里**、其后 24 小时再 75 公里；唯一计划错误＝两个重装师穿科威特城；
    与入侵伊朗的直接对比；机制＝提前数月计划＋只用 RGFC＋反复演练＋严格按书本。
  · concepts/iraq-1991-coalition-war-pollack（约 175 行）：赌美国不愿流血的战略、空袭预计 3—7 天；
    战斗机"捡漏"／SAM 与 7,500 门高炮担纲；Kari 网两天关停→拦阻射击退化→"投完弹才开火"；
    10,000 英尺以上使高炮失效；F-4G＋HARM 到第三天逼得 SAM 拒开机；GWAPS 的"缺乏态势感知"结论；
    约 40 枚 al-Husayn 打以色列却被劝住不还手；115 架飞机 01-24 起逃往伊朗；
    西翼 100 公里真空与 GPS／联军后勤两大误判；02-24 误报"8 辆法国坦克"致总参 24 小时后才知主攻方向；
    第 52 装甲旅"未接命令即不动"；第 24 机械化师发现伊炮兵只轰 55 加仑油桶（无法转移火力）；
    Madinah 山脊头十分钟击毁近 100 辆，Franks／Griffith 的"每次都打进同一个地方"对话；
    Tawakalnah 反斜面死战（177 辆坦克＋107 辆装甲车燃烧、击毁美军 4 辆坦克）；
    本书对总参的罕见高分（"定深设防是唯一可能的战略"、用最好的部队殿后＝"从彻底失败嘴里抢回小胜"）。
  · concepts/iraq-1991-final-assessment（章末总评）：与埃及"高度平行"、将帅无清晰模式但"每场战争都拿出
    可能最佳战略"、战术恒定低水平、空军比地面更差（Mirage F-1 的极小例外反证）、军工是"幌子"；
    长处＝后勤／工程兵／勇气／凝聚力；海湾战争的账"值得注意的不是 23 万人逃亡与投降，
    而是另外 25 万人没逃"。
- 更新：events/was-al-khafji-1991 增"从伊拉克一侧补记（ch2）"节并注明两章并列不合并；
  gulf-war 索引加两页；topics 页战例节加两页、国别表伊拉克行加总评链接。
- 甄别：本书未评估伊拉克化学战的规模与系统性、1988 年 Anfal 的具体责任，总评页明写"本页不作评定"；
  1973 年伊军数字与 Herzog／Rabinovich 的差异仍按既有并列处理。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 506 → 509（+3）；whole-wiki QC 为 OK。
- 断点：**第 2 章《伊拉克》全部完成**（1948／库尔德两战／1967／1973／两伊战争／1991／总评）。
  下一批转第 3 章《约旦》：1948—56 边境战与报复行动、卡拉梅 1968、黑九月 1970、1973 年约旦的角色；
  其后第 4 章利比亚（乌干达 1979、乍得 Fada／Wadi Doum／Aouzou）、第 6 章叙利亚（1976 侵黎）。

### 2026-10-22（Pollack 摄入·第 7 批：第 3 章《约旦》全章，5 页；约旦章完成）
- 来源同批 21；本批读 seg-ch3_jordan 全章（约 24.4 万字符）：
  1948 军团评估、1949—56 扩军与英籍军官、Qalqilyah（1956-10-10）与 as-Samu'（1966-11-13）、
  1967 军力与战役、战略与战术评估、"以空军作用"争论、"why Jordan lost"、
  卡拉梅（1968-03-21）、黑九月与叙利亚入侵（1970—71）、1973 的第 40 装甲旅、
  1973 以后与章末总评。
- 新建 5 页：
  · concepts/jordan-british-officers-1956-pollack（约 95 行）：本书把 **1956-03** 当作分水岭。
    1948 年"近代任何阿拉伯军队的最佳表现"，但本书同时称其对手 1948 年的 Haganah 是"很平庸的力量"、
    全部成果只是打平、且成绩几乎全归英籍军官团（引 El-Edroos 与 Dupuy）；
    扩军（1949 的 1.2 万→1967 的 5.5 万）的两个反噬：
    （一）技术兵只能用 Hadari／巴勒斯坦人 → 军队被民族分层（技术勤务＋四个步兵旅为"西岸人"，
    两个装甲旅与五个贝都因步兵旅驻东岸隔在首都与西岸之间，巴勒斯坦军官极少能升营长）；
    （二）1955 年英籍军官占军官职位**一半以上**，1956-03 侯赛因解职 Glubb，
    本书判定真因是**阿拉伯民族主义＋初级军官的晋升野心**（"以民族主义为名、行自身利益之实"）；
    撤离后"明显缺乏可用的营长与连长"（Brig. Peter Young）。
  · events/qalqilyah-and-samu-1956-1966：两战并置显示衰退。
    Qalqilyah：特拉维夫为不惊动英法谈判而否掉夺取 Zuffin 山，"袭击因此变成硬碰硬"；
    第 9 营预备队**三次沿同一条路猛冲、三次被同一支 50 人侦察连伏击**，
    靠以军阻击部队自己撞进约旦侧翼阵地才转势；以军 18 亡 60 伤 vs 约旦 120—300 伤亡。
    as-Samu'：报告混乱＋营长不侦察，全营乘卡车撞进伏击（先 15 辆卡车被打掉）；
    以 1 亡（营长）10 伤 vs 约旦 21 亡 37 伤；唯一亮点是 Hunter 飞行员
    （与 Mirage 缠斗**八分钟**＝以空军史上最长单次空战，以方称约旦飞行员远超埃、叙）。
    书中判语：萨穆"远差于 1948 年最糟的表现"；"希丁"旅后来在 1967 年成为最差的旅之一。
  · events/black-september-and-syrian-invasion-pollack（约 105 行）：48 小时闪击变十个月围城；
    把装甲送进安曼旧城 madinah；5,000 名巴勒斯坦官兵逃亡；叙第 5 步兵师（近 300 辆 T-55／1.6 万人）
    09-20 入约；09-21 约旦第 40 装甲旅**击毁 10 辆 T-55 而自损 19 辆百人队长**；
    **09-22 皇家约旦空军一天 200—250 架次、每机 4—8 架次、16 小时持续在场、零损失**，
    击毁 20—30 辆坦克并"打垮叙军装甲部队的意志"；叙军两日损 62 坦克／60 装甲车／约 600 人。
    本书称 bin Shakir（1970-11 起）的两阶段清剿"慢而残酷但非常成功"，
    并直白写下"以巨大火力与不分对象的杀戮……屠杀了许多巴勒斯坦平民"。
  · concepts/jordan-1973-october-war-pollack：约旦只为"保卫叙利亚"出兵，且**暗中请求以方准许**；
    10-16 al-Majali **不等伊军就独自进攻**（违背安曼"避免重大损失"的意图），损 28 辆坦克；
    10-19 把旅分成三股后撒手不管，损 17—20 辆换以军 4—5 辆；总计 54 辆坦克、至少 80 人伤亡。
    本书用**两重对照**定位第 40 旅：与它自己 1967 年 Qabatiyah 比（同样战斗力，1967 打赢、1970 打输）；
    与 1973 年以军第 7 装甲旅在眼泪谷比（同样的叙军步兵师，以军顶住四天并歼六个旅，约旦不到一天被推回）。
  · concepts/jordan-effectiveness-since-1973-pollack（章末总评＋1973 以后）：
    本书坦白"1973 年以来无实战，只能从美军训练交流与演习推断"；
    长处＝志愿兵制（应征者不足 15%）、单兵技能、报告准确的教导、英式传统残留；
    问题＝训练剧本化、**"他们不喜欢报坏消息"**、合同兵种训练不在一起且缺通信器材、
    在美军课程中被评为"非常平庸的战术家"、兵棋推演中**不被允许担任更高指挥**、
    无法理解任务式命令、部队"实际上无法在旅以上作战"；
    变化/不变两张对照表（1956 前 vs 1967；始终不变的单兵、飞行员、凝聚力、后勤、将帅）。
- 更新：topics 页约旦行扩为五条链接并加 1948—1991 总评条；战例节加两页；
  jordan-army-decline 与 jordan-1948-vs-1967 各加"延伸"段；1973 索引加约旦条；
  events/black-september-jordan-1970（Herzog 线）加"延伸（第二来源）"互链并注明并列不合并。
- 甄别：Qalqilyah／as-Samu' 属 1949—66 边境战，本库无该战争线，页面明示暂挂 `war` 字段；
  黑九月同理（本库无 wars/black-september-1970）。本书未给 1973-10 以军反攻大马士革的确切日期（只写"on October"），
  页面照此留白。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 509 → 514（+5）；whole-wiki QC 为 OK
  （初跑一条指向未建页的 wikilink → 改指事件页后通过）。
- 断点：**第 3 章《约旦》全部完成**。下一批转第 4 章《利比亚》：
  乌干达 1979（Lukuya／Entebbe 方向的战斗）、乍得战争（Fada、Wadi Doum、Aouzou）、
  与美国的冲突（1981 锡德拉湾、1986 空袭）；第 4 章的效能评估页已建
  （concepts/libya-military-effectiveness-pollack），本批需逐战补事件页。

### 2026-10-22（Pollack 摄入·第 8 批：第 4 章《利比亚》逐战，3 页）
- 来源同批 21；本批读 seg-ch4_libya 的乌干达 1979（Lukuya／Entebbe／Kampala 与效能观察）、
  乍得战争 1978—87（Fada、B'ir Kora、Wadi Doum、Oumchi、Aouzou、Maatan as-Sarrah 与效能观察）、
  对美冲突 1981—89（锡德拉湾四次、Attain Document III、El Dorado Canyon、1989-01-04 空战）。
- 新建 3 页：
  · events/libya-in-uganda-1979：02 月起空运 2,500 人＋T-55／BTR／BM-21／MiG-21／一架 Tu-22；
    构成是正规军＋人民民兵＋伊斯兰泛非军团的大杂烩。
    卢卡亚（03-10—12）：利军**无令却碰巧**打散 TPDF 第 201 旅（BM-21 首见、双方无人阵亡），
    随后**停在城里扎营、不挖壕、不派侦察南下**；TPDF 第 208 旅走完 60 公里回行军后夜袭侧后，
    利军溃散，遗尸 200＋乌军 200。坦方指挥官坦言"只是利比亚人的无能救了他们"。
    增兵后又**向民兵隐瞒他们是被送去作战**；Tu-22 空袭 Mwanza **错过整座城市、炸死大批羚羊**；
    恩德培守军在 TPDF 首次步兵冲击下崩溃，第一架起飞的 C-130 被火箭筒在跑道上击毁后空运终止；
    尼雷尔特意留出东侧通道让利军撤走；全役利比亚至少 600 阵亡、伤员三倍。
    本书唯一表扬：**后勤**（4,500 人＋重装备空运并维持数月补给）。
  · events/chad-war-fada-wadi-doum-aouzou（约 130 行）：1965 Frolinat 由来、1971 未遂政变、
    卡扎菲主张奥祖地带；四次介入的共同战略＝Aouzou→Faya Largeau→Oum Chalouba→Abéché→恩贾梅纳；
    1978—86 的分工是"GUNT 出兵与侦察、利比亚出火力"，1986-12 Goukouni 决裂后利比亚既无步兵也无侦察。
    Fada（01-02）8 小时陷落：利 784 阵亡／81 俘／100 辆坦克，FANT 50 死 100 伤；
    B'ir Kora（03-19）两场同一手法（佯攻调走预备队→主攻另一侧），利 800 阵亡、86 毁 13 俘 T-55；
    Wadi Doum（03-22）4 小时失守，利 1,269 阵亡／438 俘（含 Haftar 上校）／300 余辆装甲／
    20 架 L-29／4 架 Mi-24，FANT 29 死 58 伤；Trainor 目击"整场战斗一炮未发"；
    Oumchi—Aouzou（08-08）650 阵亡，08-14 两次反攻被包抄击破，08-28 以巨大火力硬攻夺回；
    Maatan as-Sarrah（09-05）2,500 守军被打垮，利 1,700 余亡、26 架飞机、70 辆坦克，
    FANT 65 人伤亡——**因过于成功**，法国怕乍得全面攻入利比亚而强压 Habré 停火。
    1987 全年利比亚至少 7,500 阵亡、近 1,000 俘、近 15 亿美元装备，而打死不到 1,000 名 FANT。
  · events/us-libya-conflict-pollack（约 110 行）：锡德拉湾 500 英里主张；1981-08-19 两架 Su-22
    对两架 F-14 发射无制导意义的 AA-2（"连目标都没截获"），两机被击落且**均未尝试机动摆脱**；
    1986-03 的 Attain Document III：利 700 架机／受训飞行员或仅 200 名／SA-5 单连／
    防空未整合、实有人数不超编制 60%、夜间基本关闭；03-24 越"死亡线"后利方率先开火，
    SA-5 与 Nanuchka 攻击全部失效，防空被"比四年前以色列对付叙利亚还简单"的两架 A-7 诱饵＋Shrike 打瘫，
    利至少 72 阵亡、美方零伤亡；1986-04-14—15 El Dorado Canyon：意、马耳他两级预警**对利比亚毫不起作用**，
    设施灯火通明、部队不在戒备，150 米低空使 SAM 全部无效，48 枚 Shrike／HARM 压制雷达，
    **一架截击机都未起飞**；- 更新：concepts/libya-military-effectiveness-pollack 删去"留待后续批次"占位、改为逐战链接并新增"战例页"节；
  topics 页战例节加三页；events/entebbe-raid-1976 加"延伸（同一地点的另一次战斗）"互链。
- 甄别：乌干达、乍得、对美冲突三条战争线本库均无，页面明示暂挂 `war` 字段；
  恩德培页（1976 以色列救援）与本批的利比亚乌干达页**分列不合并**；
  乍得内部派系沿革、法国介入政治、对美行动的国际法评价均**超出本书范围**，页面不作补写。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 514 → 517（+3）；whole-wiki QC 为 OK。
- 断点：**第 4 章《利比亚》主要战事已覆盖**（乌干达／乍得／对美／对埃及 1977）。
  余下可补：1970s 的利比亚建军细节、1989 之后；下一批转**第 6 章《叙利亚》**
  （1948／1973／1982 已成页，余 1967、1976 侵黎、1982 后与总评），或按用户指定。

### 2026-10-22（Pollack 摄入·第 9 批：第 6 章《叙利亚》1967＋1970＋章末总评，3 页）
- 来源同批 21；本批读 seg-ch6_syria 的 1948 段（补漏）、1963 政变与苏联关系、1967 兵力与戈兰防御、
  "Syrian Military Effectiveness in the Six Day War"、"Understanding Syrian Military Ineffectiveness"、
  1970 入侵约旦全段、1973 前的阿萨德建军与 1970-11 政变、"SOURCES OF DEFEAT"（1982）、
  "The Syrian Military since 1982"、以及章末 "Summary: Syrian Military Effectiveness, 1948-91"。
- 新建 3 页：
  · concepts/syria-1967-golan-pollack：本书的起手判断——"表面上看叙利亚本该赢下这一仗"：
    地面各项 2—4 倍优势、防守方、极佳地形与工事、完全警戒无突袭可言；
    以方只有制空、熟悉叙军防御、心理势头三项优势，且参战部队疲惫缺编。
    兵力：7 万人／550 辆坦克／500 辆装甲车／近 300 门炮／136 架 MiG（36 架 MiG-21）／16 个旅
    （12 步兵、2 装甲、2 机械化），12 个旅上戈兰。
    核心结论：**指挥链上没有一级愿意实施关键反击**；旅群与总参或可原谅，但前沿旅长有完全指挥权、
    空军阻断又在更靠后处，**没有任何理由不反击**。军官普遍漠视士兵（无证据支持"教派说"）；
    凝聚力"参差不齐"但整体"惊人的好"（Tel Aziziyat 士兵向要投降的军官开枪后死战）；
    真正的瓦解发生在误报 al-Qunaytarah 失守后的撤退中。
    与约旦的受控比较：高层差距极大（约旦会调兵反击、叙利亚"在戈兰任何地方都没有调动兵力"），
    中层"惊人地相似"；由此本书判定**政治化的解释力有限，机动战缺陷才是主因**。
  · events/syria-invasion-of-jordan-1970-pollack：1963 五名初级军官（含阿萨德）掌权、一次解职 700 人
    （半数由阿拉维派补缺）→ 到 1967 年阿拉维派清除所有对手；苏联顾问"是唯一认真教叙军怎么打仗的军官"。
    1970-09-18 派加强装甲旅、09-20 投入第 5 步兵师（近 300 辆 T-55／1.6 万人）打 ar-Ramtha—安曼；
    **"叙军似乎最初根本没有任何干预计划"**；09-21 约旦自损 19 辆只击毁 10 辆，叙军"撞进"第 40 装甲旅
    却仍未能取胜；**09-22 阿萨德以对空军的控制否决出动**，叙装甲被约旦空军打垮
    （实际仅毁 40—60 辆，心理效果决定退却）；叙两日损 62 坦克／60 装甲车（多因故障与弃置）／约 600 人。
  · concepts/syria-effectiveness-1948-91-pollack：章末总评。
    两个独有特征：（一）**后勤是六国中唯一明显更差的**（连苏式"推动"体系都理解不了；
    1976／1982 黎巴嫩作战皆受其累）；（二）本书的"**狗没有叫**"论证——
    叙利亚常是阿拉伯世界政治化最深、准备最差的军队，但战场表现与其他阿军"惊人地一致"，
    1973 年深度去政治化的埃及也"只比戈兰上的叙利亚略好一点"，
    1982 年黎巴嫩甚至好于 1973 年戈兰——**表现恒定，政治化只是部分解释**。
    1982 以后：官方自我吹嘘＋归咎苏械与以空军；军购扩至 40 万人／4,800 辆坦克；
    但仍有 **1,000 辆坦克无受训乘员**、飞行员与飞机比近 **1:2**、1990 年代后期仅 **2/3** 坦克可用；
    唯一做对的＝以 SAM／高炮为主、造地地导弹库、加深大马士革前方防御、扩编突击队（第 14 特种部队师＋7 个独立旅）。
- 更新：topics 页叙利亚行补 1967 与总评两链、总评条加叙利亚、战例节加 1970 叙利亚视角；
  1967 索引加叙利亚效能页（并修一处重复小节标题与多余空行）；
  events/six-day-war-golan-1967（Herzog）与 concepts/syria-1973-golan-pollack 各加"延伸"互链；
  黑九月两页（Herzog 线、ch3 约旦视角）均加指向 ch6 叙利亚视角的链接。
- 甄别：黑九月三条来源（Herzog／ch3／ch6）并列不合并；本书 ch6 未给第 35 旅群完整编成
  （原文被下一节截断），页面照实留白；叙利亚化学武器、导弹项目与对黎民兵作战本书未展开，总评页明示不作评定。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 517 → 520（+3）；whole-wiki QC 为 OK。
- 断点：**第 6 章《叙利亚》全部完成**。至此本书六国章（埃及／伊拉克／约旦／利比亚／沙特／叙利亚）
  与导论、结论均已摄入；尚余可做：埃及章 1948 前史细节、沙特章逐段、
  以及全书层面的横向专题（"脱稿即崩"机制页、六国对照表）。

### 2026-10-22（Pollack 摄入·第 10 批：结论章全章＋六国横向，3 页；本书实质收官）
- 来源同批 21；本批重读结论章（seg-concl 约 11 万字符）全部：
  "Assessing Arab Military Ineffectiveness"（逐项检验八种解释）、
  "What Were the Most Important Factors"（四常量与排序）、
  "Arab History and Modern Warfare"（凝聚力／战略与战术的"教训"）、
  "A Final Thought"（未来、2003 年伊战、非正规力量、作者自述的文化立场）。
- 新建 3 页：
  · concepts/arab-military-ineffectiveness-verdict-pollack（判决书）：
    三项被否——**怯懦**（"从来不是其中之一"；海湾战争真正值得注意的是
    20—40 万逃亡投降之外**另有 10—20 万站住了脚**）、**凝聚力差**（"更可能是强项"；
    正面例：Tawakalnah、Tel Antar、Abu Ageilah、弹药山、Ayn Zhaltah、提贝斯提）、
    **后勤差**（埃及也门 7 万人 5 年、1973 渡河、利比亚空运、伊拉克百万大军八年）；
    四项次要——士气（1973-10-14 士气最高而打得最糟）、将略（无固定模式）、
    训练（越认真越好、练得越苦改善越有限；埃及 35 次、单兵任务几百上千次）、
    技术技能（列为常量但**排序在战术领导力之后**）；
    四项常量与归并——技术技能／维护→"技术"，信息管理→加剧战术领导力，
    **"战术领导者的平庸，对军事效能的损害大于技术技能的匮乏"**；
    末尾记作者自述：本书出自其博士论文，该论文结论是**文化行为模式为首要约束、
    社会经济发展水平次之、政治化只对部分军队是问题、苏联条令与编制可能反而有帮助**——
    本库仅记为 Pollack 的观点。
  · concepts/scripted-vs-unscripted-warfare（机制页）：
    "广泛脚本化与反复演练，实质上免除了下级军官做指挥决策的需要"；
    **"证据当然就是：一旦脚本用完、或敌人迫使其偏离脚本，会怎样"**；
    脚本的门票是"高达十比一兵力比＋突然性"；
    六国档案表（每格链到本库具体页）；三类"精英部队"是例外证明规律
    （约旦军团靠英籍军官＋小规模＋长期服役；叙突击队与伊共和国卫队靠小与精英；
    三国空军精英靠社会挑选＋英法美训练）——"提升究竟多么有限"；
    并说明它与"去政治化"解释的分工（去政治化能修战役层，修不了战术层）。
  · concepts/six-armies-comparison-pollack（四张横向表）：
    四条轨迹（埃／约／伊／叙／利／沙）、兵力装备年表、四项缺陷六国形态、长处分布；
    三条判断：常量在战术层而变量在政治层／长短处互不补偿／
    **差异主要来自"对手是否被迫按它的脚本打"**。
- 更新：topics 页第一节加三页入口；concepts/arab-military-ineffectiveness-pollack 与
  concepts/unit-cohesion-question 各加"结论章的最终裁定"延伸段。
- 甄别：本书的文化解释是其自述立场且明确"另一本书才展开"，页面只记为 Pollack 观点；
  结论章对"未来／军事革命"的判断是推测，页面标为非史实；
  本书否定"怯懦"与"凝聚力差"的说法与本库早期某些表述有张力，页面要求引用时标明"Pollack 口径"并保留其他来源。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 520 → 523（+3）；whole-wiki QC 为 OK。

### 2026-10-22（Yonay 摄入·第 1 批：第 1—6 章，1948 年空军——11 新页＋3 扩写）
- 新来源㉖：Ehud Yonay《No Margin for Error: The Making of the Israeli Air Force》（Pantheon 1993，
  ISBN 0-679-41563-7）；sha256 5a98fc53…；472 页 Internet Archive 扫描 PDF；
  **`pdftotext -layout` 提取，未跑 OCR**（正文层可读）；1,157,058 字符，已切 26 段（ch01—ch26）。
  原始件＋提取文本＋paged 版存于 raw/papers/iaf-yonay/。
- 本批读：Introduction、ch1 Dead Reckoning、ch2 The New Brunswick Warning、ch3 The Czech Knives、
  ch4 The Banana Grove、ch5 The Red Squadron、ch6 Bloodying the RAF（PDF 页 17—92）。
- 新建 11 页：
  · sources/no-margin-for-error-yonay（来源页：sha、章节—PDF 页对照、OCR 讹误清单、写作性质与用法限制）
  · concepts/iaf-independence-struggle-1948：本书最硬的论点——空军难产"不是缺钱，是不想要"；
    Haganah 拒绝两万余名英军复员老兵、Palmach 的苏联式 polirtuk、Ben-Gurion 的两次"绕道"；
    Remez 的 1947-10-23 方案因主张空军半独立被否；1948-07-26 宣布空军独立、07-29 任命 Remez。
  · concepts/iaf-doctrine-air-superiority-first：Margo 1948-07 的优先次序（先夺取制空、后支援地面）；
    取代 Yadin 把空军当炮兵的用法；首次检验在 10 月约阿夫行动。
  · events/iaf-first-fighter-mission-1948（05-29 Isdud）：Remez 原本要打 El Arish（审问被俘埃军飞行员得知），
    被 Avidan 与 Yadin 强令改打 Isdud；四机全部机炮卡壳、Eddie Cohen 失踪；
    物理上"几乎没能刮伤"埃军却使纵队停止前进。
  · events/iaf-czech-airlift-1948：1947-12 首批枪械藏土豆下；04-23 以 180 万美元买 10 架
    （单机 44,000／整机 180,000 美元 vs 剩余 P-51 仅 4,000）；拆解空运 05-20 起；
    Žatec 基地"在苏联默许下"开放；08-11 因 CIA 发现空运而被美方压停。
  · events/israeli-b17-bombing-cairo-1948：07-16 夜一架炸开罗王宫附近（两吨），另两架炸加沙／拉法；
    随后两日 80 架次、50 吨。
  · events/operation-dust-bowl-1948：08-23 起空运内盖夫，至 09-09 共 170 架次／1,000 吨，
    并整旅空运北上休整；本书认为它证明"空运能续命、却确立不了政治主张"。
  · events/iaf-spitfire-ferry-winter-1948-49：航程 600→1,400 英里仍不足 1,500 英里，需南斯拉夫中转；
    Sam Pomeranz 撞山、Bill Pomeranz 迫降被扣；12-22 十架降落 Tel Nof。
  · events/downing-of-raf-spitfires-1949：01-07 与英军交火，两名当事人叙述**互相矛盾**（并列照录）；
    同日共五架 RAF 战斗机被击落；并解开"Shuftykeit"＝英军 Mosquito 侦察机之谜。
  · entities/equipment/avia-s-199：三个致命缺陷（Heinkel 发动机、扭矩无配平、起落架）＋机炮同步器自杀；
    注明"Avia S-199"是通行型号名、**本书从未使用**，性能参数本书未给不补。
  · entities/organizations/iaf-101-squadron：Herzliyya 秘密基地（水塔当塔台、柑橘林掩体）、
    红帽子与骷髅队徽、07-09 三路空袭全部流产、1949-04-01 交接给 Weizman。
  · entities/people/aharon-remez（双来源）、entities/people/modi-alon（单源）。
- 扩写 3 页：entities/people/ezer-weizman 增"Yonay 补充（空军视角）"节并加 sources；
  entities/people/mordechai-hod 增"1948-12 转场飞行"节（含本书脚注：其原姓 Fine）；
  entities/equipment/mirage-iiicj 加注"Yonay 第 13 章尚未摄入"。
- Index：1948 战争索引新增"空中作战"节（9 事件＋2 概念＋1 装备＋1 部队＋2 人物）；
  根索引新增来源㉖与空军专题入口。
- 时间线：本批未改战争时间线——新增事件均已在 1948 时间线覆盖的日期段内，
  且 Yonay 与 Herzog 的日期一致（05-29、07-16、08-23、12-22、1949-01-07），不重复录入。
- 甄别：本书为**记者体叙事**（对话与心理描写为重构），本库只取其**事实骨架**
  （日期、编制、机型、数量、决策），不引对话作史实；与 Herzog 冲突处并列
  （Isdud 停顿的原因：断桥 vs 埃军指挥官判断）。OCR 讹误清单已写入来源页。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 523 → 537（+14，含 3 页扩写）；
  whole-wiki QC 为 OK（初跑 6 处中文问号 → 改写后用〔问号〕保留）。
- 断点：ch7—ch24 未读（1948 后半年起的王子／农夫时代、1956 卡德什、幻影、1967 三小时、1973）。
  下一批建议从 ch7—ch12（1950 年代：Moti Hod 一代的成长、法国转向、1956）开始。

### 2026-10-22（Yonay 摄入·第 2 批：ch7—ch12，1950 年代与 1956，8 新页＋4 合并／扩写）
- 来源同批 1（sha 5a98fc53…）；本批读 ch7 The Prince、ch8 The Farmer、ch9 The Blues and the Greens、
  ch10 The Black Spitfire、ch11 French Shuttle、ch12 Kadesh（PDF 页 95—196）。
- 新建：
  · concepts/iaf-blues-vs-greens（约 120 行）：1949—1953 年军种地位之争。
    Remez 的论证（动员体制依赖制空权）→ 1949-06-20 十五中队计划（370 万美元）→
    Yadin 接总参谋长后的第 81 号指挥令（空军情报归军事情报部）→ Remez 1949-12-14 辞职
    （"总有一天该是 Ezer Weizman"／Ben-Gurion："什么，那头公山羊！"）→
    Shamir（1949-12—1951-08，"把空军变成像炮兵一样的技术兵种"）→
    Laskov（1951-08—1953）的两周调查（48 小时作战能力、单线电话、130 名飞行员只有 27 人可作战）→
    1953-02-23 预算摊牌（"血钱"）→ 1953-04-28 二十页《指挥与参谋结构》（误用英国 general staff 概念）→
    Tolkowsky（1953 起，被 Makleff 拖了六个月才给将衔）的条令修正与"递交辞呈的艺术"。
  · concepts/iaf-training-revolution-ot-u-105：Menahem Bar（原名 Bernstein）其人；
    OTU 105 的四个月日课表、成绩板（射击命中率 15% 平均／20% 良好）、
    枪炮照相机＋彩色漆弹拖靶计分、105／117 编成、喷气化（1953-06-17 两架 Meteor、
    1953-09 首期四名学员、1954-08 中队 12 名喷气飞行员）；
    三个制度化产物：**sevev（周转计时）／yemei krav（战斗日）／战位电话**。
  · concepts/iaf-french-shuttle-1953-56：F-86 求购失败（1954-07-09 加拿大取消）、
    Saab J-29、Mystere II 的负面试飞（Peled 首个超音速以色列人）、
    Ouragan 救场（1955-10-04 建 113 中队）、1956-06-22 法以秘密条约（8,000 万美元／追加 36 架）、
    以及 **1956-08 的"法国穿梭"骗局**（对意大利谎称 18 架次品返修、重喷同一序列号、
    两个基地以"小儿麻痹疫情"封锁，使美方侦察看到的仍是最初 24 架）。
  · events/iaf-sinai-air-war-1956（约 150 行）：Kadesh 1（先炸机场）被 Kadesh 2（禁止打机场）取代；
    开战日 15:00—16:59 的空投编队与"实际上是整个空军"；
    埃及空军反应迟缓到 MiG 被一架 Piper Cub 缠斗十五分钟；
    10-30 的"24 架 MiG"警报其实是**以色列方面发报笔误**（实为 4 架）；
    米特拉地面—空中脱节（38 死 120 伤）；当日 7 架 Mustang 与 1 架 Harvard 全损、两名中队长阵亡；
    10-31 英法终于轰炸后转为对地支援；11-01 蒂朗海峡轰炸与 Peled 被击落获救；
    结语：Dayan 在 Dakota 上宣布"空军第一、装甲军第二、伞兵第三"。
  · events/iaf-operation-rooster-1956：NF-13 夜间截击 Il-14；曳光弹致盲、右炮卡壳甩入左旋；
    第二次把瞄点放在右翼尖上；**脚注记明 Amer 本人改乘 C-47 脱身**，故不得写成"击毙埃军总司令"。
  · events/el-hamma-and-hula-air-actions-1951：04-05 八机几乎全脱靶（炸弹偏 20—60 码），
    05-06 一次"误射"击毙叙军指挥官而定胜负，以色列低调处理并从官方报告删除；此后五年空军未再实战。
  · events/iaf-meteor-vs-vampire-1955：1955-08-31／09-01 汗尤尼斯后的空战，Yoeli 击落两架 Vampire
    （瞄具还停在夜间档、靠曳光修正；第二架正好在自家基布兹上空）；
    本书称这是空军首批被正式承认的喷气战果，也是 Tolkowsky 对"绿军"唯一能用的事实。
  · entities/people/dan-tolkowsky、entities/people/beni-peled（新建，后与既有 benny-peled 合并）。
- 合并与迁移（本次重要的去重工作）：
  · `entities/people/benny-peled`（Rabinovich 线）与新建的 `beni-peled` 经核对为**同一人**，
    已合并为 `entities/people/beni-peled`（别名 Beni/Benny Peled、Beni Weidenfeld），
    1973 年空军司令一段整节并入，旧页删除，全库 4 处链接改指新页。
  · Yonay 线的 Chaim Laskov 与既有 `haim-laskov`（Herzog 线）亦为同一人：
    1951—1953 年空军司令一节整体并入既有页，拼写作 Haim / Chaim 并列，临时新建页删除。
- Index：根索引空军专题补 1950 年代四条；1956 战争索引新增"空中作战（第三来源）"节。
- 时间线：未改——新增事件日期（1951-04-05／05-06、1955-09-01、1956-10-28—11-05）
  在 1956 时间线已有对应条目，且本批为空军视角补充，不重复录入。
- 甄别：本书属记者体，本批涉及的对话一律不作史实引；法国动机（"等美国付完钱"）标为本书说法；
  Rooster 一节特别标明"未击毙 Amer"以免误传。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 537 → 545；whole-wiki QC 为 OK（修 3 处问号、4 处断链）。
- 断点：ch13 Mirage—ch24 Legacies 未读（1960 年代幻影时代、Moked、1967 三小时、1973）。

### 2026-10-22（Yonay 摄入·第 3 批：ch13—ch26 与尾声，1960—1982，14 新页）
- 本批读 ch13 Mirage、ch14 Rebels、ch15 Moked、ch16 The Frontiersman、ch17 Three Hours in June、
  ch18 Keep It Simple、ch19 "Texas"、ch20 Phantoms、ch21 Missiles、ch22 Judgment Day、
  ch23 Operatziot、ch24 Legacies、Epilogue（PDF 页 197—370）。至此全书正文完。
- 新建（概念 5）：
  · concepts/moked-plan-1967（117 行）：1963 春 Weizman 命 Nevo 制定；跑道炸不动（火箭/机炮全失败）；
    手册作废重测航程；情报渗透每座机场；六册附录挂六个业务处；**Tsiddon 算出九成把握需 530 架**；
    8:00 与 first light 之争（含 Weizman 本人的否认，标注"本书不足以支持判断"）。
  · concepts/iaf-operatziot-vs-hunt（107 行）：SA-6 之谜、"物理学 vs 电子学"、Spector 的 hunt
    （诱饵＋猎人、关掉干扰吊舱）、Ben-Nun 的 Tagar（出口塔、弹弓投弹、Shrike 与常规弹对冲）；
    Spector 原话"把我们变成阿拉伯飞行员或俄国飞行员，而我想让我们当犹太飞行员"；
    Peled 1973-05-13 的三条前提与 Dayan"我们当然会是先动手的一方"。
  · concepts/iaf-1973-intelligence-blindness（153 行）：三处结构性失败。渡口航拍照片因"不属空军业务"
    被跳过；空地支援申请要经炮兵—总参—空军作战部七道手续、次日晨才执行；打击规划处六科两科长；
    本书核心判断："导弹不是原因，导弹只是把三个早已存在、多年不出事的缺陷同时暴露出来"，
    以及"Shazly 的导弹本意只是保护入侵部队，结果把空军整个致盲了"。
  · concepts/iaf-reconstruction-after-1973（123 行）：Peled 的误伤自胸、读工程、"把马厩设在舞厅里"；
    复盘会与《乐一通》比喻；把最狠的批评者（Spector）派去训练司令部；Al Ellis 的索尼摄像机无人机
    （1979 年"击落"一架 MiG-21）；Goldman 六个月做出系统；"一支外国部队，但是友好的"。
  · concepts/iaf-blues-vs-greens（第 2 批，本批被多处引用）。
- 新建（事件 6）：
  · events/operation-moked-1967-06-05（101 行）：07:45＝埃及 08:45；三重赌博（顺序/选择/防御 12 架 Mirage）；
    手写纸板、"能返航就返航，不能就撞进海里"；18 分钟出海后左转；八处具体损失；09:00 前近 200 架、
    中午再 107 架；"埃及空军已不复存在"。
  · events/iaf-attrition-air-war-1969-70（194 行）：官方从未颁发的战役纪念章；Bir Gafgafa 的铜钟与大钟；
    编制空虚（没中队有超过半打老手）；"Texas"（Rimonim）只派冠军阵容、Hod 掐秒表指挥；
    "击落飞机没有用，它没有吓住埃及炮兵"；Boxer 159 吨＋72 罐凝固汽油弹；
    Phantom 深突袭与两次误炸（70 名工人／数名儿童，本书判为"可能是情报失败"）；
    苏联三招（集中 SA-2／SA-3 补盲／超级阵地）；pod formation 与 Hetz 之死；
    El Adabiya 2 分钟 5 架苏联 MiG；停火当夜导弹前移 16→50 个阵地；Toaster 的名不副实。
  · events/dougman-v-1973-10-07（138 行）：48→8→0 小时；"第三圣殿危在旦夕"／"西奈是沙子，这里是家"；
    Henkin 违反"禁止二次进入"撞地；六架 Phantom 换两个阵地；Peled 返回地堡下令炸桥、16:30"七座桥"；
    Spector 两次改命令两次零损失；"逐字执行任务命令的中队伤亡最重"；当天损失 35 架。
  · events/bekaa-valley-1982-air-battle（117 行）：19 个导弹连、首日毁 17、叙机 29→80 架、以方 1 架 A-4；
    本书自述"可能不完全准确"；另加第二节与 Price 卷 III（EW 技术层）的并列对照。
  · events/entebbe-airlift-1976（81 行）：Peled 的 1,200 人／2,000 英里方案被 Gur 当面否决、
    五天后由佩雷斯扭转；四架 C-130＋两架 707（一架空中医院、一架空中指挥）；18 分钟。
  · events/osirak-raid-1981（62 行）：八架 F-16＋六架 F-15、635 英里、贴地穿沙特约旦、两分钟。
  · events/elie-cohen-syrian-front-1960s（70 行）：只写本书提到的情报用途，明确不从书外补生平；
    1967-04-07 拖拉机"由头"、六架 MiG、Rabin"这是什么样的空军"。
- 新建（人物 3）：entities/people/iftach-spector（102）、entities/people/shmuel-hetz（74）、
  entities/people/avihu-ben-nun（64）。
- 合并/去重：本批无新重复（Beni Peled、David Ivri、Mordechai Hod 均已在库，仅链接）。
- Index：1967、消耗战、1973、1982 四个战争索引各加"空军视角"节；根索引空军专题扩充 14 条入口。
- 修正（QC 3 轮）：
  · 6 处 wikilink 内误写 `\|`（表格转义残留）导致解析失败 → 全库正则修正；
  · 9 处中文问号 → 〔问号〕（dougman／elie-cohen／spector／blindness／hunt）；
  · 4 处指向未建页的链接（golan-syrian-breakthrough、cold-war-air-power-lessons、
    iaf-phantom-era）→ 改指已建页；entebbe 链接指向错页名（entebbe-raid-1976 才是既有页）。
- 本书全局限制（本批反复出现，已写入各页）：记者体，对话一律按"某人回忆"处理；
  多处明写"本书不足以支持判断"（8:00 之争、Rooster 是否击毙 Amer）；贝卡谷地细节本书自认不确定。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 545 → 559；whole-wiki QC OK。
- 断点：**正文与尾声已全部读完（ch1—ch24＋Epilogue）**；余 Author's Note 与致谢未逐字读（不含史料）。
  Yonay 线实质收官。可选补漏：ch14 中 Gazit 与 Weizman 冲突的具体日期；ch20 的 Phantom 中队番号
  （本书明示部分为化名）。

### 2026-10-22（Yonay 摄入·第 4 批：Author's Note ／ Sources ／ 收线，2 新页）
- 本批读 Author's Note（PDF 页 371—374）与 Sources 三层（PDF 页 377—395）。
  这是**收线批**：不再产生战役或人物新事实，而是给整条 Yonay 线加上史料学层。
- 新建：
  · concepts/yonay-sources-and-methodology（"谁在说话"）：三层史料结构（约 75 人次访谈为主、
    约 55 种第二层文献、6 种多为 classified 的空军内部出版物）；作者自陈的三重不利
    （从未服役、带"空军始于 Weizman"的错误预设进场、被视作 Yored——Lapidot 当面拒他
    "你是个 Yored，你为钱写作。我为什么要帮你"）；Hod 给他的方法（"按时间顺序跟每一位司令谈，
    从 Remez 开始"）；作者自己承认的"机构修正主义"与对 Menahem Bar 被省略的致谢；
    **化名清单**（Gad Eldar、Amichai Gal、Danni Brown／Josh Elon、Yehuda Palit、Menahem Goldman
    与"221"／"171"两个虚构中队番号），并据此定纪律：**化名人物不建 canonical 实体页**；
    本书五条偏向；"哪些内容本库能交叉验证"的对照表。
  · concepts/iaf-six-theses-yonay（"一支空军怎样看待自己"）：把散在 24 章里的判断抽成六条，
    逐条列出落点与自我矛盾（尤其判断 5"1973 年的真正原因是失明"——**同时是原告与证人的陈述**，
    库内只作一个解释并列，不作定论），并给出三条本库的保留意见（蓝绿框架过窄、
    "系统性卓越"的证据只取成功案例、人物评价高度依赖被访者恩怨）。
- 扩写 sources/no-margin-for-error-yonay：新增"四之二、Sources 的结构"。
  **本批最实用的一条副产品**：Sources 的访谈名单里，人名后括号内是**改姓前的原姓**——
  Beni Peled (Feldman)、Moti Hod (Fine)、Shaya Gazit (Schwartzman)、Yak Nevo (Milner)、
  Ran Ronen (Pecker)、Menachem Bar (Bernstein)、Shlomo Lahat (Landau)、Moshe Peled (Weidenfeld)。
  这正是第 2 批"Beni/Benny 是同一人""Chaim/Haim Laskov 是同一人"两次去重的判断依据，
  今后遇到同名疑点应先查这张原姓表。此外新增"五之二、Yonay 线页面总表"（概念 11／事件 18／
  实体 9／扩写既有 5）。
- 记录一处本书内部的不一致（不判定）：Author's Note 说作者"从未服役"，同一页说他毕业于
  Kadoorie 农业高中、同班 65 人只有 1 人进空军——**这是他诉诸"外人视角"的自述，不是史料矛盾**。
- 由本批确认的一处**史实纠错**：Author's Note 记作者少年时的传说"Modi Alon 1948 年在特拉维夫上空
  打下两架 Dakota"——本书正文已写明那次是两架埃及 C-47／Dakota 型轰炸机（即 **B-17 轰炸开罗**前后
  拦截行动中的对手），与本库 [[events/iaf-first-fighter-mission-1948]] 的口径一致，不需改页。
- Index：根索引空军专题补两个史料学入口。
- 检查：SCHEMA sha256 191cd20f…（未变）；内容页 559 → 561；whole-wiki QC OK。
- **YONAY COMPLETE**：正文、尾声、Author's Note、Sources 已全部摄入（ch1—ch24＋Epilogue，
  PDF 页 17—395）。仅 Index（PDF 页 396 以后）未逐条读——索引为多栏混排、OCR 不可靠，
  按用户提醒本就不作命名依据。
- 本线成品：概念 11、事件 18、实体 9、扩写既有页 5；QC 三轮修正（6 处 `\|` 残留、
  9 处中文问号、4 处断链／错页名）。

### 2026-10-22（Van Creveld《The Sword and the Olive》· 第 1 批：全卷通读＋机构层主干）

- 来源：Martin van Creveld, *The Sword and the Olive: A Critical History of the Israeli Defense Force*,
  PublicAffairs 1998／平装 2002，449 页。sha256 `c7e26a42…`（全值见来源页）。
- 提取：`pdftotext`（数字文本 PDF，非扫描、未跑 OCR）+ `pdftotext -layout`；生成
  `raw/papers/idf-van-creveld-sword-olive/` 下 `idf-van-creveld-sword-olive.pdf`、`sword-olive-paged.txt`、
  `sword-olive-layout.txt`、`sword-olive-clean.txt`（450 个 `<<<PDFPAGE\|BOOKPAGE>>>` 定位标记）。
- 本批通读范围：PDF 1—23（卷前、术语表、平装版序、导论）、26—286（第一至三部 ch1—ch17 全部正文）、
  288—386（ch18—ch21 与结语，部分段落快读）、388—426（Notes 抽样→未逐条录入）。**尚未逐字读 ch11—ch13 的战役段落细则**（仅取结构信息）。
- 新建（来源层 1）：`sources/idf-van-creveld-sword-olive.md`（含**章节—PDF 页对照全表**、本书性质与用法限制）。
- 新建（机构层 1）：`entities/organizations/idf-tzahal.md`（沿革 Bar Giora→Ha-shomer→Hagana→PALMACH→TSAHAL、
  指挥链与法律地位、总参与军种结构、1949—1982 兵力表、军队—社会关系、本书总评）。
- 新建（概念 10）：
  · `idf-manpower-and-reserves`（1949 年服役法、三角结构、服役期变动表、预备役正反两面、"en brera"）；
  · `idf-officer-corps`（行伍出身、年龄与 PAZAM、教育缺陷、1984—94 军衔通胀数据、宗教军官化）；
  · `idf-civilian-control-and-censorship`（服从纪录 vs 监督缺失、1945 年紧急条例、主编论坛、Vanunu、1989 年判决）；
  · `idf-command-culture-optional-control`（机制、1956/1967 成功面、1973"反向 optional control"、1982 多头指挥室）；
  · `idf-women-conscription-chen`（PALMACH 五分之一、CHEN 1948-06、MOS 210→296→500/234、黎巴嫩与 Intifada 转折）；
  · `idf-armor-doctrine-helem-hashiryon`（Tal 的装甲论证、训练改革、1967 误读、1973 崩解与自发修正）；
  · `idf-nation-building-role`（GADNA／NACHAL／移民教育班、"民族学校"论、发展理论出口）；
  · `idf-dayan-milson-occupation-1967-87`（1967 两张方案、Dayan 最低干涉、Gush Emunim／Likud 定居、乡村同盟、Intifada）；
  · `idf-decline-thesis`（因果链、可核查量化支柱、作者自承的反面证据、用法纪律）；
  · `idf-defense-industry-complex`（TAAS／RAFAEL／IAI、1966—84 产值出口表、"两头卖"、Lavi 取消）。
- 新建（事件 1）：`events/idf-trust-crisis-1982-1997`（黎巴嫩—Intifada—事故诉讼—新史学家的四段信任崩解时间轴）。
- 新建（专题 1）：`topics/idf-force-history`（IDF 军队史专题入口，含"本书与他源分工表"）。
- 更新（既有 7 个战争索引）：1948、1956、1967、消耗战、1973、1982、海湾——各加"机构层（第四来源）"小节并
  在 `sources:` 追加 `idf-van-creveld-sword-olive`；海湾战争一栏另记 1991 年以色列反导/民防的"无能"判决（ch19）。
- 时间线（3 处增量，不覆盖既有条目）：
  · `wars/gulf-war/timeline.md` 新增"以色列方面的日期（据 ch19）"：1991-01-18 首轮落弹、全程约 39 枚、伤亡与房屋损失、1991 年后设本土防线司令部；
  · `wars/war-of-attrition-1969-70/timeline.md` 新增"机构侧增补（据 ch12）"：1968-09-08、Naj Hamadi、1969-03-08 开战节奏与 84/475/231 事件数、
    1969-07-20 动用空军、夺雷达与夺岛、1969-08—12 阵亡 180、1970-08-07 停火与违约；
  · `wars/sinai-campaign-1956/timeline.md` 新增"机构与指挥侧（据 ch9）"：塞夫勒、10-29 空降 395 人、10-31 拉法协同失灵、
    Ibrahim al Awwal、11-04/05 沙姆沙伊赫、作者对"英法未动则战果存疑"的判断。
- 检查：`SCHEMA.md` sha256 `191cd20f…`（未变）；全库 dual-mode QC **0 PROBLEM**；14 个新文件 `newpages-check` CLEAN；
  glitch-scan 仅余 ascii-word 白名单项与一处标题（# IDF 女兵与 CHEN，属误判）；内容页 561 → 576。
- 异常 / 需要人工确认：
  · 本书为**单一作者的批判史**，评价性极强（"1967 胜利是以色列最坏的事""IDF 软肿"等），各页已统一标〔Van Creveld 判断〕；
  · 本书数字多为作者综合二手，与他源（Herzog／Rabinovich）冲突时按本库规则**并列不合并**，已在 `idf-decline-thesis` 留下对读入口；
  · 1956 年以方阵亡数本书给 **190**、1967 年 **980**、1973 年 **2,800**（ch14）——与 Herzog/Rabinovich 数字并列使用，勿替代。
- 断点：**全书正文已通读**；下一批可按需逐章细补（建议次序：ch1—ch4 建国前线的 Ha-shomer/Hagana/PALMACH 专页、
  ch9—ch10 的 1956 编成与 1967 战前核问题、ch13—ch14 的 1973 指挥层人事、ch17 的 1982 出兵规模与指挥室结构）。
### 2026-10-22（Van Creveld《The Sword and the Olive》· 第 2 批：ch1—ch5 建国前线）

- 说明：同一文件（sha256 `c7e26a42…`）二次调入，判定为**已摄入来源的增量批**（非重复、非来源漂移）；不重建来源页，
  只补第一批明确留空的建国前线（Ha-shomer／Hagana 建制／1936—39 起义）。
- 本批细读：PDF 28—98（ch1—ch5），逐段核对原始提取文本 `sword-olive-clean.txt`。
- 新建（3）：
  · `entities/organizations/ha-shomer.md`：Bar Giora／Ha-shomer（1907—1920）——Gomel 核心十余人、约百人规模、
    120 法郎步枪与 40—120 法郎月费、Kfar Tabor（1909）与 Merchavia（1911）两次"占地"、Jamal Pasha 驱逐 7,500 俄籍移民、
    Ben Gurion 申请被拒、1920-05 解散并移交 Hagana。
  · `events/nili-network-1917.md`：NILI（Zichron Yaakov；1917 年 9—10 月被奥斯曼破获）。**严格限于本书两段所述**，
    不补成员名单与情报内容，页内已标明这一史料限制。
  · `events/arab-revolt-1936-39.md`：1936—39 年阿拉伯大起义——04-19 雅法骚乱（16 死）、最高委员会与 172 天总罢工、
    Kauji 的四连、1938 年春 15,000 名游击、Wavell 在杰宁的 2,000 人正规战；**犹太方所得三件**：notrim／辅助警察 3,000 人、
    kofer ha-yishuv 负担 70% 经费、nodedot 400 人／FOSH 300 人；Wingate 的 SNS（40 英军＋75 notrim）与其"五条条令"。
- 更新（1）：`concepts/haganah-palmach.md` 追加"补充资料（据 Van Creveld ch1—ch4）"——1920—39 建制年表、
  1929 年六天伤亡（133 犹太死／116 阿拉伯死／希伯伦 65）、1939 年家底（15,000 人、步枪 6,000 等）、PALMACH 编制与规模
  （1943 年 1,000／1944 年 1,500／第一批结业 427 男 6 女）、Post Occupation Scheme、1945—46 反英作战（Atlit、11-01 铁路 153 处、
  06-17 十一桥炸十）、ETSEL／LECHI／saison 关系。原 Herzog 段落未改动。
- 时间线（1）：`wars/war-of-independence-1948/timeline.md` 新增"托管前（据 Van Creveld ch1—ch4 增量）"共 28 条日期条目
  （1907—1947，含 1946-06-29 Agatha 行动与 1946-07 大卫王酒店），并注明与 Herzog 线并列不替代。
- Index：根 index 来源㉗ 一行与"军队史专题"入口补 3 个前身页；`wars/war-of-independence-1948/index.md` 机构层节增"建国前身线"；
  `topics/idf-force-history.md` 增"七、建国前身线"一节（原"待续"改为第八节）。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；全库 dual-mode QC **0 PROBLEM**；5 个改动文件 `newpages-check` CLEAN。
- 异常：本书 1947 年 Hagana 家底（迫击炮 754、步枪 17,642 等）与 Herzog 线 1947 年数字（步枪 10,500 等）差异较大，
  已在时间线内并列标注、未合并。
- 断点：ch1—ch5 已逐段核对；ch6 以后仍按第 1 批通读结论使用。下一批建议：ch9—ch10（1956 编成与 1967 战前核问题段）或 ch13—ch14（1973 指挥层）。
### 2026-10-22（Van Creveld《The Sword and the Olive》· 第 3 批：ch8—ch10 过渡期与 1956 编成）

- 同一文件（sha256 `c7e26a42…`）第三次调入：仍为**增量批**，不重建来源页。
- 本批细读：PDF 126—200（ch8 兵役三角与军官团、ch9 渗透—报复—1956 西奈、ch10 建军与 1967 战前核问题段），逐段对照 `sword-olive-clean.txt`。
- 新建（1）：`concepts/idf-sinai-1956-order-of-battle.md`——1956 年以军**师（ugda）层级编成**（38 师：10、4、37 旅＋7 装甲旅预备；
  77 师：1、27 旅；202 伞兵旅；9 摩托化旅；55 伞兵旅预备）、动员（10-24 个别召集、逾 10 万应召、超编）、
  Dayan "不在场"的指挥设计、**十条事故清单**（空投测错、Mustang 割线、扳手、米特拉山口违令、38 师两旅长与师长被撤、
  Simchoni 提前放装甲、7 旅与 37 旅互射、Eytan 部队无后勤、误击 HMS Crane 与己方、Dayan 征用埃军轿车）、
  作者的两项保留（埃军已撤走约一半→45,000∶30,000；10-31 19:00 时只有佯动方向成功，若无 Musketeer 是否同样成功"存疑"）。
- 更新（3）：
  · `entities/people/moshe-dayan.md` 加"补充资料（据 ch1—ch14）"——早年（Ha-shomer 时代 1915 生、1939 判 10 年）、
    总参谋长任内的报复政策与指挥风格、对装甲兵的成见（Kalkiliya 禁用装甲、"坦克上运输车"提议）、1967/1973 与 Agranat 结论。
  · `concepts/idf-nation-building-role.md` 新增"二之补：1949—1970 年代军国化的社会机制"（纪念读物、军队演出队、brarah 一代、
    Ben Gurion 议会主张、i katan／meatim mul rabbim 与感知 1:3）。
  · `wars/sinai-campaign-1956/index.md`：修正来源状态抬头（主源 Herzog，并列 Yonay／Van Creveld 三源），机构层节挂本战专页。
  · `topics/idf-force-history.md` 转折与评价节挂入本战专页。
- 撤销一项拟建页：ch5 曾拟开「政治对抗单位」专页，但该名称与四项职能在本 PDF 文本层查无对应段落（属我误记），
  按「不确定即留白」原则删档、不建页。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；全库 dual-mode QC **0 PROBLEM**；4 个改动文件 `newpages-check` CLEAN。
- 断点：ch8—ch10 已逐段核对；下一批建议 ch13—ch14（1973 指挥层与损失统计）或 ch17（1982 出兵与指挥室）。
### 2026-10-22（Van Creveld《The Sword and the Olive》· 第 4 批：ch13—ch14 1973 指挥层与损失口径）

- 同一文件（sha256 `c7e26a42…`）第四次调入：仍为增量批，不重建来源页。
- 本批细读：PDF 240—266（ch13 十月地震全章、ch14 清算），逐段对照 `sword-olive-clean.txt`。
- 新建（1）：`concepts/idf-1973-command-and-generals.md`——战前顶层人事（1971 年末 Bar Lev 去职、Elazar 接任、Sharon 转预备师、Gonen 升任）；
  前线与后方指挥结构表（Elazar／Tal／Gonen／Adan／Sharon／Mandler→Magen／Choffi／Eytan／B. Peled／Bor 内的 Yadin、Rabin、Weizman、Zeevi）；
  作者的两个关键判断（"被一群据称才华横溢的将军缠住"、"反向的 optional control"）；Agranat 的组成、处置与"情报评估仍归 IDF"的结构性批评；
  战后制度调整（预备役不得指挥大于旅、常设师与军、1983 年 MAFCHASH、1982 年顶层更糟）。
- 更新（1）：`concepts/yom-kippur-1973-outcome-assessment.md` 加"第二口径：Van Creveld 的损失与强度对照"——
  四场战争的阵亡／伤／"每面对一个阿拉伯师所付阵亡"（1948—49：5,682；1956：190／900、76:1；1967：980／4,500、98:1；1973：2,800／8,300、200:1；1982 首周 113:1）；
  日均阵亡 100+ vs 1948 年 15 人但人口五分之一的换算；与 Rabinovich 口径（2,656／7,250）**并列、指出差异约 5%—14%、不裁决**。
- 更新（2）：`wars/yom-kippur-war/index.md` 机构层节加"本战指挥层"两条；`topics/idf-force-history.md` 转折与评价节挂入指挥层页。
- 一处自纠：指挥层页初稿把编注残留 "author：" 混入正文，已改为正常叙述。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；全库 dual-mode QC **0 PROBLEM**；3 个改动文件 `newpages-check` CLEAN。
- 断点：ch13—ch14 已逐段核对；下一批建议 ch17（1982 出兵规模、北方军区作战室与贝卡空战的组织面）或 ch15—ch16（重建与军工／核）。
### 2026-10-22（Van Creveld《The Sword and the Olive》· 第 5 批：ch15—ch16 重建、扩军与军工／核）

- 同一文件（sha256 `c7e26a42…`）第五次调入：仍为增量批，不重建来源页。
- 本批细读：PDF 272—306（ch15 恢复与扩张、ch16 军工与核），逐段对照 `sword-olive-clean.txt`。
- 新建（1）：`concepts/idf-rebuild-and-expansion-1973-82.md`——兵力表（1973／1977／1982：现役 115k／164k／170k，
  总兵力 30 万／40 万／54 万，师当量 7／13／16）、编制变化（军 corps、准将衔、总参谋长升中将、1983 年装甲兵降格与 MAFCHASH）、
  装备存量表（坦克 1,700→3,600；装甲车 3,000→8,000；火炮约 2,000；作战机约 400→近 700；导弹艇 12→19；E-2C 六架、
  AH-1／MD-500、CH-53、Harpoon／Barak／火神密集阵）、动员后勤改革（维护监察署、YAMACHim、干贮存、卡车与坦克运输车）、
  美援与国内代价（1967 前后 ≤5,000 万→年均 2.5 亿→22 亿→30 亿→1984 年 45 亿占 GNP 20%；国防占 GDP 8.7%→21.3%→26.3%，1973 峰值 32.7%；
  通胀 37%—400%）、1973 年美空运的定量评断（约 200 架次、50 架 F-4、155／175 mm 弹）、Lavi 始末。
- 更新（2）：`entities/equipment/merkava.md` 加"第二来源"节——Tal 的装甲论证前提、M-60 的四项缺陷、发动机前置与后部大弹药舱、
  扁平收窄炮塔、105 mm＋激光测距＋火控＋Arrow 弹、Mark II／III（120 mm、全电炮塔）、与 NAGMASH／反应装甲的配套；仍留白车重精确值等。
  `wars/lebanon-war-1982/index.md` 机构层节加"出兵前的底账"一条；`topics/idf-force-history.md` 挂入重建页。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；全库 dual-mode QC **0 PROBLEM**；3 个改动文件 `newpages-check` CLEAN。
- 断点：ch15—ch16 已逐段核对；下一批建议 ch17（1982 出兵规模、北方军区作战室与贝卡空战的组织面）或 ch19—ch21（海湾／Intifada／信任破裂）。
### 2026-10-22（Van Creveld《The Sword and the Olive》· 第 6 批：ch17 黎巴嫩战争的编成与指挥）

- 同一文件（sha256 `c7e26a42…`）第六次调入：增量批，来源页不动。
- 本批细读：PDF 308—330（ch17 黎巴嫩泥潭全章），逐段对照 `sword-olive-clean.txt`。
- 新建（2）：
  · `concepts/idf-lebanon-1982-order-of-battle.md`——6.5 个师入黎＋1 个师在戈兰警戒（作者算作 1973 年南线兵力的两倍）；
    自西向东编成（沿海两师 Mordechai／Yaron＋Awali 河两栖旅；中部 Kahalani 师；其后 Einan 师向贝鲁特—大马士革公路；
    Metulla 方向 Ben Gal 少将的两师军；戈兰 1 师预备）；指挥结构"头重"（作战室内 Drori、其副手、Saguy、Yariv、Eytan、Levy、Efrat、Sharon，头两天还有 Begin）；
    Drori 控制幅度过大；Yekutiel Adam 死因不明；两条规模解释（对苏威慑／Sharon 与 Eytan 的重心之争）；
    后果（拥堵、不用直升机夺点、沿海三日改六日、Einan 误令损失 12 小时、Sultan Yakub 未侦察入伏）。
  · `events/bekaa-valley-1982-air-battle-vancreveld.md`——贝卡战役的**第三口径**：19 个叙军导弹连＋ZSU-23-4；
    IAF 一年猫鼠游戏标定阵地与雷达频率；RPV 诱雷达开机→F-4／F-16 反辐射弹→可能集束炸弹；
    **M-107 175 mm 火箭增程弹参与 SEAD（射程 25 英里）**；E-2C 提前识别升空叙机；
    结果近 100 架对 1 架（约五分之一叙空军，100:1，1967 为 30:1、1973 为 50:1）；
    作者判断"空中大胜、地面作用有限"，含 6-10 **误击己方装甲营**。
- 更新（1）：`wars/lebanon-war-1982/index.md` 机构层节挂入上述两页（编成页与贝卡第三口径页）。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；全库 dual-mode QC **0 PROBLEM**；3 个改动文件 `newpages-check` CLEAN。
- 断点：ch17 已逐段核对；仅余最后一批（ch6—ch7、ch11—ch12、ch18—ch21）。
### 2026-10-22（Van Creveld《The Sword and the Olive》· 第 7 批＝收线：ch6—ch7、ch11—ch12、ch18—ch21 核对完毕）

- 同一文件（sha256 `c7e26a42…`）第七次调入：**收线批**。本批把此前只"通读取结构"的章段逐段核对完，
  本书至此**全章（ch1—ch21＋结语）已逐段核对**，不再留有未读正文。
- 本批细读：PDF 116—123（ch7 成就与代价）、202—266（ch11 六日战争三线、ch12 城门下、ch13—ch14 复核）、330—386（ch18—ch21、结语）。
- 新建：**0**（本批不新开页——按"同题已有 canonical 则增量"原则，全部落在既有页）。
- 更新（4）：
  · `concepts/war-of-independence-assessment.md` 加"第二口径：Van Creveld 的伤亡统计与代价论"——
    死亡 5,682（军人 4,520／平民 1,162）、男女与平民分布、阶段分布（1947-11—1948-05 约 2,000；05-15—06-10 1,200）、
    年龄结构（18—30 岁占 64.8%）、Latrun 383 人（含 3 名女性）、女性军人死亡 108 人（占军人 2.4%，女兵占兵力 10.6%）、
    "占全部战争死亡约三分之一"、"比英德 1914—18 更密集"、纪念书 320 种；并记作者否定"失去一代"说法的理由。
  · `concepts/bar-lev-line-origins.md` 加"第三口径"（Van Creveld ch12 的两派版：Tal＋Sharon vs Bar Lev，
    政治理由＝防止安理会固化立足点），并扩成**三源对照表**（Herzog／Rabinovich／Van Creveld），
    记录 Herzog 归 Gavish 与 Adan、Van Creveld 直接归 Bar Lev 的差异，不裁决。
  · `concepts/idf-rebuild-and-expansion-1973-82.md` 加"地面部队编制细节"（军常设化与同级指挥、每装甲营配一个乘车步兵连、
    取消师属侦察营的争议、"武装定居点"计划失败）。
  · `concepts/idf-decline-thesis.md` 加两节量化："1991 年海湾战争"（39 枚导弹、恐惧致死与敌火致死 10:1、1,000 人就医、
    三分之一面具不合脸、HAGA→本土防线司令部、预警 2→7 分钟）与"Intifada 的制度消耗"（巴方亡约 1,200、
    生活水平 −40%、300 名官兵受审、1996 年 7% 合格者未入伍、预备役报到率约 50%、72% 称服役打击士气）。
- 复核结论（写入各页时已注明）：ch11 的 1967 年三线叙述与既有 Herzog／Yonay 页无实质冲突（本书数字与之并列）；
  ch12 的消耗战时间线已在前批落入 `wars/war-of-attrition-1969-70/timeline.md`，本批补其制度面（Bar-Lev 之争）。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；全库 dual-mode QC **0 PROBLEM**；4 个改动文件 `newpages-check` CLEAN。
- **本书收线**：来源页 1、机构层 1（`idf-tzahal`）、`concepts/idf-*` 15 页、事件 4（NILI／1936—39 起义／1982 贝卡第三口径／信任破裂）、
  前身组织页 1（`ha-shomer`）、专题 1；7 个战争索引与 3 条时间线挂接；
  两处"误记拟建页"已回退（政治对抗单位、以及未成立的三源合并数字）。

### 2026-11-04（Lambeth《Moscow's Lessons from the 1982 Lebanon Air War》· RAND R-3000-AF, 1984 · 单批完成）

- 来源：`Moscow_Lessons_1982_Lebanon_Air_War_unrestricted.pdf`（62 页）· sha256 `15bc8f6d74c82e7677747ae34784037c03095ce797de0bac4d898da6c1cda104`
- 提取：pdftotext -layout（用户提供即为 Acrobat Paper Capture OCR 版，未重跑 OCR）；raw 存 `raw/papers/moscow-lessons-1982-lebanon-lambeth/`（pdf＋txt）。
- 通读：全书 2351 行（前言/摘要/§I—§V/Dubrov 附录 p.35—46），一次通读，无分段遗留。
- 新建（4）：
  · `sources/moscow-lessons-1982-lebanon-lambeth.md`——含 OCR 校读说明（!AF=IAF、ia=is、页眉数字混行等）。
  · `events/bekaa-valley-1982-soviet-lessons-dubrov.md`——Dubrov 原文要点（CAP 正负、"VKP"式中枢、APG-63/上半球 >80 km、
    双机 1000 m 上下半球搜索、"战斗机之间首次互动"、AIM-7F 5—50 km、全向=未来浪潮、RPV 单价 100 万 vs 有人机 1000 万、
    Mastiff Mk2 参数、SEAD 四阶段、Ze'ev 40 km 无制导地地弹、Shrike/Standard ARM 防区外仅 13—16 km）＋Lambeth 三处重大误判与结论层。
  · `concepts/soviet-propaganda-lebanon-1982.md`——1982 年宣传口径逐条清单（06-11 电台、07-01 TASS、07-03 Zamyatin "40 架"、
    07-18 红星报"67 架"、Kashuba 系列）＋Yurasov/Ogarkov 代表团＋SA-5/SA-8/SS-21 军援。
  · `concepts/airborne-command-and-control-1982.md`——GCI vs 自主搜索 vs 空中指挥所三种形态的作战概念页。
  · `concepts/bekaa-1982-numbers-four-sources.md`（comparison 型）——Herzog/Yonay/Van Creveld/Pollack/Lambeth 五列数字对照，不裁决。
- 更新（4）：
  · `events/bekaa-valley-1982-air-battle.md` 新增第九节（Lambeth 背景、10 分钟压制次序、90v60、Creech 机型拆分 40/44/1、机炮 7%、
    叙飞行员"飞 8 字"、Eitan"假想线"）＋frontmatter sources/updated；页首说明改为三源。
  · `events/bekaa-valley-1982-sam-suppression.md` 增"第二口径：Lambeth 对同一链条的细化"（炮兵/Ze'ev 与 F-4 ARM 按射程分工、四阶段）。
  · `wars/lebanon-war-1982/index.md` 增"苏联与对手视角"节＋sources/updated。
  · `wars/lebanon-war-1982/timeline.md` 增"空中作战的补充日期（Lambeth 口径）"9 条（1981-04-29/30、06-09 计数、06-10、
    06-13 Yurasov、07 Ogarkov、07-01—07-20 宣传、08 SA-8 击落 F-4、1983-09/10 Dubrov 文）。
- 未建页的说明：Dubrov 与 Lambeth 均未给 E-2C/707A/SA-8/Su-27 的新技术参数（只有零星数字），按"不造浅页"原则不新开装备页；
  SS-21 仅一处提及，不建页。SCHEMA 无需扩展。
- 检查：SCHEMA sha256 未变；新增/修改页 YAML 有效、sources 齐、wikilink 未指向不存在页；
  `events/bekaa-valley-1982-air-battle.md`、`wars/lebanon-war-1982/index.md`、`timeline.md` 编辑时工具报"sibling subagent 修改过"，已按当前内容 patch 未覆盖（patch 前均读取段首）。

### 2026-11-04（Grant《The Bekaa Valley War》· 2002-06-01 · 单批完成，与同日 Lambeth 批次同源战例）

- 来源：`The Bekaa Valley War By Rebecca Grant June 1 2002_20261104140437.pdf`（10 页，重新排版件无 OCR 噪声）·
  sha256 `bcd7a98b132a07def4fb3f04e37040decce7ee48ff3a6e08f4fc74e5bb6e23f7`；
  归档 `raw/articles/bekaa-valley-war-grant-2002.pdf`＋`.txt`（原文件名的 `2026…` 为导出时间戳，已更名）。
- 性质：对 1982 年以空军司令 **David Ivri** 的专访式叙述（大量直接引语），非档案研究；作者为 IRIS 总裁、Eaker Institute 研究员，
  文体属美国空军协会系统刊物。文中"ZSU-24"为笔误（应为 ZSU-23-4），页内已标〔原文作 ZSU-24〕。
- 新建（1）：`sources/bekaa-valley-war-grant-2002.md`。
- 更新（6）：
  · `events/bekaa-valley-1982-air-battle.md` 增第十节（战前 1967/消耗战/1973 账、1981 红线与奥西拉克、06-08→06-09 改案、
    两小时毁 19 连、四机编队放行、"半小时约 26 架"、停火 82 架／标题 87-to-Zip、LGB"太慢没用"、两周后"四打三中"、
    "买飞毛腿"与苏联震动）＋sources 改四源。
  · `entities/people/david-ivri.md` 增"Grant 2002 专访"节＋sources/updated。
  · `concepts/bekaa-1982-numbers-four-sources.md` 增第五节 Grant 列与附：1973/1967/消耗战数字；标头改"多源"。
  · `concepts/iaf-reconstruction-after-1973.md` 增第八节（1,220 架次/50 架/4%、A-4 53/170、F-4 33/177、10-14 埃 28 架、
    战末一次损失 5 架 Phantom、SAM 庇护 SS-21）＋sources/updated。
  · `events/iaf-attrition-air-war-1969-70.md` 增第十四节（Mason 交换比 1:40→2:4，标注为转引、与全期总账不同算法）＋sources/updated。
  · `wars/lebanon-war-1982/index.md` 增"以空军司令 Ivri 的自我叙述（第五来源）"节＋sources；
    `wars/lebanon-war-1982/timeline.md` 增 06-08、06-09 内阁放行、06-11 正午三组 Grant 口径日期＋sources。
- 未改动：奥西拉克页（Grant 的"14 架"与该页既有"8 架 F-16＋6 架 F-15"其实相容，不新增内容）；Ezer Weizman 页
  （"翅膀被 SAM 折断"一语已见于既有页所引同源转述，判断后不重复加）。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；新页 YAML 有效、sources 齐、无断链；数字一律并列未择优；
  三处既有页编辑时工具报 sibling 写入，均按当前磁盘内容 patch。

### 2026-11-04（Hurley《The Bekaa Valley Air Battle, June 1982: Lessons Mislearned?》· Airpower Journal Winter 1989, pp.60—70）

- 来源：`1989_Vol3_No4.pdf`（Airpower Journal 第 III 卷第 4 期整刊，103 个 PDF 页，18 MB）·
  sha256 `aceba37b8449091d8d1cfc588e2e087fd8e4c292b5ee33d9b7c5210e7ff89934`；
  归档 `raw/articles/airpower-journal-1989-v3n4/`（pdf＋全刊 txt＋本文按页切分 txt）。
- 范围判定：本期其余各篇（Boyd 领导力、Carter 凸出部空权、Davis 军官 PME、Berkowitz 反卫星与战略稳定、
  Allard 1945—50 军种间差异、书评/索引）**与既有战争线无实质关联，未摄入**，raw 保留整刊。用户指定的
  "这本书"在库内按**一篇文章**处理（全篇 p.60—70 一次通读，无遗留段）。
- OCR：Acrobat Paper Capture；字距被插入空格、页眉页码乱码（b7=67、b'J=69、/une=June、AVVACS=AWACS、LIS=US）；
  校读项已在来源页 content_note 记明。
- 新建（2）：
  · `sources/hurley-bekaa-lessons-mislearned-1989.md`
  · `concepts/air-power-lesson-learning-critique.md`——Lambeth（敌手误学）／Hurley（己方误学）双向对读。
- 更新（3）：
  · `events/bekaa-valley-1982-air-battle.md` 增第十一节（前史、SANA 口径、技术表：APS-125／ALR-59、福克兰 27 发 25 中、
    VHF FM 30—88 MHz、EL/L-8200、RPV 激光指示、turnaround <10 分钟、F-4 600 项改装；Perroots／Eitan／Tlas 转引）＋五源标头。
  · `concepts/bekaa-1982-numbers-four-sources.md` 增第六节 Hurley 列，标头改"七个来源"。
  · `wars/lebanon-war-1982/index.md` 增"教训学习的批评（第六来源）"节＋sources。
- 未改：timeline（本文无新日期）、`entities/equipment/sa-6-2k12-kub.md`（本文无 SA-6 新参数）。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；新页 YAML 有效、sources 齐、无断链；数字并列未择优。

### 2026-11-04（《Под жарким солнцем Сирии》· Г.П. Яшкин 回忆 · 《红星报》"我们是国际主义者"项目 · 网页转载 2015-10-31）

- 来源：`Под жарким солнцем Сирии_20261104155940.pdf`（俄文，文本型排版件，西里尔完整无 OCR 噪声）·
  sha256 `94e2a29667b4897b6898e51114e3ea6a98406d2eae2c0cd41b5ee041fddf18d0`；
  归档 `raw/articles/soviet-redstar-yashkin-syria-2015/`。
- 范围：单篇回忆全文（286 行）一次通读；无遗留。
- 性质：苏方当事人（1980—1984 驻叙首席军事顾问）回忆，带宣传框架；全部战果数字为苏／叙口径。按 PRC 官方侧单源的规则处理：照录＋标口径，不合并、不裁决。
- 新建（6）：
  · `sources/yashkin-syria-krasnaya-zvezda-2015.md`（含"未提萨布拉—夏蒂拉屠杀"这一史料空白说明）
  · `events/soviet-military-advisors-lebanon-1982.md`——顾问团在 1980—1984 的行动与苏方口径（06-03 电报、06-08 Захрани 河、
    06-09 四个坦克师 100 km 正面、四天 958 架次／击落 23 架／防空毁 27 架、120 枚 Фагот、07-20 Носенко 指挥所遭遇战、
    Губкин 临时接掌第 10 机械化师、10 月莫斯科会谈、1983-12 封锁、1984-03 撤离、总参总账 16,282 人／亡 44 人）
  · `entities/people/grigory-yashkin.md`
  · `entities/organizations/soviet-231st-aa-missile-regiment.md`（仅番号与照片说明，参数一律留白，与 SA-5 页并列不等同）
  · `entities/equipment/9k111-fagot.md`（120 枚、每型 6 个基数、越野车机动反坦克排、毁坦克 150+／第 21 机械化旅 59 辆）
  · `concepts/soviet-advisors-military-assistance-model.md`（顾问／专家／作战分队三层级与四条边界）
- 更新（3）：`concepts/bekaa-1982-numbers-four-sources.md` 增第七节（叙／苏口径列，标头改八个来源）；
  `wars/lebanon-war-1982/index.md` 增"苏联顾问与叙方口径（第七来源）"节；`timeline.md` 增"苏方顾问团视角"15 条日期（含 06-05 与 06-04 的日期分歧并列）。
- 未建页：Тлас、阿萨德、Устинов 等均已在库或仅一处提及（Тлас 为叙防长且此前已有转引，本批只在新事件页随文出现，未单开页）。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；9 个新增/改动页 YAML 有效、sources 齐、无断链。

### 2026-11-04（Tlas 访谈《‘War of Liberation’》· Der Spiegel 1984-11-22 期 · 英译 Edna McCown）

- 来源：`‘War of Liberation’ A Talk with the Syrian Defense Minister_20261104160910.pdf`（文本型重排版，无 OCR 噪声）·
  sha256 `f2f02ade65937f4fa47a30b60ced232e07f260cf69198c1277916d5bf0697a6f`；
  归档 `raw/articles/tlas-der-spiegel-1984/`。
- 范围：全文 755 行一次通读，无遗留。
- 性质：叙国防部长塔拉斯战后两年半的立场访谈（宣传／自我辩护），与同日 Яшкин 苏方顾问回忆构成"两方当事人口径"。
  核报复保证一节只记"Tlas 如此宣称"，明确标注不得据此推定苏方承诺。
- 新建（4）：
  · `sources/tlas-der-spiegel-1984.md`（访谈结构、硬信息表、采访者反驳、使用纪律）
  · `events/lebanon-1982-syrian-defense-minister-interview.md`（七板块＋采访者反驳＋史料价值）
  · `entities/people/mustafa-tlas.md`（生平按访谈编者介绍；出生年标"据 52 岁推算"）
  · `concepts/syrian-strategic-doctrine-tlas.md`（"解放战争"理论：来源、三阶段、与常规军建设的张力）
- 更新（4）：`entities/equipment/sa-5-1983.md`（增叙方口径：240 km、霍姆斯—贝鲁特、指挥权、无线电连大马士革，与 Herzog 并列）；
  `concepts/bekaa-1982-numbers-four-sources.md` 增第八节（Tlas 列，标头改九个来源）；
  `wars/lebanon-war-1982/index.md` 增"叙方部长的公开表态（第八来源）"节；`timeline.md` 增 1984-11-22 条目。
- 修正记录：编辑 `sa-5-1983.md` 的 updated 时我误删了 frontmatter 结束的 `---`，已即时补回并复验 YAML 通过（8 个改动页全部 yaml True）。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；新增/改动 8 页 sources 齐、无断链。

### 2026-11-04（《موسوعة السياسة والحرب في بلاد الشام》第 3 卷 · 只摄入 1982 年战争章）

- 来源：`Noor-Book.com  موسوعة السياسة و الحرب في بلاد الشام 3 .pdf`（1109 PDF 页，叙利亚图书总局／文化部 2011；
  作者 Ibrahim Mustafa al-Mahmud 准将，序 Ali Habib 少将）· sha256 `1ba4dc00…`；归档 `raw/articles/shama-politics-war-vol3/`（pdf＋全文 txt）。
- 范围：按用户指示**仅 1982 年战争内容**——本书本章＝印刷页 366—500（PDF 页 880—1020）；
  PDF 881/1014/1023 三处章首标题（"حرب عام ١٩٨٢م"、"المنطقة بيئة استراتيجية جديدة"）。其余（古代—2006 年战争、1948—2000 各战、2006 战争、书目与附录）未摄。
- OCR：扫描件文字层存在**阿拉伯数字反转**与字距扩大；数字与专名均按上下文还原，标〔OCR〕。
- 新建（3）：
  · `sources/shama-encyclopedia-vol3-1982.md`
  · `events/sultan-yaqub-battle-1982.md`——库内**第一份叙方专章**的战例叙述：06-10 第 58 机械化旅受领任务、
    06-11 以军"精选旅"营陷入"火袋"、以军空袭打错目标（打第 81 旅后卫）、弃 8 辆 M48A5、
    叙方称毁／弃 61 辆装甲车、以军 4 死 6 伤；附本书 14 条"教训"与作者 1982-06-11 前线勘察见闻（含心理战广播细节）。
  · `concepts/lebanon-1982-force-balance-syrian-source.md`——三方兵力与阶段划分（巴解 12–14k、叙军"一个加强装甲师" 30k/300 车/300 炮、以军 169k 现役／125–150k 投入）。
- 更新（3）：`concepts/bekaa-1982-numbers-four-sources.md` 增第九节（叙方百科 vs Pollack 的直接冲突表，标头改十个来源）；
  `wars/lebanon-war-1982/index.md` 增"叙方百科：苏丹雅各布之战（第七来源）"节；
  `timeline.md` 增 8 条叙方百科日期（含 06-05 内阁决定、1982-12 末多国部队进驻——与库内 08 月口径并列）。
- 未建页：哈比卜少将（仅为序作者与专著作者，本书未给生平）；"精选旅"、第 58 机械化旅、第 622 营等仅一处提及，不单开部队页。
- 检查：SCHEMA sha256 `191cd20f…`（未变）；6 个新增/改动页 YAML 通过、sources 齐、无断链；页码已按 PDF↔印刷页实测校正。

### 2026-11-04（《الغزو الإسرائيلي للبنان》第二册 · 贝鲁特 1989 · OCR 版）

- 来源：`ocr_Noor-Book.com  الغزو الإسرائيلي للبنان 2 .pdf`，807 页扫描件（用户明示 OCR），
  sha256 `de237b2b2d41816bc1a73bce90011aca7a30abcb1e68998477001c0ec5dbbcaa`。
  作者未署名；卷首为"武装力量总司令致其战斗员"训令，按体例系叙利亚军方／官方出版物。出版批号 ١٠٨١٣，登记 1989-11-09。
  raw：`raw/articles/israeli-invasion-lebanon-book2/`（pdf + pdftotext 全文）。
- 范围：用户限定"上个世纪 80 年代有关以叙在黎巴嫩的战争"。实摄第六（贝卡空战，pp.276—317）、
  第七（贝卡地面战，pp.318—369）、第十（萨布拉—夏蒂拉，pp.516—539）三章为骨；
  第八（贝鲁特围城）、第九（政治倡议）、第十一（1980 年代后期）只取与叙军／以叙交战相关段落。
  第五章末与索引页不摄；第一册不在范围。
- 立场：叙利亚／阿拉伯官方一侧，战果只记本方；但大量直引以色列报刊与将领原话（Haaretz／Yediot／Maariv／
  HaOlam HaZeh、沙龙、艾坦、Drori、Bar Kokhva、Buis），本库均按"转引"记，未回查以方原刊。
- 新建（5）：
  - `sources/israeli-invasion-lebanon-book2.md`（含 11 条 OCR 校正表）
  - `events/bekaa-valley-1982-palestinian-account.md`（6/9 逐时时序；"战管被打瘫后 70 机对 90 机"）
  - `events/bekaa-valley-1982-beqaa-ground-battle.md`（兵力、6/6—6/11 逐日、苏丹雅各布的分散写法）
  - `events/beirut-siege-1982-palestinian-account.md`（"消耗战"三阶段、65 天推进 7 km／500 m／150 m）
  - 无新实体页：本书提及的以方人名（Eitan／Drori／Yaron／Schreiber／Buchnil）均已在库或属以方单源转引，
    不为转引开人物页；T-72 页已存在，未据本书改写。
- 更新（5）：
  - `events/sabra-shatilla-massacre-1982.md` 增第二节（PLO 口径）：38 小时、150 人、Eitan—Drori—Yaron—Hobeika
    指挥链、黎军两次拒绝（Aoun／Wazzan）、加沙医院、两段无线电通话；与 Herzog 的**共同面／冲突面**分表列。
  - `concepts/bekaa-1982-numbers-four-sources.md` 增第十节（第十一来源），并标出"70 对 90"与 Lambeth
    "90 对 60"的**互为镜像**关系。
  - `wars/lebanon-war-1982/index.md` 增"阿拉伯（PLO／叙）官方实录（第八来源）"节。
  - `wars/lebanon-war-1982/timeline.md` 增 11 条（1981-04-28/29 导弹入贝卡、06-07 Shebaa、06-08 1794 高地、
    06-08/09 夜袭、06-09 14:10 干扰、06-10 直升机机降、06-11 T-72 反攻与 12:00 停火、09-15 入西贝鲁特、
    09-16 入营、09-24 多国部队重返）。
- **顺带修库内既有断链**：`bekka-valley-war-grant-2002`（错误拼写）→ `bekaa-valley-war-grant-2002`，
  涉及 `events/bekaa-valley-1982-air-battle.md`、`events/iaf-attrition-air-war-1969-70.md`、
  `concepts/bekaa-1982-numbers-four-sources.md`、`concepts/iaf-reconstruction-after-1973.md`、
  `entities/people/david-ivri.md`、`wars/lebanon-war-1982/index.md`、`wars/lebanon-war-1982/timeline.md`、
  `sources/bekaa-valley-war-grant-2002.md` 共 8 处。此错自 Grant 批即存在，此前校验脚本按文件名反查未捕获。
- OCR 处理：阿拉伯数字未出现"反转书写"（与第 3 卷百科不同），但出现 `Howk/Hawk Eye`、`حاضبيا`→`حاصبيا`、
  `قليه`→`قليعة`、`م د`（مضادة للدروع）、章节标题空格丢失、拉丁/阿拉伯数字混排等；已在来源页列校正表。
- 待人工裁定：本书"叙军在贝卡初始兵力＝一个加强旅"与叙百科"一个加强装甲师 30,000 人"、Herzog／Pollack 的
  "师级集群"三者并列未合并；本书 T-72 反攻"压退 10 km"与 Pollack 的"叙军反攻被击退"正相反。
- **2026-11-04 补充（核原文用词后）**：两本叙方书的原词不同——第 3 卷百科（2011）作 **فرقة مدرعة معززة**（师，约 3 万人，
  语境是"在黎全境的阿拉伯威慑部队"）；第 2 册（1989）作 **بلواء معزز**（旅，语境是"开战日驻扎在贝卡的兵力"）。
  同书内 فرقة 专用于以军编成，故非笔误。百科另给：开战日仅第 1 装甲师（萨菲）满编在贝卡，另有 85 步兵旅／62 机步旅／
  51 装甲旅独立旅集群，6/11 再投入第 3 装甲师（法耶兹）。据此两说很可能不在同一层次（全境 vs 贝卡一地），
  但两书均未明说统计范围，本库仍按两种口径并列，不合并为"叙军在贝卡 3 万人"；层次判读记在
  `concepts/lebanon-1982-force-balance-syrian-source.md` 第一节小表，标"待核"。
- **补摄（同批第 5 章）**：`sources/israeli-invasion-lebanon-book2.md` 第 5 章"اجتياح جزين ومعارك الجبل"
  （PDF 页 230—274／印刷页 231—276）全文实读，新建
  `events/jezzine-and-mountain-war-1982-palestinian-account.md`：
  杰津地理与叙军"安全部署"（自承非战斗部署）、06-04/05 提高战备、06-06—09 杰津争夺（Jbaa 一个排守 3 小时、
  Hitoura、Dahrat al-Ramla）、06-08 两次海上登陆并 15:00 抵 Beit al-Din、Madayrij 节点、
  Ayn Zahlta—Madayrij 血战（00:40 白刃、09:30 Gazelle 毁 6 辆、Samqaliya 指挥所）、
  06-10 Tal Aghmid 空降与叙军脱离机动、Qabr Shmun（8 死 15 伤未失守）、
  **截获以军无线电**（"损失太大、目标无法达成"）、Bahamdoun 巷战（两批各约 50 辆坦克）、
  06-26/27 山区接触线定型；数字：以方自认 29 死 141 伤（06-24）、累计 252、七日推进约 35 km（日均 400—500 m）。
- 同步更新：`wars/lebanon-war-1982/index.md` 第八来源节新增首条；`wars/lebanon-war-1982/timeline.md`
  新增"杰津与山区之战（本书第 5 章）"19 条；来源页实摄范围表加第 5 章、"未摄"改为第 1—4、12—15 章。
- **一处并列未调和**：本书称 06-09 空袭 Samqaliya 以军指挥所，**以军副总参谋长阵亡**（称以方承认）；
  库内以方来源（Van Creveld ch17）只记前总参司长 **Yekutiel Adam**"以某种任务"进入黎巴嫩、"死因至今不明"，
  无日期、地点、军衔。两者并列，未合并，亦未据此新建人物页。

## 2026-11-18 · 来源㉙ Karlin《The Inheritance》（911 后美军机构史）

- 来源：`/mnt/share/test/The Inheritance Americas Military After Two Decades of War (Mara E. Karlin (author)).epub`
  → 存档 `raw/papers/karlin-inheritance/karlin-inheritance.epub`；
  SHA-256 `08e41516b5d890393ff4ea30be380b17bafbddb5a07d92eb656279f775919620`（库内首次摄入，无重复）。
- 提取：EPUB 本地解包（zipfile）→ 去标签、unescape、保留 spine 顺序；`karlin-inheritance.txt`（710,611 B）
  ＋`sections.json`（22 段）。未跑 OCR。文本型 EPUB，正文约 49 万字符。
- 新建（22 页）：
  - 来源页 `sources/karlin-inheritance.md`
  - 战争线 `wars/post-9-11-wars/index.md`＋`timeline.md`（**非战役线**，机构层入口）
  - 三危机 `concepts/crisis-of-confidence-karlin`、`crisis-of-caring-karlin`、
    `crisis-of-meaningful-civilian-control-karlin`
  - 概念 8 `concepts/civilian-wars-legacy-memory`、`iron-triangle-painful-tradeoffs`、
    `department-of-defense-ad-hockery`、`post-9-11-war-funding-open-bar`、
    `all-volunteer-force-family-business`、`accountability-soup-karlin`、
    `personalization-of-casualties`、`post-9-11-theories-of-victory`、
    `by-with-and-through-partnerships`、`sof-and-drones-post-9-11`（共 10 个概念页）
  - 事件 1 `events/post-9-11-war-planning-failure.md`（过程事件：war planning 2001—2009）
  - 军种 4 `entities/organizations/us-army-post-9-11`、`us-marine-corps-post-9-11`、
    `us-air-force-post-9-11`、`us-navy-post-9-11`
  - 专题 2 `topics/post-9-11-wars-legacy`、`topics/post-9-11-military-manpower`
- 更新（4 页）：`index.md`（战争入口加 911 后线＋来源㉙）；`wars/iraq-war-2003/index.md`
  （新增"美方视角（并列来源，不合并）"节、sources 加 karlin）；`wars/gulf-war/index.md`
  （新增"海湾战争作为遗产的读法"节、sources 加 karlin）；本 log。
- 未更新：`wars/iran-iraq-war-1980-88/*`、Pollack 各页——本书不涉两伊战争与阿拉伯军效能，无实质新增。
- 口径与纪律（已写入来源页与相关页）：
  1. 本书为**近百人匿名访谈**（2018—2020，以将官为主＋少量文官），无脚注的引号句即访谈原话；
     全部引语在本库标〔Karlin 访谈〕，**不当作多源证实的事实**。
  2. 所有数字（$1.5 万亿／$6 万亿、战斗机 −50%、316/278/308 舰、46,000 水兵、6,000 in-lieu、
     80% 伤亡由路边炸弹造成、无人机 473 次打击等）均为**本书转引**，来源页已注明"原始表未见"。
  3. 时间下限约 2021 年初；**阿富汗撤军（2021-08）及其后不在本书范围**，不得挂本书。
  4. 本书弃用 GWOT／Long War／Forever War 等称呼，本库沿用其"post-9-11 wars"定义（含约 40% 国家的作战/部署）。
- 与其他来源的关系：与 [[sources/malovany-wars-of-modern-babylon|Malovany]]（伊方视角）、
  [[sources/arabs-at-war-pollack|Pollack]]（阿拉伯军效能）三角并列，**框架不同、不合并**；
  方法上与 [[sources/idf-van-creveld-sword-olive|Van Creveld 的 IDF 机构史]]最近。
- 异常／待核：
  - 出版信息：EPUB 版权页仅存"THE BROOKINGS INSTITUTION … Washington, D.C. 20036"，**无年号**；
    出版年 2022 为推定，标待核。
  - Brief Chronology 与正文日期冲突：2010 年伊拉克作战结束，年表作 2010-08-30，正文另处作 2010-06-30；
    两说并列于 `wars/post-9-11-wars/timeline.md`。
  - ch4 第 110—138 行、ch5 第 155—165 行（PRT 后半）、ch8 第 168—210 行（伦理）**跳读未逐字**；
    `notes.xhtml`（15.6 万字符）未提取；Figure 5-1／6-1、Table 6-1 三处图表数据仅存图题。
- 检查：22 个新页 YAML 全部可解析（3 页 `title` 内含双引号，已按库规改用「」；1 处表格内 `\|` 转义链接
  会造成假断链，已改为纯文本）；新页断链 0；`SCHEMA.md` 未改动；raw 原件与提取文本已保存。
- **顺带修复（存量缺陷，非本批引入）**：全库扫描发现 9 个旧页 frontmatter 无法被 YAML 解析，原因两类——
  (a) 未加引号的标量值里含英文 `: `（`sources/arabs-at-war-pollack.md`、`sources/us-electronic-warfare-history-vol1-price.md`、
  `…vol2-price.md`、`sources/yom-kippur-war-rabinovich.md`、`entities/people/ingwald-haugen.md`）；
  (b) `title` 用**英文双引号包裹内层引号**（`"蓝军与绿军"：…`），引号提前闭合
  （`concepts/plan-d-1948.md`、`iaf-blues-vs-greens.md`、`yonay-sources-and-methodology.md`、
  `scripted-vs-unscripted-warfare.md`、`iaf-six-theses-yonay.md`）。
  已按本库既有约定处理：含 `: ` 的值整值加引号；标题内层引号改为「」或改用 `——`。
  **正文一字未改**，仅动 frontmatter 该行。修复后全库 0 个 YAML 解析失败。

## 2026-11-18 · 来源㉚ Hallion《Storm Over Iraq: Air Power and the Gulf War》（空军视角的海湾战争）

- 来源：`/mnt/share/test/Storm Over Iraq Air Power and the Gulf War Smithsonian History of Aviation Series
  (Hallion, Richard P).epub` → 存档 `raw/papers/hallion-storm-over-iraq/hallion-storm-over-iraq.epub`；
  SHA-256 `cc66d70fa9d85e6b7b121810fc8c4e8f68822b41238cb6dbaa54f176d87ddb55`（库内首次摄入）。
- 提取：EPUB 本地解包（zipfile）→ 去标签、unescape、保留 spine 顺序；`hallion-storm-over-iraq.txt`（949,500 字符）
  ＋`sections.json`（36 段）。未跑 OCR。文本型 EPUB（7.98 MB）。
- **版本注意**：版权页署 1992（ISBN 1-56098-190-3／1-56098-723-5，eBook 978-1-58834-519-6），
  但 EPUB 的 Preface 自述"距海湾危机已过十年"并讨论 1994 年卢旺达、1995 年波黑"审慎力量"、1999 年科索沃
  "盟军力量"，系 2001 年前后的重印前言。引用时须区分"1992 年正文"与"后加前言"。
- 新建（14 页）：
  - 来源页 `sources/hallion-storm-over-iraq.md`（含"立场与史料性质""引用注意"两节）
  - 概念 7：`concepts/air-power-legacy-hallion`（ch1，含一战/二战/原子时代/越南/中东五段）、
    `air-combat-training-revolution-post-vietnam`（ch2、ch4）、`airland-battle-and-31-initiatives`（ch3）、
    `precision-strike-revolution-hallion`（ch6—ch7、附录）、`parallel-warfare-warden`（五环＋DMPI＋并行战）、
    `bda-and-intelligence-gulf-war`（ch7、ch8）、`air-power-decisiveness-debate-1991`（ch8 五问五答）
  - 概念 1（双源）：`concepts/weinberger-powell-doctrine.md`——Hallion 记起源与六条标准，Karlin 记 911 后回潮与批评，
    **两书立场相反，页内并列不调和**
  - 事件 5：`events/desert-one-1980-eagle-claw`、`events/desert-shield-airlift-1990`、
    `events/instant-thunder-1990-08`、`events/desert-storm-air-campaign-1991`、`events/scud-hunt-1991`
- 更新（8 处）：`wars/gulf-war/index.md`（新增"空军视角（第六来源）"整节＋sources＋战争入口描述改为六来源）；
  `wars/gulf-war/timeline.md`（增补 40 余条〔Hallion〕口径节点，frontmatter sources/updated 同步）；
  `events/desert-storm-opening-night.md`、`events/iraq-1991-desert-storm-air-war.md`、`concepts/sead.md`、
  `concepts/iraq-1991-coalition-war-pollack.md`、`entities/equipment/f-117a-have-blue.md`、
  `concepts/air-power-lesson-learning-critique.md` 各加"并列来源：Hallion"节（只加链与口径提示，不改正文）；
  `index.md`（新增"空中力量专题"入口＋来源㉚条目）。
- 口径纪律（已写入来源页与各页）：
  1. 本书是**公开的空军主张书**，非中立战史；作者自陈"非常个人化的战争观，不试图代表任何官方机构"。
  2. 所有战果/损失数字（F-117 命中率 79%、联军损失 42 架、空军损失率 0.00047、伊军坦克 90% 被毁、
     空战 35:0、飞毛腿发射 93 枚、首夜 668 架、首日 535 架次打 31 处核生化设施等）标〔Hallion〕。
  3. **"爱国者拦截率 96%"** 与库内 Van Creveld 的"几乎拦不中"**并列不合并**；本书自己也承认
     "后来研究对 96% 提出疑问"，但未给替代数字。
  4. "空权赢得了海湾战争"这一核心主张，与 Pollack／Malovany 的伊军侧解释并列；本库不裁断。
- 异常／待核：
  - **五环框架**：首次快速检索未命中 `five rings` 字样而误写"本书未复述五环"，**随后全文复核确认书中 ch5 明写
    "Warden's concept of the Five Strategic Rings"**，已据此重写 `concepts/parallel-warfare-warden.md`
    （含五环五项、DMPI 分配法、Deptula 的"打一处瘫一栋"论证）。已删除一度误建的占位页。
  - Table 4.1／5.1／5.2／6.1／6.3／8.1 六处统计表在 EPUB 文本中仅存表题与正文引述，表格数据未解析。
  - `notes.xhtml` 尾注（约 13.6 万字符）与 Index 未提取；引用具体脚注须回 raw 核对。
  - 未逐字精读的段落：ch1 二战小节后半、ch2 导弹技术小节、ch4 利比亚/巴拿马中段、ch5 后半（部队进驻与
    伊拉克军力清单已读）、ch8 航母与陆战队两节中段。列为"未完整覆盖"，日后如需可补读。
- 检查：14 个新页 YAML 全部可解析（含 2 页含 `\|` 转义链接，已按库规改写为 `[[a]]（b）`，避免表格内假断链）；
  新页断链 0；`SCHEMA.md` 未改动；raw 原件与提取文本已保存。

## 2026-11-18 · 来源㉛ Putney《Airpower Advantage: Planning the Gulf War Air Campaign, 1989—1991》

- 来源：`/mnt/share/test/AirpowerAdvantageSoftcover.qxd.pdf`（497 页，PDF 1.7，数字文本层）
- SHA-256：`e79473a24af6f381023514c19933da4b5554e815cae8f03e0128db152be4e09a`
- 提取：`pdftotext -layout` → `raw/papers/airpower-advantage-cohen/airpower-advantage-cohen.txt`
  （1,597,784 字符，保留分页符）；未 OCR。
- 性质：**美国空军官方史**（Air Force History and Museums Program，2004），
  解密档案＋规划人员访谈；不写战果，战斗执行只在末章用首日 24 小时作样本。

**新建 9 页**

- `sources/putney-airpower-advantage.md`（含章—行号对照、史料性质、口径冲突清单、未提取范围）
- 概念 5：`jfacc-and-tacc-gulf-war`、`warden-five-rings-and-targeting`、
  `targeting-for-effects-and-parallel-warfare`、`counterland-attrition-50-percent`、
  `gulf-war-intelligence-support-failure`
- 事件 3：`opled-100290-and-internal-look-1990`、`warden-briefs-horner-1990-08-20`、
  `desert-storm-first-24-hours-1991`

**更新 7 页**

- `wars/gulf-war/index.md`：新增「计划层（第七来源）」整节；sources 加 putney
- `wars/gulf-war/timeline.md`：新增〔Putney〕口径 30 余条计划层节点；sources 加 putney
- `events/instant-thunder-1990-08.md` · `events/desert-storm-air-campaign-1991.md` ·
  `events/desert-storm-opening-night.md` · `concepts/bda-and-intelligence-gulf-war.md` ·
  `concepts/parallel-warfare-warden.md`：各加「并列来源：Putney」节，只加链与口径提示，
  sources 追加、正文未改
- `index.md`：新增「海湾战争计划层（USAF 官方史）」入口＋来源㉛ 条目

**跳过 / 未逐字**

- Glossary、Bibliography、Notes（p.383—460）、Index 未提取
- 插图 40 余张与作战图表仅存图题，不据图判读
- 跳读：ch3 后段、ch4 中段、ch7 后段（Bush 简报与欺骗计划）、ch9 大部分
  （人质营救、PSYOPS、欺骗、目标开发各节）

**异常与处理**

- 文件名 `AirpowerAdvantageSoftcover.qxd.pdf` 的 "qxd" 与库内 slug 不符，slug 定为
  `airpower-advantage-cohen`（沿用文件目录，未改文件名）；书名页核对为 Diane T. Putney。
- 排版核对中发现 wiki 内 `events/opled-100290-and-internal-look-1990` 一处链接误写
  `opl100290-...`，已修正。
- 首次给 timeline frontmatter 追加 sources 时误插入注释行，已用 patch 撤回。

**检查**

- 新页 YAML 0 问题；新页断链 0
- 全库 711 个 md：YAML 仅 SCHEMA.md／log.md 无 frontmatter（符合设计）
- 全库断链 7 处，全为存量（SCHEMA 示例占位符 `wikilinks`／`PAGE n`／`a`、
  `operation-bolo`、`chermon-missouri-final-battles-1973`、`entities/people/avner-halutz`），
  与本次摄入无关
- `SCHEMA.md` sha256 前缀 `191cd20f951e` 未变

## 2026-11-18 · 来源㉛ 批次二：补读 ch7 / ch9 / ch10（Putney）

- 背景：批次一（计划层骨架）跳读 ch7 后段与 ch9 大部分即建了情报页，属批次合并失误。
  批次二补读：ch7 全章（Dugan 事件→Gorilla Package→Poobahs Party→情报支援抱怨→
  Phase I 目标扩张→NBC 目标→Task Force Normandy）、**ch9 全章**（Reflex、Scud、
  人质营救、McConnell—Glosson 链路、MIB 调查、目标材料、BDA 四难、规划者—情报官摩擦、
  海军/陆战队/陆军/沙特/英国五组摩擦、欺骗、PSYOPS、领导层与 C3、BW 再议、Proven Force）、
  ch10（四阶段总汇报、CENTAF 两次改组）。

**新建 4 页**

- `events/dugan-affair-1990-09.md`——空军参谋长因向记者谈"打萨达姆本人"被解职；
  Horner"是我们的人要因此去死"、Warden 问 Dugan 是否故意泄密、Dugan 的元帅军衔法律论证
- `concepts/gulf-war-deception-and-drones-1990.md`——BQM-74C"Poobahs Party"
  （44 架、18 套发射器、第 868 战术导弹训练大队→第 4468 战术侦察大队、
  架设时间 9.5h→1.5h、前 31 小时 10 个无人机包）、两级作战欺骗、Burning Hawk 的官僚窒死
- `concepts/nbc-targeting-and-bw-debate-1991.md`——"打也不是、不打也不是"：
  百万级伤亡预测、超级胶等荒唐方案、Fort Detrick 少校与阳光、1990-12-20 决策、
  F-117+CBU-89 黎明攻击方案、Abu Ghraib 奶粉厂、CW 8→16 与 35 个目标
- `events/gulf-war-campaign-planning-1990-10-to-1991-01.md`——Reflex 预案（3 枚测试飞毛腿触发）、
  Scud 问题（500—700 枚/36 部 TEL/64 固定位；Horner"军事上不重要"的自陈）、
  Touted Gleem 结果不佳、以色列方向（Hammer Rick、拒绝爱国者、扣住 IFF）、
  五组摩擦（海军 CAP/A-6/BVR、陆战队 HARM 300、陆军 JSTARS 与破障、沙特 CSS-2、
  英国丢失计划文件）、1990-12-20 四阶段总汇报（1,316 架、238 目标、32 天、Warden 的 146 架损失预估）、
  **战后分析未把共和国卫队削到 50%**

**更新 3 页**

- `sources/putney-airpower-advantage.md`：改"未逐字"清单为"2026-11-18 补读（批次二）"；补批次二页清单
- `concepts/gulf-war-intelligence-support-failure.md`：新增「ch9 补读后的追加」七小节
  （Whitley 书面抗议与 Horner 正面对立、MIB 调查含 SR-71 建议、McConnell—JIC 链路与
  "他满足于自己是唯一受益者"、Talbot 的互不信任诊断、Glock 常驻、Christon 战后总结）
- `concepts/bda-and-intelligence-gulf-war.md`：新增「BDA 的四个结构性难题」七小节
  （ARCENT 无方法、DIA 三相与 ring-down 之弊、判读技艺消亡与 GBU-27 单独保密、
  按效果评估加大难度、卫星不够分、平台限制、Schwarzkopf 禁令）
- `wars/gulf-war/index.md`、`index.md`：入口补 4 页

**仍未逐字**

- ch3 后段（Desert Storm Phase I 的逐目标叙述）、ch4 中段（CENTAF 防御性空中战役、
  ATF/ATO Bravo 概念）、Notes（p.383—460）、40 余张图表

**检查**

- 新页 YAML 0 问题、断链 0；全库 715 个 md，YAML bad 0
- `SCHEMA.md` 未改动

## 2026-11-18 · 来源㉛ 批次三：Glossary / Bibliography / Notes（Putney）

- 读取：Glossary（p.363—366，全文）、Bibliography（p.367—382，全文单栏，质量良好）、
  Notes（p.383—460，**双栏排版，pdftotext 提取后两栏逐行交错，无法按条目重排**）。
- 处理：不做逐条抄录（技术上不可能），改为**统计＋分层判断**，产出 1 个史学专题页。

**新建 1 页**

- `topics/putney-airpower-advantage-source-base.md`——Putney 的史料解剖：
  - **层一 访谈**：约 70 位受访者，四个承接机构（CADRE/AU、AFHSO、AFHRA、各司令部史办）；
    被访频次（本库统计）：Deptula≈410、Horner≈290、Harvey≈192、Glosson/Warden≈175、
    Glock≈104、Schwarzkopf≈92；**Warden 的访谈由 Putney/Davis/Jamieson/Hallion 四人共同进行**
    ——解释了本书与 Hallion 书在材料上的亲缘关系
  - **层二 GWAPS 未刊采集件**：尾注 GWAPS≈502 次、NA 文献编号 48 处、microfilm frame/reel 91 处；
    另有 Mandeles file、Col Warden's Notes、CSAF Notes 14 Aug、Meilinger/Stanfill 笔记、
    Kuehl「Notes on Instant Thunder」、AD Fact-Finding 报告
  - **层三 一手文书**：USCINCCENT/USCENTAF/DO/DOX 电文、Horner 1990-04 的 OPLAN 100290 空中行动简报
    （逐页引用）、100290 两版草案、AFM 1-1／FM 100-5 三版／USCENTAF Reg 55-45 等条令、
    单位史与 GWAPS NA 研究报告
  - **层四 学术文献**：列出与本库直接相关的 12 种（Warden 1988、Mets 1998、Belote 1999、
    Davis 2002、Andrews 1998、Reynolds 1995、Mann 1995、Frostic 1994、Winnefeld 1994、
    Pape 1996、Record 1993、Summers 1992）
  - **证据强度分层表**（文书日期=高／会议内容=中高／引语措辞=中／数字=中且为计划值／
    对他人的评价=低），并定引用纪律：访谈引语须标〔据 Putney 转引访谈〕
  - **Glossary 的库内用处**：D-day/G-day/H-hour 三者区分（地面战役／战略空中战役）；
    counterland 是作者自选术语，1990 年 AFM 1-1 无此任务分类，1997 年才入条令（溯及尾注第 35 条）；
    GAT = Guidance, Apportionment, and Targeting

**更新 3 页**

- `sources/putney-airpower-advantage.md`：补「史料基础」指向与「批次三」读取说明
- `wars/gulf-war/index.md`：新增「史学与史料（专题）」入口
- `index.md`：入口补该专题页

**异常**

- Notes 的双栏交错是**提取工具层面**的缺陷（`pdftotext -layout` 对双栏无解），非源文件问题；
  已在来源页与专题页两处写明「具体脚注须回 PDF 按页核对」，并把统计口径标为 ±10%。

**检查**

- 新页 YAML 通过、断链 0；全库 716 个 md，YAML bad 0
- 全库断链 7 处，全为存量（SCHEMA 示例占位符 3 处、log 中 3 处、jezzine 页 1 处）
- `SCHEMA.md` 未改动

## 2026-11-18 · 来源㉜ Woods《The Mother of All Battles》（伊拉克政权层，缴获档案）批次一

- 来源：`/mnt/share/test/The mother of all battles  Saddam Husseins strategic plan for the Gulf War
  (Woods, Kevin M) (z-library.sk, 1lib.sk, z-lib.sk).pdf`
- SHA-256：`73306848a2d7135adb852353b507ab89dd8df17846b7a46e77d32fd788a6c5bf`
- 提取：`pdftotext -layout` → `raw/papers/woods-mother-of-all-battles/woods-mother-of-all-battles.txt`
  （1,020,924 字符）；**Internet Archive Scribe 扫描 + OCR 层，未重跑 OCR**。
- 书目：Naval Institute Press，2008，ISBN 978-1-59114-942-2，LoC DS79.724.I72 W66 2008。
- 性质：**Iraqi Perspectives Project**（JCOA/JFCOM 资助，JAWD/IDA 出版）；
  材料为 2003 年 OIF 缴获的伊拉克总统办公室、军事、情报记录与萨达姆会议录音录像
  （DIA Harmony 数据库，尾注以 ISGQ-2003-M00xxxxx / ISGP-2003-xxxxxxxx 标注）。

**OCR 状况（本批重点核查）**

- 正文识别率约 98% 以上，可正常引用。
- **目录页（p.v—x）几乎完全乱码**，无法据目录定位章节；已用页眉行号分布重建章目，
  写入来源页（起点准确，页内边界可能 ±1 页）。
- 图表／地图／照片页为图像＋噪声，**仅存图题，不据图判读**。
- 典型误识：`Irag`/`Iraq`、`Tragis`/`Iraqis`、`SS.`/`U.S.`、`XVII`/`XVIII`、
  元数据 LoC 号 `DS79.724.172` 实为 `I72`。专名罗马化**按书中形式照录，不归一化**。

**本批读取范围**：Preface（p.xiii）、A Note on Sources（p.xv）、Introduction（p.xix）、
ch1（美方视角概览，p.1—30）、ch2（Saddam's Narrative，p.31—46）。

**新建 3 页**

- `sources/woods-mother-of-all-battles.md`——书目、OCR 状况与常见误识、章—行号对照、
  史料性质四属性（不完整／无法估计损失比例／嵌着精心记录的谎言／叙事天然失衡）、
  翻译层失真（Sharabi、Lewis）、引用纪律、与 Malovany 的层级分工
- `concepts/saddam-pan-arab-strategic-vision.md`——"阿拉伯帐篷的中央支柱"、
  "长期战争"论与十二个月五万伤亡预算、加利利海与原子弹推演、象年寓言（伊朗=波斯、
  美国=拜占庭、以色列=阿比西尼亚、叛徒=现代阿拉伯国家）、"海湾阿拉伯人是腐朽的阿拉伯人"、
  1979 年对科威特的预言式表述、两伊战争是手段非目的、Barzan 1989-09-04 密信五要素
- `concepts/two-wars-narrative-asymmetry-1991.md`——"仿佛在描述完全不相干的事件"、
  海夫吉与撤离科威特的分叉、"联军视角充其量只有一半正确"、联军基线的三处高估
  （伊军能力／精确弹药对装甲／中空轰炸代价）、四个研究用途（批判分析／历史准确性／
  红队／适应）、以及"巴士拉坦克纵队长当众斥责萨达姆"与"萨达姆自认赢家"并存于档案

**更新 3 页**

- `wars/gulf-war/index.md`：新增「政权层（第八来源）」节；sources 加 woods
- `index.md`：新增入口与来源㉜ 条目
- （未改 `log.md` 以外的既有正文）

**待读**：ch3（战略算计，1990 春—夏）、ch4（Restoring the Branch，含入侵与共和国卫队闪击）、
ch5（占领与巩固）、ch6（科威特防御计划）、ch7（万物之母之战，约 5,400 行，最长）、
ch8（萨达姆的战后教训）、ch9（Epilogue）、Notes。

**检查**

- 新页 YAML 通过、断链 0；全库 719 个 md，YAML bad 0
- 全库断链 7 处，全为存量（SCHEMA 示例占位符 3、log 3、jezzine 页 1）
- `SCHEMA.md` sha256 前缀 `191cd20f951e` 未变

## 2026-11-18 · 来源㉜ Woods 批次二：ch3（战略算计）+ ch4（入侵计划与执行）

**读取范围**：ch3（p.47—59，行 2620—3320）、ch4（p.60—92，行 3320—4605）。

**新建 2 页**

- `concepts/saddam-kuwait-decision-1990.md`——决策层：
  "档案里没有决定时刻"（compartmented 决策风格）、与 1979 年对伊朗同构的逻辑、
  经济数字（油价每桶每跌 1 美元＝年损 10 亿；最后要求 24／120／100 亿＋布比延岛租借）、
  al-Duri"你在逼我杀你"、埃米尔的"夏日云彩"、Glaspie 两种读法并列、
  1990-04-19 阿拉法特录像会谈（"准备好与美国作战""派绑炸弹的人去华盛顿""当我们抵抗时让我们成为野兽"）、
  1990-08-04 对也门总统（"科威特是伊拉克的土地""如果他们不付我们就打他们"）、
  1990-08-07 部长会议逐人发言（无人质疑正当性，只讨论合并方案与阿尔萨斯-洛林先例）、
  1990-08 复兴党招待会（第二次卡迪西亚的"合法孩子"）
- `events/project-17-iraqi-invasion-plan-1990.md`——作战层：
  al-Rawi 受命、总参谋长 al-Khazraji 不知情、GMID 五份研究（**07-25 已预警"美国会干预"**）、
  Hamdani 宣誓保密、160 公里装甲突进、只打榴弹不打穿甲弹的自我约束、
  过期 1:100000 地图与"用旅游地图打科威特城"、三叉突击与三个战斗军团、
  两伊战争三条经验（预备步兵旅／保温水箱／130mm 照明弹推进，20→40 km/h）、
  空军四次 MiG-25 侦察得 800 余幅图像、海军 36 小时通知与"以色列行动"掩护故事、
  08-02 海军实况（故障、俄国专家、螺旋桨撞礁、俘获基地司令时骗其"这是演习"）、
  1990-07 部队规模表

**更新 3 页**：来源页（已读／未读范围）、`wars/gulf-war/index.md`（政权层节补 3 页）、`index.md`（入口补 2 页）

**本批的三个重要并列点（不裁断）**

1. **07-25 GMID 研究报告已写明"美国已声明会干预"**，与"Glaspie 绿灯说"构成张力；
   Woods 未裁断，本库并列（误判说 vs 知情下注说）。
2. **Hamdani"对科威特人无敌意、只打榴弹"属单方战后回忆**，与科方／联军记录的伊军暴行不一致，
   照录但标为自述。
3. **1990-08-07 部长会议是入侵后记录**，发言有迎合动机，不能当战前共识证据。

**检查**：新页 YAML 通过、断链 0；全库 YAML 无新增错误；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉜ Woods 批次三：ch5（占领与巩固）+ ch6 前半（科威特防御计划）

**读取范围**：ch5（p.93—123，行 4605—5878，读了其中约 90%）、
ch6 前半（p.124—137，行 5878—6290，至"海军防御"一节）。

**新建 2 页**

- `events/iraq-occupation-of-kuwait-1990-91.md`——占领：
  组织（al-Majid 任省长、Sabawi 管安全、Taha Ramadan 管掠夺、国防部"道德指导局"印
  《科威特伊拉克化手册》）、al-Majid 的占领方针、**Sabawi 自述的处决与集体惩罚**
  （"严厉对待，然后杀掉、埋掉"；al-Fuhud 28 人全杀；一发子弹打整个街区；
  当众处决后烧房；换身份证或失去全部公民权利）、国家组织的掠夺（400 辆卡车、
  1.5 万吨大麦、萨达姆指定 Taha Ramadan 负责）、早期混乱的伊方内部备忘录、
  人民军与"不受欢迎的军队"、人口降 60%、11-24 命令里那句"盗窃者将被处决"、
  萨达姆战后"悔意"（为军队廉正受损，不为暴行）、
  阿盟分裂与 08-12 挂钩提议、致拉夫桑贾尼的信废掉八年战争理由、
  800 名人质与"客人"政策、萨达姆论联合国"是布什的组织"、
  普里马科夫来访与"强大伊拉克是地区平衡所需"、时间感的正面对撞
- `concepts/iraqi-kuwait-defense-plan-1990.md`——防御：
  **没有入侵沙特的严肃计划**（共和国卫队两师无后勤）、35 个师"河豚式防御"、
  GMID 八份威胁评估（08-08 至 08-29，均不缩小挑战）、
  西方报章是"最准确情报来源"、**全国只有 16 张过期沙特地图**、侦察纵深 40 公里、
  萨达姆"没想到空袭持续一个半月"、"好战士是蜷起来抱住武器的人"、
  疏散与伪装原则、500 辆废坦克作假目标、烧油生烟到 500 米、
  反巡航导弹科学会议、避卫星演练、禁止使用电话、
  **实弹靶场与"抵抗与自由演习"（1990-12-19）**、al-Faw 掩体工程（250 磅标准）、
  "战前空中轰炸"一词的政治含义、海军 1,300 枚水雷七个雷场

**更新 3 页**：来源页（已读／未读范围）、`wars/gulf-war/index.md`、`index.md`

**本批的重要并列点（不裁断）**

1. **"毁伤百分比非常低"是伊拉克自办实弹试验的结论**，Woods 已指出参与试验的将军
   与士兵在掩体中的利益不一致。本库保留该批评，同时注明：掩体保人 ≠ 空袭无效。
2. **al-Faw 掩体按承受 250 磅炸弹直击设计**，与联军实际使用的 2,000 磅级钻地弹
   不在一个量级（本库观察，书中未明说）。
3. 占领罪行部分全部出自**伊方自己的会议录音与文件**，引用须标〔据 Woods 转引，Harmony 档号〕，
   不得改写成第三方指控。

**检查**：全库 723 个 md，YAML bad 0；断链 8 处（新增 1 处为自身笔误
`irawi-kuwait-defense-plan` → 已修为 `iraqi-kuwait-defense-plan`，其余 7 处为存量）；
`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉜ Woods 批次四：ch6 后半（防御概念、11-18 转向、空军与防空军、导弹）

**读取范围**：ch6 后半（约 6290—7000 行，p.135—150），至导弹部队一节前半。

**新建 3 页**

- `concepts/iraqi-ground-defense-concept-1990.md`——作战构想：
  萨达姆"地面战将是常规战"的假设、城市战被强调但没准备（Hussein Kamel 任军长）、
  前推防御与"1939 年马奇诺心态"、第 5 机械化师"机动一号计划"（三次"不惜代价"）、
  对敌方情景的判断（两路纵队＋Mutla 岭空降，与美军"一个军计划"接近）、
  **1990-11-18 战略转向**（六条指示原文，含"在敌人的计算里制造恶性循环"与
  "古典式计算保证了对手单方面优势"的自我批评、从前线收缩换纵深与预备队）、
  第三军的实施（前推阵地削减近半、假坦克换真坦克）、11-22 增派七个师、
  12-08/13 破坏命令与油沟点火演练、共和国卫队三种任务与三份反击方案、
  **11-23 沙盘会议**（陈述"没有说服力"、多数人按伊朗框架答、Hamdani 的间接路线被孤立）
- `concepts/iraqi-air-force-pre-war-assessment-1990.md`——空中力量：
  入侵后语气急转、"保存力量"为规划主线、自评 **1:4／1:8／1:12**、
  八项作战构想（打海水淡化厂判定"经济上毫无价值"并自承损失 50%
  ——**自我否决**；反航母方案 30 架出动 12 架到目标无一返航"无效"；
  "66 号任务"；逃伊朗"几乎没有预谋"）、防空军七项优先配置与第五防区（科威特）、
  "防空兵是政权常规防御的阿尔法与欧米伽"（1991-01-17 02:30 与 2003-04-08 16:00 两份电报）
- `concepts/oil-as-weapon-project-tariq.md`——塔里克工程：
  1990-09-17/18 首次讨论、拉希德委员会、**首要目的是烟幕掩护不是污染**、
  三项任务（部队前方／海岸与布比延岛／海上油污）、
  A 部分岸基泵站＋"工业岛"、B 部分五艘油轮 53.5 万吨与改装泵、
  12-13 油沟试验（火焰 50 米、烟 400—500 米）、1,300 枚水雷七个雷场 60% 已布设

**更新 3 页**：来源页、`wars/gulf-war/index.md`、`index.md`

**本批重要判断（不裁断）**

1. **塔里克工程证明"烧油田"是 1990 年 9—10 月就成案的有代号方案，不是 1991 年 2 月溃退的临时破坏**；
   但本库**不断言**纵火是萨达姆一开始就下的令，实际点火的下达依据待 ch7。
2. **空军自我否决"打海水淡化厂"** 与西方常见的"伊拉克意图以水厂胁迫"叙述张力明显，并列记录。
3. **陆军过度自信 vs 空军清醒** 是本书内部的真实差异，不简化为"整个政权自欺"。
4. **11-18 战略转向**是本批最有史料的发现：伊军战前已知前推防御会被绕开，
   试图改纵深防御，**但迟了**（11-18 下令、11-22 增派七个师，联军西翼回旋正是为此）。

**检查**：全库 726 个 md，YAML bad 0；断链 7 处全为存量；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉜ Woods 批次五：ch7 前半（1 月 13 日—1 月 23 日）

**读取范围**：ch7（Um Al-Ma'arik）前半，p.172—191，约 7942—8600 行。

**新建 2 页**

- `events/um-al-maarik-iraqi-air-war-1991.md`——战役前半（至 1 月底）：
  战前"许多政治与军事领导人 99.9% 确信战争不会开始"；
  1-13 幕僚会议十项内容（水雷"放蛇"、**塔里克工程预授权给当地指挥官**、
  国旗写"真主至大"及其理由"有了这些话它就不能被不尊重了"、纽约—巴格达时区误解、
  1987 年"决战年"的玩笑、海军被公开看不起、运输机 1 月初送伊朗、
  库尔德语／土耳其语通信构想、指挥官乘车换车的防护建议）；
  **1-17 02:00 Task Force Normandy 与"无线电静默保证了报告没到巴格达"**；
  Hamdani 的 0245 回忆；**0420 破坏 al-Wafrah／al-Burqun 油田命令**；
  萨达姆在防空作战中心"关心的是不要反应过度"；03:50 与 11:00 的导弹命令原文；
  **Project 777 的"17 天"**（伊方单方面说法）；
  **13:34 塔里克工程启动 → 800 万桶原油入海**；
  1-18 八枚导弹打特拉维夫海法、发射车循环；1-19 电子战命令原文
  （"不是买密码机，而是停止所有通话"）与手写密件的由来、1,800 枚炸弹仅损 1 人；
  1-20 导弹效果报告与第三军越境袭击；**1-21 从"防御"转向"存活"**
  （"敌人正计划缩短这场我们打算延长的战争"→ 缩减弹药 → 士气崩溃、
  第 25 步兵师用骆驼运补给、al-Majid 说弹药节约反而提高了联军效能）；
  1-22 拆机器；1-23 Hamdani 失去两个高炮连
- `concepts/iraqi-failure-to-read-coalition-westward-swing-1991.md`——
  **1-23 GMID 十项敌方方案评估**（全条合理、结论全错，"第七军是预备队"是致命误判）、
  Woods 的诊断"试图让情况符合先入之见"与"2003 年作战瘫痪的预演"、
  三层原因（40 公里侦察纵深与地图灾难／两栖欺骗成功／伊朗框架的先入之见）、
  Hamdani 在 11-23 沙盘会议上被孤立的预测、**与 Putney 情报失败页构成同一问题的两半**

**更新 3 页**：来源页、`wars/gulf-war/index.md`（新增"战争进程"节）、`index.md`

**本批关键结论**

1. **纵火有令**：**0420** 破坏 al-Wafrah／al-Burqun 油田（陆上）、**13:34** 塔里克工程启动（海上）。
   与批次三、四的"方案—预授权—执行"链条闭合，**不再是"溃退失控"的模糊说法**。
2. **1-21 是伊军崩溃的转折点**：从"防御"改为"存活"、缩减弹药，直接导致士气崩溃——
   **这是伊拉克人自己战后的分析**，不是联军侧的判断。
3. **1-23 的十项评估**是本库最好的"情报充分但框架错误"案例，
   与 Putney 记录的"情报送不到"合成完整图景。
4. **Project 777 的"17 天"**为伊方单方面说法，与联军侧记录不合，**并列不裁断**。

**检查**：全库 728 个 md，YAML bad 0；断链 7 处全为存量；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉜ Woods 批次六：ch7 中段（1 月 24 日—2 月上旬）

**读取范围**：ch7 中段，p.189—205，约 8600—9250 行。

**新建 4 页**

- `events/iraqi-aircraft-and-ships-flee-to-iran-1991.md`——
  **1-26 萨达姆亲自下令**（18 Mirage＋9 Sukhoi＋1 Falcon-50 起）"为了安全保管，
  直到适当的时机到来再把它们用于对付敌人"；2-13 空军日志里"派四名 Su-25 飞行员
  连同护照去伊朗办手续"；**137（伊方情报）vs 22（伊朗承认）**；伊朗落地即刷涂装；
  1-29 夜海军冲向 Bandar-e-Khomeini：9 艘出发（4 导弹艇、3 登陆驳船、炮艇、扫雷舰）、
  230 公里、无导航雷达无无线电、6 艘沉没、3 艘抵港、
  **20 人死亡（7 名将军＋13）、68 人被俘、9 人到 1993 年仍关在伊朗**
- `events/khafji-1991-iraqi-perspective.md`——**不重复战斗过程**，只补：
  第三军 1-20 越境命令与"迫使敌人进入地面战"的逻辑、
  伊拉克绝密研究引言（"敌人害怕伊拉克的决心……把他们拖入一场适合我军的地面战"）、
  1-29 夜第三与第四军三师越境、1-31 结束"两个师重大损失无持久收获"、
  **萨达姆"海夫吉败坏了敌人的名声，它被视为一次成功"如何定调官方军事史**
- `concepts/scud-campaign-iraqi-records-1991.md`——
  **52 枚的分配表**（特拉维夫 20、海法 8、利雅得 13、达兰 7、Baqaq 2、达曼 1、朱拜勒 1）、
  损失自报（1 军官 5 兵阵亡，未损失任何发射车与导弹）、
  **库存 230 枚＋75 枚"特殊弹头"、燃料只够 118 枚**、
  2-02 被迫减半到 2 枚/日、**2-13 al-Firdos 后下令"报复"打 Hafir al-Batin 美军**、
  循环发射路线、**难民营发射阵地只在缴获原稿里（公开版删掉）**、
  1-25 十枚为最成功一日、与 Force 17 协作、西部沙漠特种部队交火三例

**更新 3 页**：来源页、`wars/gulf-war/index.md`、`index.md`

**本批的关键点**

1. **"逃伊朗"是 1-26 萨达姆的命令，有明确理由（保存待用）**，不是溃散或叛逃；
   结果与意图相反——伊朗不归还，"安全保管"没有共同定义。
2. **飞毛腿的硬约束**：燃料只够 118 枚 → 2-02 必须减半发射率。这解释了 2 月发射量的下降，
   **不是联军猎杀的战果，而是库存见底**。本库同时保留 Hallion 侧"猎杀效果有限"的记录，
   两条互为印证但因果归属不同，并列不裁断。
3. **al-Firdos（2-13）触发"报复"命令（2-14 11:45）**：联军侧通常把 2 月中旬的发射记为
   "持续骚扰"，伊方文件显示其中有**明确的政治报复动机**。
4. **"特殊弹头"书中未明说是什么**，本库不推断为化学弹头。

**检查**：全库 731 个 md，YAML bad 0；断链 7 处全为存量；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉜ Woods 批次七：ch7 后段前半（2 月 14 日—24 日）

**读取范围**：ch7 后段前半，p.206—220，约 9250—9900 行。

**新建 3 页**

- `events/soviet-mediation-february-1991.md`——2 月苏联调停全过程：
  2-12 普里马科夫构想 → 2-15 巴格达电台宣布准备"处理 660 号决议"→
  2-18 戈尔巴乔夫要阿齐兹转达"巴勒斯坦问题交给我"→
  **2-22 阿齐兹宣布 48 小时解除制裁换三周撤军**；**三封信全文**：
  萨达姆 2-23 19:00 信（"我们把伊拉克的荣誉托付给这份信任"）、
  戈尔巴乔夫 2-24 04:45 回信（建议**把 21 天改成 9—10 天**）、
  萨达姆 06:30 回信（"布什的双手沾满了流血"）；萨达姆急于向俄国大使证明
  "这封信写在进攻消息之前"；**Woods 的关键判断：油田点火（2-22 已燃 140 多口井）
  让莫斯科提议在华盛顿当场死亡——预授权的自主性炸掉了自己的退路**
- `events/feb-24-1991-iraqi-leadership-meeting.md`——2-24 当天的会议录音：
  02:00 第一军"情况在控制之下"；"苏联骗了我们"／"管他们的父亲……逐屋作战"；
  朗读三封信；"我就知道他会背叛我们，这个骗子"；阿齐兹"别问我"；
  "法国人在进攻？还是坐在他们师前面哭？"、"密特朗非常卑鄙"；
  **萨达姆先见之明**（"先撤回海岸线上伸出去的部队，否则路被切断就回不去"）；
  **有参谋当面说出"他们要打共和国卫队右翼"却被忽略**；
  给人民讲话草稿（"敌人继续溺死在自己的血与耻辱中""局势完全在控制之下"）；
  09:00 的实际态势（第 14 师"可能被击败"，西翼第七军只报"七架直升机"）
- `concepts/iraqi-army-morale-collapse-1991.md`——士气崩溃：
  第 20 师逃兵供述（"不相信那个事业"、一天一顿无肉米饭、三人分 1.65 升水、
  "都在想着投降，恐惧在阻止他们"、尸体留在原地）；
  五环因果链（1-21 节约弹药 → 看得见打不着 → 防空失去机动 → 补给断绝用骆驼 →
  成建制逃亡）；al-Majid"弹药节约反而提高了联军效能"；
  共和国卫队参谋长 1991-05 的坦白；第四军军官"真正伤害我们的是慢速飞机"；
  **政权层三次误判**（把士气当纪律问题、当宣传问题）

**更新 3 页**：来源页、`wars/gulf-war/index.md`、`index.md`

**本批的关键发现**

1. **萨达姆确实在让步**：2-22 已同意 660 号决议与三周撤军，2-24 06:30 的信还在"确认我们已同意的事项"。
2. **油田大火炸掉了自己的退路**（Woods 判断）：预授权给军长的点火权 → 2-22 点燃 140 多口井 →
   布什以此为理由拒绝苏联提议 → 2-24 地面战开打。这是本批最重要的因果链。
3. **2-24 的会议室里有人说对了**（"他们要打共和国卫队右翼，或用空中力量消灭他们"），
   萨达姆的回应是"要不是他们的空军，我们的共和国卫队早就出来把他们宰了"。
4. **士气崩溃是"节约弹药"命令的直接后果**，而政权把它当成纪律/宣传问题。

**检查**：全库 734 个 md，YAML bad 0；断链 7 处全为存量；`SCHEMA.md` sha256 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉜ Woods 批次八：ch7 后段（2 月 24 日全天至 27 日）

**读取范围**：ch7 后段，p.220—237，约 9900—10560 行。

**新建 2 页**

- `events/iraqi-withdrawal-from-kuwait-1991.md`——撤出科威特：
  **2-25 20:30 萨达姆的电话**（"我不希望我们的军队惊慌……希望他们抬着头回来"）、
  Husayn"死刑判决比这道命令容易得多"、Sultan 的班子的两夜时序（第一夜：海湾行动／
  第三军／海军／Faylakah；第二夜：第四、六、二、七军，共和国卫队 Tawakalna 留到最后）、
  信使"无法到达科威特城，因为道路遭轰炸、车辆被毁"、通信崩溃与"没有指挥官怎么撤退"、
  "我们没有为撤退做过计划，根本没想过这件事"、天气救了人也毁了撤退、
  **2-26 07:00 萨达姆推翻数小时前的"摧毁"令**、2-26 的实际命令流（1145／1520／1610／1740）、
  **73 东线的伊方版本**、2-27 萨达姆亲笔信（神学化动员）、
  2-26 广播"史诗般的决斗"、3 月下旬把"撤出"改称"**撤退战**"、
  **萨达姆为共和国卫队辩护"卫队司令有权做他所做的……这不会改变"**（对政变的恐惧）
- `concepts/iraqi-victory-narrative-1991.md`——"我们赢了"叙事的构造：
  三步（重设目标→重设判定标准→政权存活即胜利）、四根支柱（"只有面对面才算战争"、
  Project 777"17 天"、共和国卫队幸存、海夫吉）、
  **本库归纳的"四点不算错"与"四点错在哪"**、能维持十二年的三个条件、
  与 Karlin 侧"海湾战争被神话为 RMA 证明"构成同一枚硬币两面

**更新 3 页**：来源页、`wars/gulf-war/index.md`、`index.md`

**本批的关键点**

1. **2-26 07:00 萨达姆亲自推翻自己数小时前的"摧毁一切带不走的装备"令**，
   改为"撤出所有装备与伤员"——这说明他在 26 日上午仍在试图保存装备。
2. **撤退的失败不是"溃逃"，是"没有计划的计划"**：
   伊方自己说"我们没为撤退做过计划，甚至没想过"，加上通信全断、无指挥官、天气双重作用。
3. **"撤退战"是 1991 年 3 月下旬才定的名字**，目的是让士兵"学会此类行动的最精确技能"——
   叙事改写有明确的实用动机。
4. **萨达姆对军事政变的担忧高于对外部入侵的担忧**（为卫队的独立性辩护），
   Woods 指出"正如 2003 年又将如此"。

**异常**

- 书中一处日期矛盾：al-Majid 说萨达姆认定"撤出"一词不准确、应称"撤退战"，
  针对的是"3 月 26—28 日"的机动，而撤退实际发生在 2 月 26—28 日。
  **已标注为书中原文／可能的笔误或 OCR 误差，待回 PDF 第 231 页核对。**
- 本批修正自身笔误 1 处：`events/desert-storm-100-hours-ground-war` 不存在，
  已改为既有的 `events/iraq-1991-desert-storm-ground-war`（4 处）。

**检查**：全库 736 个 md，YAML bad 0；断链 7 处全为存量；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉜ Woods 批次九：ch7 末（2 月 27 日—3 月 3 日）

**读取范围**：ch7 末段，p.237—247，约 10560—11000 行。

**新建 1 页**

- `events/ceasefire-and-safwan-1991.md`——停火与萨夫万谈判：
  **2-27 亲笔信承认原防御计划"不正确"**、改城市战（并类比两伊战争的
  al-Shush／Dezfuz／al-Karun／霍拉姆沙赫尔）、八条重新部署令（共和国卫队负责巴士拉内部防御）、
  2-27 共和国卫队报告的语气（"尼布甲尼撒、汉谟拉比、Adnan 状况良好"、Medina 师"超过 50% 实力"）；
  2-28 空降谣言与 Tallil 以南真实交战；萨达姆 5-1 复盘（"每营三十五辆坦克"＋承认士气是严重问题）；
  **萨达姆的停火解释**（"布什直到意识到我们的装甲在抵抗才加快停火""他一个人抢在安理会之前"）；
  官方战史两个互相矛盾的版本（"敌人打不进来" vs "我们抵消了技术优势"）；
  **3-2 Hawr al-Hammar 堤道：600 多辆车辆被毁，汉谟拉比师被命令返回巴士拉**；
  **伊方军官自述"如果没撞上美军，就没有空返回巴士拉"**（起义已开始）；
  萨夫万：代表团路上遭射击、坦克护送、警卫受伤；
  **萨达姆的谈判方针**（"以胜利者的精神去""不要先握手""用更严厉的侮辱回敬"
  "你们连我们所抵抗的 20% 都承受不了"）；
  **两个视角并列**（Sultan"他们甚至不能直视我们的眼睛" vs 西方记述"伊拉克代表团被震住了"）；
  **伊拉克获准飞直升机**（本库标出与镇压起义的关联，非书中原文）

**更新 3 页**：来源页、`wars/gulf-war/index.md`、`index.md`

**本批最沉重的一段**

3 月 2 日美军在 Hawr al-Hammar 堤道摧毁 600 多辆伊拉克车辆，
**客观上把汉谟拉比师赶回了即将陷落的巴士拉**，而这支部队随后参与镇压起义。
伊方军官自己说"如果没撞上美军，就不会有空返回巴士拉"。
Woods 照录不评价；**本库照录、不引申为对美方决策的指控，也不掩饰这条因果**。

**检查**：全库 737 个 md，YAML bad 0；断链 7 处全为存量；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉜ Woods 批次十（完）：ch7 起事部分 + ch8 + Epilogue + 关键尾注

**读取范围**：ch7 起事部分（约 11000—11350 行）、ch8（p.299—305）、Epilogue（p.307—309）、
以及尾注 51／124／14／19 等关键条目。**全书正文（ch1—ch9）已读完。**

**新建 3 页**

- `events/al-firdos-bunker-1991.md`——**这一页本库处理得最保守**：
  204 名平民（书中估计）、尾注 124 的完整叙述、第 1 章"联军规划者不知道它也是防空洞"、
  政权 2 月初开始打"平民伤亡牌"→ 巴格达市中心成为禁区；
  2-13 萨达姆下令报复 → 2-14 11:45 六枚齐射；
  **Woods 尾注 51 的暗示（"可能是政权一次成功的陷阱，旨在制造平民伤亡"）单列一节，
  标为〔Woods 提出、未经证实〕，并列出支持（4 条）与反对（4 条）两方证据，不写入任何结论**；
  同时标出书内两处对死者身份的表述不一致（"复兴党精英及其家属" vs "寻求庇护的平民"）
- `events/iraq-1991-uprising-iraqi-explanation.md`——3 月起事的政权解释：
  **"复兴党一度失去除 al-Anbar 省以外所有省份的控制"**（本书最重的事实陈述）、
  1990-12-31 GMID 情报（"他们计划在战争开始时攻击伊拉克"）、
  **被俘营长"如果我的师长命令我调转枪口，我会做的……但谁会下这道命令"**、
  萨达姆 4-3"起义才是美国计划的目的本身"、Woods"正如宏大阴谋论通常那样，
  它能解释掉显然无法解释的事"、**"背后捅刀"与 1920 年 Haldane 的类比**、
  "叛徒叛乱比它之前的阶段更难"、镇压手段（直升机、al-Majid 视频截图）；
  **暴行细节按书的处理保持极简，不勉强推导**
- `concepts/saddam-postwar-strategic-lessons.md`——ch8 + Epilogue：
  六条"教训"、"在失败之后宣布胜利正是他熟悉的事"（Woods 一句话）、
  他对 1992 美国大选的分析、**Epilogue 四条可推广洞见**
  （① 不要假设共同理解 ② **胜利在观者眼中：把胜利定义为"没有输"，把失败定义为"被赶下台"**
  ③ **不要假设公开修辞与私下信念有差距** ④ 极权国家也有军事创新）、
  Michael Howard 那句"无知，尤其是受教育者的无知，可能是一种比知识更强大的力量"

**更新 3 页**：来源页（已读／未读最终状态）、`wars/gulf-war/index.md`、`index.md`

**本批最需要谨慎的一处**

Woods 在尾注 51 暗示 al-Firdos 可能是政权故意设的陷阱。这是**全书最重的暗示，
且只有他一人提出**（Hallion、Putney、Malovany 均无）。本库：
**单列、标为未经证实、列两方证据、不写进任何结论性语句。**

**检查**：全库 740 个 md，YAML bad 0；断链 7 处全为存量；`SCHEMA.md` 未改。

**本来源剩余**：Appendix A（Timeline）与 Index 未读；尾注仅抽查关键条目，未逐条通读。

## 2026-11-18 · 来源㉜ Woods 批次收尾：全书验收 + 跨来源冲突登记 + 存量表格修复

**1) 全书批次验收（Woods 共 10 批）**

- 24 个新页：source 1、concept 10、event 13；净增约 72,400 汉字 + 4,076 英文词。
- 更新页：`wars/gulf-war/index.md`（新增「政权层」与「战争进程」两节 + 7 个来源登记）、
  `index.md`（入口 + 来源㉜ 条目）、`log.md`（11 条记录）。
- 覆盖 ch1—ch9 全部正文；Appendix A（Timeline）与 Index 未读；
  尾注仅抽查关键条目（51／124／14／19）。

**2) 新建 `topics/gulf-war-source-conflicts.md`（本书之外的库级收益）**

海湾战争线现为 **7 来源**，此前冲突散落在各页、没有集中登记处。本页补上：

- **来源层级分工表**（7 源各自的层级／材料性质／不适用的问题）——
  〔本库判断〕多数"冲突"其实源于层级混用。
- **9 组硬冲突**：① 爱国者 96% vs 拦不中；② 共和国卫队 50% 指标的三重口径
  （Hallion／Putney 战后分析／Putney 战前自评 39-47-32）；③ Warden 汇报日期与场面；
  ④ 首夜 668 架次 vs 700 架飞机；⑤ 空权因果权重四说；⑥ 海夫吉三解；
  ⑦ 飞毛腿发射减少的两种归因（压制 vs 库存见底）；⑧ al-Firdos 陷阱说（未证实）；
  ⑨ Karlin 年表 2010 两次日期。
- **5 组"不是冲突的层级差异"**（Malovany vs Woods 关于卫队师数、
  Hallion vs Woods 关于 17 天、Putney vs Woods 关于情报两条腿等）。
- **5 条引用纪律** 与 **6 个已知缺口**（GWAPS 五卷、海军侧专源、科威特沙特方来源、
  第二家独立使用 Harmony 库的研究、DIA 年表、伊方回忆录原文）。

**3) 存量缺陷修复（非本书批次引入）**

- 发现 **28 行表格内嵌 `[[target|alias]]`**，`|` 会破坏表格列结构
  （库规明令禁止）。全部改为 `[[target]]（别名）`，涉 14 个页面。
- 修复过程中脚本一度产生 4 行嵌套括号 `（…（…））`，已逐行修正。
- 复核：全库 741 个 md，YAML bad 0；表格内 alias 违规 0；断链 7 处全为存量
  （SCHEMA 示例占位符 3、log 3、jezzine 页 1）。
- `SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉝ Lambeth《The Transformation of American Air Power》（Cornell/RAND 2000）批次一

- 来源：`/mnt/share/test/The transformation of American air power (Lambeth, Benjamin S)
  (z-library.sk, 1lib.sk, z-lib.sk).pdf`
- SHA-256：`4a6541799734cf48aa8f964514efdc602d8f879fa1993f405dd58ce97831ae17`
- 提取：`pdftotext -layout` → `raw/papers/lambeth-transformation-us-air-power/lambeth-transformation.txt`
  （1,064,750 字符）；**Internet Archive Scribe 扫描 + OCR 层，未重跑 OCR**。
- 书目：Cornell University Press / RAND，2000，ISBN 0-8014-3816-0，LoC UG633 .L26 2000。
- 性质：**RAND 研究项目**（Fogleman 上将 1996 年批准），**智库分析者写的空权转型论著**，
  非官方史；作者系民间飞行员，飞过 35 型以上战机约 280 次训练任务。

**批次一读取范围**：Preface、第 1 章（Air Power Comes of Age, p.1）、第 2 章前半（The Legacy of Vietnam）。

**新建 3 页**

- `sources/lambeth-transformation-us-air-power.md`——书目、OCR 状况与常见误识、
  章—行号对照（9 章）、**与库内三本 1991 相关来源的分工表**、
  **Lambeth 对 Hallion"误用产生误解"论的明确反驳**（原文对照）
- `concepts/air-power-coming-of-age-lambeth.md`——第 1 章：
  冷战"战略空权＝核＋不被使用"的概念史、1991 年前夜的判断、
  开战前伤亡预期（10%／施瓦茨科普夫 5,000／鲍威尔 3,000）、
  首夜 800 架次仅损 1 架 F/A-18（**红外 AA-6 被动寻的的技术解释**）、
  Mason"20 世纪空权的神化"、Drew"新战争范式"、
  **McPeak 三句话（campaign vs operation、"第一支被空权击败的野战军"、
  "我们持球我们得分"）及其限定语与陆军的反击**
- `concepts/vietnam-air-power-deficiencies-lambeth.md`——第 2 章：
  量级（1,248,000 架次、**800 万吨＝二战总和两倍**、2,561/3,720 架损失、58,000 死）；
  **对 Hallion 的反驳结构**（承认政治约束"公允"，但指出装备／运用／组织／熟练度四类内部缺陷）；
  **1964—68 vs 1972 的关键对照**（政治约束未消失、变的是能力）；
  早期决策链（1954 奠边府、1963 顾问 16,500、1964-03 NSAM、94 目标 16 天计划、
  参联会 Wheeler、东京湾决议、**Pierce Arrow 64 架海军飞机**、渐进升级的选择）

**更新 4 页**

- `wars/gulf-war/index.md`：新增「空权转型论（第九来源）」节；sources 加 lambeth
- `index.md`：新增「空权转型论（跨战争）」入口
- `topics/gulf-war-source-conflicts.md`：**新增冲突 10**（越战失败的归因：误用 vs 能力不足）；
  来源数 7→8；sources 加 lambeth

**本批要点**

1. **Lambeth 与 Hallion 在越战归因上明确对立**，且 Lambeth 是后来者、点名批评，
   而 Hallion 无法回应——这是本库记录的第一组**有时间不对称的论战**。
2. **首夜损失的技术解释**（红外被动寻的、无雷达照射故无告警）是库内此前没有的细节。
3. **800 架次**与库内 Hallion 668／Putney 约 700 构成第三种说法，
   已并入冲突 4 的口径差异。
4. 本书**大量重叠**于 Hallion/Putney 的 1991 部分，但**科索沃（ch6）与空天协同（ch7）
   是库内空白**，后续批次的重点应放在这两章。

**异常与修复**

- 本批两次踩到库规"表格内不得嵌 wikilink"：来源页的比较表与冲突页的增补行。
  已分别改为列表形式；复核全库**表格 alias 违规 0**。

**检查**：全库 744 个 md，YAML bad 0；断链 9 处（4 处为 SCHEMA/log 的示例占位符与
本日志中的字面写法，5 处为存量），本书新增链接 0 断链；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次二：第 3 章前半（苏联动因 + 训练革命）

**读取范围**：第 3 章前半，p.54—64（行 2932—3480），至"A Revolution in Training"与 DOC 制度。

**新建 2 页**

- `concepts/soviet-threat-driver-us-air-transformation.md`——**补库内一个结构性空白**：
  此前所有来源都在讲"1991 年美国很强"，但没有一本讲"**它本来是准备打谁的**"。
  内容：华约 60→90-120 个师 vs 北约 45 个师；3,600 架支援飞机；
  **苏联每年 1,300 架战斗机＝每天 3 架／每周一中队／每月一联队**；
  MiG-23 带来**"全向导弹威胁"**取代越战的"后方偷袭"范式；Su-24＝苏联的 F-111；
  MiG-29/Su-27 质的追平（下视下射、迎头攻击）；3:1 与 2:1 两种数量算法；
  **"对消耗无动于衷，只要前进势头维持"的作战哲学**；OMG 与 FOFA；
  **尾注 3 的"好消息"：苏联飞行员熟练度被正确评估为远低于美国、
  作战概念僵硬且依赖地面控制**——这构成全书论证的闭环；
  1973 年赎罪日战争作为"预演"（**以色列损失 97 架＝整个空军的 1/3**、两周内物资损失 30%）
- `concepts/aircrew-training-revolution-dact-redflag.md`——训练革命的**建制史**：
  1972 年 Nellis 研讨会（"我们没跟上""**没在飞机器的人身上投入足够努力**"）、
  **"记录的飞行时间与作战熟练度没有相关性"**这一基石前提、
  DACT 的技术理由（角速度 corner velocity 等）、
  **1972-10 第 64 战斗机武器中队组建／1973-06 具备作战能力**
  （"空军中高层普遍紧张不安"、全靠 **Momyer 上将**硬推）、
  **侵略者中队与 Topgun 的方法差异**（模拟苏联式僵硬战法 vs 把性能发挥到极限）、
  T-38→F-5E、6 名 GCI 管制员、4 架／两周／40 架次／20 组机组、
  **"凭感觉把 g 判到半 g 以内"的升级标准**、
  1975-12 首次红旗（Dixon 批准、Moody Suter 上校构想）、
  **"前十架次决定生死"**、完整蓝军编成（含 OV-10／RF-4C／F-105 WW／HH-53／
  生存学校四人组／EC-121 干扰）、1977-05 的 141 架／19 型／2,000 架次、
  Green/Maple/Blue/Checkered/Copper Flag、**MCM 3-1**（含"以色列人反对写下战术"的对照）、
  **Bright Star 1982（12 架 A-10 不着陆飞开罗西，30 小时内已在埃及西部沙漠作战，
  简陋基地 17 天，对抗真实苏制 SAM）**、
  **Combat Archer（每年 700 枚以上实弹）／Combat Hammer**、DOC 制度

**更新 3 页**：来源页（已读范围）、`wars/gulf-war/index.md`、`index.md`

**本批要点**

1. **1991 年的能力是为打华约准备的**，其认知目标是一个"熟练度低、依赖地面控制"的对手——
   1991 年在伊拉克遇到的是这两种弱点的放大版。
2. **Bright Star 1982 是"1991 年不是侥幸"的硬证据**：演练想定正是西南亚，
   且已验证"离开美国 30 小时内投入作战"。
3. **"前十架次决定生死"** 是红旗全部设计的立论基础，也是本库此前没有的一句。
4. **训练革命是上将硬推的**，不是官僚体系自发——书中明写"中高层普遍紧张不安"。

**OCR 校读**：`C-3`→`C-5`、`KC-133`→`KC-135`、`KC-ios`→`KC-10`、`flares` 保留原拼写。

**检查**：全库 746 个 md，YAML bad 0；除 log/SCHEMA 外断链 4 处（3 处为 SCHEMA 示例占位符、
1 处存量 jezzine 页）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次三：第 3 章后半（战术演进）+ 第 4 章前半（沙漠风暴评价）

**读取范围**：第 3 章后半（行 3480—3700，战术演进／ACMI／低空环境）、
第 4 章前半（行 5312—5700，至开战前欺骗）。

**新建 2 页**

- `concepts/air-to-air-tactics-evolution-1970s-80s.md`——**库内此前完全空白的一层**：
  不是"训练了多少"，而是**战术本身怎么被重写**。
  焊翼／射手-掩护（"僚机只该喊 Mayday 或'长机你着火了'"）→
  **loose deuce（海军）／double attack（德国空军驻卢克 F-104）／fluid two（融合后）／
  Six Pack（F-106，换气泡座舱盖＋内置 20mm 炮）**；
  "所有飞机都被解放为射手，没有任何一架被浪费为长机的纯观察员"；
  **ACMI 1977 年夏在内利斯启用**（AIM-9 尺寸吊舱＋微波中继＋实时全向）；
  三项高性价比辅助（带活引导头挂飞 AIM-9／座舱录音／枪炮胶片与 HUD 录像）；
  **Topgun：30 天课程 23 个架次，讲评"冷静分析、不允许情绪或吹嘘"，
  谁赢谁输不重要——与电影形象几乎相反**；
  O'Rourke"要把飞机用到极限，留余量的不是真战斗机飞行员"；
  低空高威胁训练（"在无线电静默下完成整件事"）；
  **训练改革导致事故率一度显著上升，Dixon 与 Creech 两位上将"咬住子弹"接受了代价**
- `concepts/desert-storm-reassessment-lambeth.md`——第四套独立评价：
  148 名战斗死亡 vs **集结五个月期间日常事故死亡更多**；
  Cordesman"**即时历史永远是浅薄历史**"（爱国者有效性属被证伪的"事实"）；
  引 Michael Howard"历史本身不教教训"；
  **【本批核心】"Adams 在休假"这一偶然性**——若 Adams 在，
  TAC 会主导答复，而 TAC 立场是"空权支援地面"；附 **1990-08-11 TAC 传真**作反证
  （"对高价值目标示威性攻击……视需要升级"），Lambeth 评："很可能给联军一个沙漠泥潭"；
  Horner 同时拒绝了 TAC 与海军的提案（route packages＋由外向内 rollback）；
  Murray 归功于"特殊性的个人因素"；
  **Goldwater-Nichols = "海湾战争成功的教父"**（Winnefeld & Johnson）；
  ATO：200 页以上、**每天 2,000+ 架次**、**900+ 离散无线电频率**、
  **错五分钟就取消任务**、海军每天派人开软盘送六艘航母；
  Kari 四区 100+ 雷达站、"在莫斯科之后巴格达防空最密集"；
  **"预期伊拉克空军像此前叙埃空军对以色列那样作战"**（把苏联动因页与实际对手接上）

**更新 4 页**：来源页（已读范围）、`wars/gulf-war/index.md`、`index.md`、
`topics/gulf-war-source-conflicts.md`（冲突 1 补时间线：Lambeth 2000 已判定爱国者有效性被证伪）

**本批关键判断**

1. **1991 年空中战役的存在部分取决于一位中将恰好在休假**——Putney 官方史未载，
   Lambeth 有，且附反证文件。这是本库目前最具体的一条"偶然性"证据。
2. **Lambeth 在 2000 年就判定"爱国者有效性"被证伪**，而 Hallion（1992）仍以 96% 为说——
   已并入冲突 1 的时间线说明。
3. **美国 1970—80 年代模拟的那个"僵硬的苏联式对手"，1991 年以伊拉克空军的形式出现。**

**检查**：全库 748 个 md，YAML bad 0；除 log/SCHEMA 外断链 4 处全为存量；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次四：第 4 章中段（压制 Kari／夺取制空权／中空转移）

**读取范围**：行 5700—6280。Negating Iraq's Air Defenses、The Gaining of Air Control、
Air Power Fights a Land War、The Move to Medium-Altitude Operations、
Precision Engagement and the Battle That Didn't Happen（海夫吉／JSTARS）。

**新建 2 页**

- `concepts/kari-sead-and-air-superiority-1991.md`——**库内缺失的"量化过程"**。
  H 时 0300 由 **CENTAF 气象值班上尉**按"月照最少"建议（尾注 19：Horner 1997-05-15 函）；
  首夜分钟级序列（H-22 阿帕奇 Hellfire 打两处预警雷达 → H-9 F-117 投下战争首批炸弹
  打拦截作战中心 → 20 分钟后西区空中作战中心）；
  SEAD 概念原话"迫使尽可能多 SAM 连开机向 HARM 射手暴露位置"，
  并明确**追溯到 1982 年贝卡对叙 SA-6**；
  **量化链**：同时 200+ 枚 HARM 在空中／前 4 小时近 100 次雷达辐射→降至 13 次／
  首 24 小时 500+ 枚／全战近 2,000 枚半数在第一周／**第 6 天辐射降 93%**；
  **失效时间线：核心 1 小时、C2 目标 8 小时达成（Glosson 要求 24 小时）、
  Kari 36 小时、加固中心 4 天**；"不是逐层剥离而是同时攻击"；
  **SPEAR 两大弱点：AAA 按预设方位弹幕射击；Kari 朝西对以色列、朝东对伊朗、
  不朝南对沙特**；12 架以上假"Magnum"呼叫即可压制；
  损失率 1/1800 架次，比后卫 II 低 14 倍；
  首 24 小时 **812 个作战架次**（二战以来最大单次空中攻势）；
  联队损失时间分布（近半 17 架在第一周、8 架在最后一周恢复低空支援地面）；
  **越战 83% 被 AAA 打掉数千架 vs 1991 年 71% 却只有二十余架**；
  反空军：33 个战果多为 AIM-7、40%+ 为 BVR、IQAF 不到 300 架次 vs 联军 69,000、
  "最可怕的三个词是可以起飞"、八机跑道头两架被击落后六架滑回掩体、
  1-24 两架幻影 F1 被一架沙特 F-15 接连击落（挂对地弹药、目标为达兰西南炼油厂）；
  打机场两阶段（JP233 需 200 英尺直飞、龙卷风损失六架 → 1-23 转打掩体，
  20 架 F-117 各四枚 Mk 84、七分钟每五秒一命中、**373/594 机堡 63%**）
- `concepts/medium-altitude-sanctuary-package-q-1991.md`——
  **Package Q 完整编成**（72 F-16＋8 F-15＋8 F-4G＋2 EF-111＋1 EC-130＋1 RC-135），
  最后一刻改计划导致混乱，**两架 F-16 在野鼬鼠因油量撤离后才被击落**（书中标 significantly）；
  三条连锁命令（除 F-117 与巡航导弹外禁飞巴格达／中空下限扩至全区／
  **任何兵力包不得超过 23 架**）；下限 13,000→8,000→按需；
  **"选择而非被迫"**；中空代价＝无制导炸弹投放距离变四倍、精度大降，
  战后解法是**增加能投 LGB 的战机数量**（而非回低空）

**更新 4 页**：来源页、`wars/gulf-war/index.md`、`index.md`、
`topics/gulf-war-source-conflicts.md`（飞行至伊朗增列第三个数字：Lambeth"三天内 80 架"）

**本批关键判断**

1. **两个来源独立指向"伊朗框架"**：Lambeth 的 SPEAR 分析（Kari 朝东朝西不朝南）
   与 Woods 的 11-23 沙盘会议（与会者按伊朗框架回答、只有 Hamdani 说对）
   **互不相干却结论一致**——建议在冲突页作为"跨来源印证"单列。
2. **Package Q 用最直接的方式证明了中空自由来自 SEAD**：野鼬鼠一撤，两架 F-16 立落。
3. **"80 架出逃"是第三个数字**（Woods 137／伊朗 22／Lambeth 80），已并列不合并。

**检查**：全库 750 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次五：第 4 章后段（坦克打靶／战果／ATO 摩擦）— 第 4 章读完

**读取范围**：行 6280—6720。JSTARS 效能与弱点、Tank Plinking and Its Impact、
Allied Air Power in the Endgame、战果数字与 Odom 之争、Air Tasking 与空地协调摩擦。

**新建 2 页**

- `concepts/tank-plinking-1991.md`——库内唯一完整交代该战术的材料：
  **起源是 1990-12"夜骆驼"演习的物理副产品**：装甲车散热比周围沙地慢，
  日落后到午夜在红外上格外突出（且是在模拟攻击陆军第七军的对抗演习中偶然看到的）；
  **启用原因不是战术更优，而是 BDA 跟不上施瓦茨科普夫的时间表**——
  把库内 BDA 页与 50% 指标页接上；
  规模：ATO 中 **73% 的 F-111F 架次**、23 天 664 架次；
  战果：2-13/14 夜 46 架投 184 枚 GBU-12 毁 132 辆（**72%**）、全战 **920／6,100**、
  峰值 **500+ 辆/天**、CENTCOM 到 2-14 记 1,300 确认击毁；
  **"挖洞就死，出洞死得更快"**；**逃兵率 25—30%，且是在"当场处决逃兵"的命令下**；
  绰号由来（施瓦茨科普夫嫌"打靶"不敬要求改用"坦克猎杀"，结果反使后者流传）；
  JSTARS：**首过 90% 命中**、"弹药先于燃油耗尽"、单次 80% 瘫痪、分不清履带与轮式、
  **海夫吉以北"敌军活动"实为风中蛇腹铁丝网**；1-29 至 2-3 损耗速率**放大四倍**；
  装备损耗：G 日前 39%/32%/47%，战后 76%/35%/90%，
  **尾注 61：CIA 与 DIA 估计低得多，而施瓦茨科普夫拒绝让强调百分比的汇报进行**；
  **死亡公路死者 200—300 人，却因错误图像导致 100 小时停火**；
  **Odom"陆军打掉 70—80%" vs Watts"固定翼至少 61%"，
  旁证是 220,000 发坦克炮弹运去、实射不到 2%**；
  Mason"陪审团应继续休庭"与被俘军官"再打两三周就会被迫撤退"并列
- `concepts/air-tasking-and-air-ground-friction-1991.md`——
  **头两周陆军提名 1,185 个目标 → 202（17%）进 ATO → 137（12%）被打**；
  全战 3,067 个提名只有略超三分之一被攻击；
  **军长看战场像"巨大的保龄球道"**；"对抗不是关于空权的表现，而是关于陆军无法控制它"；
  **但 Horner 几乎不需要被说服就把努力转向地面部队**（区分空军内部之争与军种之争）；
  Push CAS 是 **1990 年 4 月**（危机前四个月）就想好并汇报过的；
  **陆战队 70% 架次记为 CAS 但只有 14% 在 FSCL 内**、GWAPS"很少出现部队接触的情形"

**更新 3 页**：来源页（第 4 章读完）、`wars/gulf-war/index.md`、`index.md`

**本批踩坑**：`tank-plinking-1991.md` 的 title 又用了英文双引号嵌中文短语，
YAML 直接解析失败（库规老问题），已去掉引号并重新 parse 通过。

**本批关键判断**

1. **坦克打靶不是"更好的战术"被采用，而是"打完证明不了"这个官僚问题被解决**——
   因果链 BDA 之难 → 50% 指标无法验证 → 换成能自己看见结果的打法。
2. **"22 万发坦克炮弹运去、实射不到 2%"** 是 Odom 之争里最直白的一条旁证。
3. **CENTCOM 主动拒绝百分比简报**，解释了此后所有"伊军损耗"数字为何对不上。
4. **死亡公路的 200—300 名死者 + 错误图像导致 100 小时停火**——
   与 Woods 侧伊方理解（布什抢在安理会前控制停火）并列，归因不同、不裁断。

**检查**：全库 752 个 md，YAML bad 0（修复后）；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次六：第 5 章前半（隐身／弹药／SAC 撤销）

**读取范围**：行 7883—8560。Into the Post-Cold War Era、The Operational Impact of Stealth、
The Advent of the B-2、A New Generation of Munitions、Completing the Shift to a Conventional Bomber Force。

**新建 2 页**

- `concepts/stealth-and-precision-munitions-post-1991.md`——把"隐身/精确"从形容词变成数字：
  **隐身把雷达制导 SAM 有效交战包线缩小 93% 或更多**；
  **同一场战争中：非隐身包 38 架飞机、仅让其中 8 架打 3 个瞄准点；
  20 架 F-117 打 37 个瞄准点 → 覆盖 +1,200%、飞机 -47%**；
  Cashen 的限定"隐身在实践中是低可探测性与战术的结合，
  **未采用适当战术时，名义上隐身的飞机生存性根本没有任何保证**"
  （1989—1999 年的判断，正好预言 1999-03-27 那架 F-117）；
  B-2 数量四部曲 **132→73（1990-04，柏林墙倒后不到六个月）→20（1991-12 苏联解体后）
  →21（含试验机升级）**、400 亿美元、可用率 69%／成熟 80%；
  **1996 年内利斯三架 B-2 用 GATS/GAM 打 16 个分散目标全部命中，从 42,000 英尺以上投放**；
  **由此问句反转："一个架次能打多少个瞄准点"取代"要多少架次才能摧毁一个目标"**；
  **85,000 吨炸弹中 PGM 不到 10%（约 8,000 吨），却造成 75% 以上重大毁伤**；
  DSB 1993"**一吨 PGM 通常替代 12—20 吨无制导弹药**"；
  JDAM 绕过天气（Glosson：天气比伊拉克空军更是阻碍）；
  CBU-97 十枚 BLU-108／共 40 枚 Skeet、每枚扫描 2/3 英亩；
  **Fogleman：战斧每发 150 万美元，打一场空中战役会很快让国家破产；GPS 弹药低到每发 1.5 万美元**；
  AMRAAM 主动寻的、350 磅（因 F-16 翼尖挂架限制）、
  **1982 年 9 月开始全尺寸研制、部署比原计划晚六年**、1992 年 12 月首次实战（最小射程击杀）
- `concepts/sac-disestablishment-1992.md`——库内完全空白的建制史：
  **SAC 是被它自己的司令官 Butler 提议撤销的**，理由是
  "如果再打一次波斯湾，SAC 只能带 B-52 从 40,000 英尺投带箍的高阻炸弹，
  **那我们就不会被邀请参加**"——不是战果问题，是资格问题；
  "SAC 就其核心而言是一个核机构，一直如此、当时如此、将永远如此"；
  **"越战一结束，轰炸机就回家了，直接回到核角色，结果是几乎全部那些战时经验都丢失了"**
  （解释了为什么 1991 年 B-52 机组投弹精度差）；Chain 让 31 架获得常规角色但"系统不容忍它"；
  Chain 1988 年要打掉三根"常识支柱"，并指责美国空权思维
  **"倾向于用战略一词来描述武器和目标，而不是行动和效果"**（与 Putney 侧 `counterland` 术语问题相通）；
  **1988 年弹药业已配齐（TMD、CBU-87/89/97、DAACM、CALCM），缺的是防御空域内的生存能力**；
  **1992 年 6 月 SAC 与 TAC 同时撤销**，战斗机武器学校改名加入 B-52／B-1 分部，
  **但"战斗机和轰炸机机组仍不说同一种语言，也不以同一种模式思考"**

**更新 3 页**：来源页、`wars/gulf-war/index.md`、`index.md`

**本批关键判断**

1. **"我们下次不会被邀请参加"** 是本章最重的一句——胜利之后意识到资格会丢失，
   比任何"转型必要性"的论证都更有效。
2. **"越战经验全部丢失"** 填补了一个库内此前无法解释的空白：1991 年 B-52 投弹不准的历史原因。
3. **弹药齐了、平台进不去**——不可把"轰炸机不能打常规战"当作平台缺陷。
4. 术语问题两条互证：Chain 说"战略被用来描述武器而非效果"、
   Putney 说 `counterland` 是自造词。**美军空权的词汇没跟上能力。**

**踩坑**：本批两次写错 wikilink——`air-land-battle-and-31-initiatives`
（实际文件名 `airland-battle-and-31-initiatives`）、以及一个臆造页
`pave-way-and-laser-guidance-gulf-war`（不存在）。已用全库断链扫描发现并修正。

**检查**：全库 754 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次七：第 5 章中段（AEF／海军转型／波斯尼亚"审慎力量"）

**读取范围**：行 8560—9100。Operational Concepts for the Post-Cold War Era、
Toward an Expeditionary Air Force、Navy and Marine Developments、
A New Rite of Passage over Bosnia、Operation Deliberate Force Scores a Win。

**新建 3 页**

- `concepts/air-expeditionary-force-aef.md`——建制史：
  McPeak 依沙漠风暴"暂编联队"经验建三个混编联队，样板第 366 联队
  （36 架射手：B-1／F-15C／F-15E／F-16＋E-3＋KC-135）；
  **Fogleman 砍掉两个专司 CAS 的联队，理由正是"CAS 在沙漠风暴中不是重要需求、
  也不代表未来战争"**——一个战术事实直接决定建制决定，这条因果链库内此前没有；
  AEF 出自 Jumper 在 CENTCOM 任空军司令时，
  **是 1950 年代中期 TAC 第 19 航空队"混编空中打击部队"的复活**；
  早期编成 **33—40 架（6 轰炸机／12 空对空／12 空地／6 SEAD／最多 14 运输）**、
  能力略大于一个航母战斗群但到达更快、**24—48 小时投入、surge 七天**；
  **1998 年重组为 20 个远征联队／10 个基地、每 AEF 约 230 架、约 73 架外派，
  低密度高需求资产（B-2／F-117／U-2／AWACS／JSTARS）留本土待命**；
  **"heavying up"——地面部队不再直接交战而是让敌军变重减速、由空权逐个歼灭，
  且这需要战区 CINC 的观念转变**
- `concepts/navy-and-marine-aviation-post-cold-war.md`——
  Owens"**对海军来说，比任何其他军种更是如此，沙漠风暴是变革的助产士**"；
  1992-09《由海向陆……》"**从海上机动，而不是在海上机动**"；
  F-14 加 LANTIRN（改装 200 架，进入 F-15E 同档）；
  **终于能电子接收 ATO**（正是 1991 年"每天开软盘送六艘航母"的补正）；
  舰载联队可 24 小时内换装机型、**岸上机场架次率与有效架次比高于舰上**；
  海军与陆战队 F/A-18／F-14／AV-8／EA-6B 并入共同池；
  **Owens 放弃"战略轰炸理论是否绝对正确"，改问"如何最好地为成功的战略轰炸战役作贡献"**——
  海军自 1920 年代以来的立场出现实质退让
- `events/operation-deliberate-force-1995.md`——**本库此前波斯尼亚完全空白**：
  8-28 萨拉热窝炮击 38 名平民死亡为触发点，8-30 0200 开始，11 天；
  战略前提"**对支配的恐惧是波黑塞族的核心脆弱点**"（打机动自由与补给能力，不打领导层）；
  **对手是苏式 IADS（SA-2／SA-6），由受过华约大规模空袭迎击训练的前南防空专业人员操作**，
  不是"民兵"；首日 300+ 架次／23 个目标／90 次命中、F-15E 用 GBU-10 打冷战地下指挥掩体；
  9-2 至 9-3 暂停试探、9-5 恢复，**恢复后的空袭与炮兵协调、
  由地面战术空中控制小组提供目标数据，"与 1982 年贝卡谷地行动开局高度相似"**；
  **意大利在最高层级最后一刻拒绝 F-117 从阿维亚诺出动**（因被排除在联络小组之外），
  改用战斧与 GBU-13；天气致美国架次取消 23—30%；
  **精确武器总体成功率约 60%，GBU-12 最高 76%**；
  70% 为 LGB／光电制导；**338 个瞄准点／36 个目标／600+ 件精确武器**；
  DMPI 由维琴察 JFACC 集中控制、尽量用 500 磅而非 2,000 磅；
  **"未命中 7 英尺以内不算任务有效"**；
  **1.5 架次 + 2.8 件 PGM 每 DMPI vs 非精确 6.6 枚铁弹**；
  **3,515 架次／293 架／8 国／18 个地点／750 攻击架次／65% 美国人**；
  唯一损失为法国幻影 2000D（SA-7）；代顿 11-21 草签／12-14 签署；
  Fogleman"不是击败塞族，而仅是解除围困并促其遵守联合国授权"

**更新 3 页**：来源页、`wars/gulf-war/index.md`、`index.md`

**本批关键判断**

1. **"沙漠风暴是海军变革的助产士"**——一场海军几乎没打的战争成了海军改写自己的理由，
   因为旧的存在理由（远洋制海）已无可信挑战者。
2. **"贝卡模式"第二次被复用**：1995 年空袭＋炮兵协调＋地面引导小组，
   书中直接类比 1982 年贝卡开局（第一次是 SEAD 战法，见批次四）。
3. **"heavying up"** 是本库第一次见到把地面部队角色定义为"减速器"的表述。
4. **"零平民死亡、没有塞族抱怨"是 Lambeth 单方口径**，库内无第二来源，标"〔Lambeth 口径〕"保留。

**检查**：全库 757 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次八：第 5 章末（禁飞行动的失败）＋第 6 章前半（科索沃）

**读取范围**：行 9100—9420。How the Bosnia Mission Almost Failed＋
NATO's Air War for Kosovo 前半（起源、三阶段计划、首夜、第一周）。

**新建 2 页**

- `events/operation-deny-flight-1993-95.md`——**本书唯一的"空权完全失败"完整案例**。
  Lambeth 的核心论点：波斯尼亚最该记下的教训不是"审慎力量"的成功，
  而是**之前两年多"几近灾难性的与失败的调情"**——
  "无论现代空权这个工具多么有能力，**它产生胜利结果的能力绝不是预先注定的**"；
  **100,400 个架次（1993-04-12 至 1995-12-20）vs 审慎力量的 3,515 个（70% 突入作战）**；
  100 多次 CAS 请求只批准 4 次攻击、**精确打击总共只有五次**、
  5,300 次禁飞区违规只击落 4 架 Galeb；
  **1/3 是 CAP、30% 是支援**；
  联合国限制清单（不得打乌德比纳的飞机与防空、只能打向自己开过火的阵地），
  Ryan 上将"以一种我们不常用空权的方式使用空权"、
  **"制造噪音"使塞族领导人对北约的威胁"习惯于"不去兑现**；
  两次可避免的击落：英国海鹞**为打一辆坦克第三次通过同一地点**被 SA-7 击落、
  F-16 沿"到那时已完全可预测的高空跑道形航线"被 SA-6 击落
  （**Shalikashvili"绝对没有任何情报" vs Joulwan"已知高威胁环境"，并列不裁断**；
  Perry 承认信息传递有问题；电子侦察资产"获得了实时迹象但未能及时传达"）；
  **"跑道可以炸，停机坪上二十多架 Galeb 不能炸"**——1995 年 8 月的"越南式思维"
- `events/operation-allied-force-1999.md`——**本库此前科索沃完全空白**：
  3-24 至 6-7 共 78 天；Lambeth 判定它是 1990 年代第三次空权决定地区结局，
  **但"在效率上相较沙漠风暴是一次倒退"**；
  四类问题**全是组织性的**（决策犹豫、美欧不信任、互操作性、美军内部军种冲突），
  **没有一条是打击精度**；
  三阶段计划（44 度纬线为界、第三阶段才打贝尔格莱德）、五项目标、
  **明确排除任何北约地面部队支撑**；
  地理 39,000 平方英里（小于肯塔基州）、科索沃本身不大于洛杉矶都会区；
  防空：**60 个 SAM 连／约 1,000 枚 SA-2/3/6／1,830 门高炮／240 架作战飞机
  （15 架 MiG-29、60 架 MiG-21）**，器材至少 15 年机龄，
  **但"操作人员熟悉美国战术、已精炼技术四十余年"，装备多于 1995 年波黑塞族、
  防御比 1991 年伊拉克更集中**；五角大楼战前估计首波可能损失 10 架；
  **初次攻击被公开提前宣布**（为 60 个瞄准点编程战斧需一天以上），
  Albright 当晚"**我不认为这是一场长期行动**"；
  首夜 **400 架次中只有 120 个攻击架次、40 个目标**；15,000 英尺高度下限；
  两架 MiG-29 被 F-15C 击落、一架被荷兰 F-16 击落；
  **第一周每夜平均不超过约 50 个攻击架次**

**更新 3 页**：来源页、`index.md`（新增三个后冷战事件入口）

**本批关键判断**

1. **十万架次换来五次精确打击**——本库目前关于"空权无效"最刺眼的数字，
   而且来自自己的统计，不是敌方宣传。
2. **科索沃的四类问题没有一条是打击精度**，全是决策/联盟/互操作/军种内斗。
3. **"公开提前宣布开战时间"＋"我不认为这是长期行动"** 可以解释后面 78 天的全部困难。
4. **1999 年首夜 120 个攻击架次／40 个目标 vs 1991 年 812 架次／全类别目标**——
   "效率倒退"的具体含义。

**踩坑**：`operation-deny-flight-1993-95.md` 的 title 又用英文双引号嵌中文（库规老问题），
YAML 失败，已去掉引号。

**检查**：全库 759 个 md，YAML bad 0（修复后）；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次九：第 6 章中段（科索沃僵局、升级、屈服因果、B-2）

**读取范围**：行 9420—9960。防空僵局→遮断、Clark 增兵、阿帕奇之争、
地面选项的缓慢转向、"四根支柱"与电力战三阶段、KLA 反攻、Why Milosevic Gave Up、
Air Power's Accomplishments 前半。

**新建 2 页**

- `concepts/kosovo-stalemate-and-escalation-1999.md`——结构性论点：
  **没有地面威胁 → 塞尔维亚部队仅靠分散隐蔽就能在空袭下生存**
  （与 1991 年"挖洞就死"形成精确反面：同一套能力，不同政治条件，完全不同结果）；
  强度：**第一周每夜约 50 个攻击架次（沙漠风暴第一周每天 1,000），
  一半以上飞机因天气未投弹返回**；**第三周某一个 24 小时 439 架次只打 28 个目标**；
  Clark 要 300 架 → 总数近 1,000（开战 430 的两倍多，却不到沙漠风暴的一半，
  美国增加 60%），军种首长抱怨"过度杀伤"、EUCOM 未充分利用现有资产；
  **阿帕奇之争**：公开理由"怕盟国误认为地面行动前奏"，未明说理由是生存性，
  最终 24 架部署阿尔巴尼亚、同时声明"不是地面行动前奏"（自相矛盾的物证）；
  地面选项三步退让（Shelton"目前"→Cohen"非敌对"→Albright"宽容环境"），
  Clark 与五角大楼裂痕；**Clark："在没有地面组成部分的情况下打一场地面战争，
  对空军人员来说有点像一种不自然的行为"**；克林顿"修辞牢笼"（官员语）；
  **四根支柱（政治机器、媒体、安全部队、经济体系）**、4-21 首次打电视台
  （先警告员工撤离）、4,700 磅 GBU-37 打地下 100 多英尺的全国指挥中心；
  **电力战三阶段**：5-3 石墨弹 CBU-94/BLU-114（70% 停电，只瘫痪不摧毁）→
  经济战（克鲁耶瓦茨一厂 13,000 直接失业＋40,000 分包，"产出减半、10 万人失业、
  超过二战纳粹与盟国连续轰炸"）→ **5-24 实弹打电网**
  （"这一目标集在沙漠风暴最初几天就已在巴格达被打过"）；
  **Clark："这是历史上唯一一场恋人们在暮色中沿河岸散步、在露天咖啡馆用餐、
  观看烟火的空中战役"**；
  KLA"箭"行动 5-26 四千米游击队，**起初被挫败（250 人被 700 人压制），
  但迫使塞军出来集结 → 被传感器发现 → 才打得到**；
  6-7 两架 B-52＋两架 B-1B 投 86 枚 Mk 82 与集束弹，
  估 800—1,200 人中不到一半幸存（**标初步评估、未证实**），
  五角大楼称为全战役对已展开部队最重打击
- `concepts/kosovo-causation-debate.md`——两种对立说法并置不裁断：
  "历史上第一次仅凭空权迫使军队整体撤出" vs Jackson
  "**6 月 3 日俄罗斯支持西方是结束战争最具意义的单一事件**"、
  "**我不负责空中战役；你问错人了**"（Lambeth 明标 Jackson 是公开的空权批评者）；
  Lambeth 自己的"**同义反复**"批评：没有空袭清洗会继续是真的，
  但这不等于空袭导致屈服；五条其他因素（国际支持丧失含莫斯科、
  战争罪起诉、精英家属外逃、寡头经济损失、**地面入侵预期**）；
  **他把最不利于空权主张的一条称为"最令人不安的"**；
  北约地面力量清单（SFOR 32,000→50,000、阿尔巴尼亚 7,500、
  亚得里亚海 2,200 陆战队、匈牙利 800）；
  **都拉斯—库克斯公路承重标准三变：难民 → 布拉德利 → M1A2（投降前三天）**；
  秘密 Plan B-minus（9 月第一周，170,000 人，英国出 50,000；
  渊源 Plan Bravo 300,000）；
  **B-2 战绩：43 个任务、不到总架次 1%、投放全部精确弹药的三分之一、
  能在让所有其他盟机停飞的云层之上作战、首夜第一个突入的人驾平台**；
  21 架轰炸机（10 B-52／5 B-1／6 B-2）投了 23,000 枚中的 11,000 枚

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"挖洞就死"（1991）vs "分散就能活"（1999）**——同一套空中能力，
   政治条件不同，结果完全相反。这是本库关于"空权有效性"最有结构的一条对照。
2. **"同义反复"批评**是本库见到的最清晰的关于反事实论证的批评。
3. **一条路的承重标准（难民→布拉德利→M1A2）** 是"行动比言辞更响亮"最字面的例证。
4. **B-2 43 个任务投了三分之一的精确弹药**——隐身轰炸机最有说服力的一组数字，
   与 1996 年内利斯演示形成"预演→实战"链条。

**检查**：全库 761 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次十：第 6 章后段（战果归零／假目标／SEAD 失效／F-117）

**读取范围**：行 9960—10330。战果统计、Friction and Problems Encountered、
Frustrations of the SEAD Campaign、The F-117 Downing。

**新建 3 页＋更新 1 实体页**

- `concepts/kosovo-ground-force-attrition-evidence.md`——"打不着"的证据链：
  **第三周末北约分析人员未能确认击毁哪怕一辆坦克**；
  初步复盘"空中战役对塞尔维亚在科索沃的军事行动几乎没有影响"；
  KFOR 实测"只有少数"；**五角大楼最终 700/1,500，但检查人员未发现相应数量残骸，
  塞军撤退时带走数百辆且"桀骜不驯而非被打败"**；
  **口径从 150 辆下调到 110 辆**（因许多是假目标）；
  **假目标工艺：牛奶盒材料做的坦克、烟囱倾斜的烧柴炉冒充火炮、
  假目标内放盛水容器在阳光下升温以复制红外信号**；
  JSTARS/红外在科索沃"基本不适用"的技术原因（SA 分散、关机省油、
  藏于谷仓教堂森林居民区）；
  Lambeth 判词"这是先前战略选择的可预测结果，而非空武器固有缺陷"；
  **"33% 的空中努力用于对付防空换来零阵亡"**；
  **"无人机损失不引起关切，因为它们是故意派去送死的"**——1999 年原话，
  预言了此后二十年的无人机战争逻辑
- `concepts/kosovo-sead-failure-1999.md`——为什么八年之后同样装备失效：
  ① 敌人不开机（"拒绝成为合作目标"，无法压制也无法证明压制成功）；
  ② **"融合雷达输入"——从北方跟踪、把数据馈给南方防空雷达，
  使南方扇区作战中心在附近无任何有源雷达的情况下引导武器**，
  这解释了 F-16CJ/EA-6B 为何用 HARM 追踪"通常部署在 SAM 连附近"的雷达会失效；
  ③ 山地使 JSTARS MTI/SAR 与 U-2/RC-135 传感器斜视角失效；
  **全战约 700 枚 SA-3/SA-6 发射、许多是弹道式无制导**；
  塞族固定战术是打离场编队的最后一架；
  **F-16CJ 盘旋太远，探测到发射并发出 HARM 所需时间超过 SAM 飞行时间**，
  所以被攻击的战斗机"基本上只能靠自己"；
  **首次把进攻性计算机网络战作为精确武器**（Jumper 证实），
  1991 年只监听不操纵 vs 1999 年"把假目标放进敌方计算机使其与对方本来就相信的东西相吻合"；
  **"操作方对情报方"两难**（"不要摧毁，我还在监听"）
- `events/f-117-downing-1999.md`——隐身飞机首次战斗损失：1999-03-27 约 20:45、
  布达诺维奇附近、**一阵 SA-3 弹幕**；
  洛马专家：**"标准倾斜转弯可使雷达截面积增加 100 倍以上"**，而狭小空域内不可避免；
  RC-135 未能定位肇事 SA-3 连并可能未及时转达——
  **"与 1995 年 6 月在波斯尼亚 F-16 被击落前所发生的情况非常相似"**；
  Hawley"当你面对大量未被定位的威胁时，即使在一架隐身飞机里你也有风险"；
  三种技术假设（舱门开启／云底剪影／双基地雷达）；
  **空军正式复盘的结论（媒体转引，空军沉默）：低技术战术＋快速学习＋精明的即兴创造，
  在一个转瞬即逝的瞬间汇合，使一枚不在正常雷达制导模式下工作的 SA-3 击落该机**；
  **空军排除：舱门卡住／低于 15,000 英尺／被 AAA 击中**；
  三项被指称（alleged）的程序性失误：RC-135 未跟踪、
  **三处可探测的低频雷达因美机"轰炸了雷达复合体内错误的瞄准点"而未被瘫痪**、
  **因 SACEUR 禁飞波黑（保代顿协议）F-117 连续四晚飞同一航线**、
  EA-6B 距 80—100 英里且方位不对
- `entities/equipment/f-117a-have-blue.md`（**更新，非覆盖**）：
  追加 1999 年战斗损失一节，frontmatter 增补 `lambeth-transformation-us-air-power` 至 `sources`，
  `updated` 改 2026-11-18

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"打不着坦克"与"村庄被烧"是同一件事的两面**：塞军不需集结就能完成清洗，
   所以既能躲空袭又能干活。
2. **牛奶盒坦克＋晒热的水平衡红外**——本库全部史料中最低成本对抗高科技的实例。
3. **"雷达与发射架分离＋融合雷达输入"** 是防空方对反辐射武器的一次成功适应，
   而它用的是**四十年前的电话线与地下电缆**。
4. **"政治约束生产战术可预测性"已是第三次重演**（1993 海鹞三次通过、
   1995 F-16 可预测跑道形航线、1999 因代顿禁飞而四晚同航线）。
5. **情报链断裂也是第三次**（1991 Putney 侧／1995 波斯尼亚／1999 科索沃，后两次同一型 RC-135）。

**检查**：全库 764 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` sha256 仍 `191cd20f951e`。

## 2026-11-18 · 来源㉝ Lambeth 批次十一：第 6 章末（科索沃"教训"判词）— 第 6 章读完

**读取范围**：行 11354—11700。A First Cut at Kosovo "Lessons"。

**新建 1 页**

- `concepts/kosovo-lessons-lambeth.md`——本书对盟军行动的最终判词，全书最不客气的一节：
  **他反对"空权胜利"这个说法本身**：克林顿"证明了持续空中战役能阻止一支地面军队"、
  Cohen/Shelton"压倒性的成功"、报纸"仅凭空中力量取得的胜利"，
  而 Lambeth 说这些"与高级军事专业人士的共识观点明显相悖"；
  **四条职业军人的否定引语**：战前四位军种参谋长一致怀疑仅凭空袭能否成功、
  空军参谋长 Ryan"我不知道没有地面部队我们能不能做到"、
  1995 年得胜指挥官 Leighton Smith"历史上我们运用军事力量可能最糟糕的方式"、
  前空军参谋长 Fogleman"结果不错不意味执行得当，空权的运用是有缺陷的"、
  本次 JFACC Short"我们本应该做得不一样"；
  **他们当时真的没想到会赢**：五月底大多数空军上将已认为打不着更多分散部队、
  Short 已认为战略难以击垮米洛舍维奇意志、
  **当时正在计划把空中行动持续到十二月甚至更长**；
  三条正面（首次纯空中强制、79% 精确弹命中、**平民死亡不超过 600 人**——
  人权观察实地调查口径、经空军分析员认可"西方最好的实地数据"）；
  **总判词**："盟军行动是那些负责指导其运用的战略的人对空权的一次次优运用"、
  "**如果空中武器被以损害其可信度的方式使用，空权的长处本身就会变成弱点**"；
  **违反两条古老公理**（达成突然性、让敌人对意图不清楚）；
  **逐条驳斥国防部事后辩解**：①"迫使塞军躲起来因而作为机动力量无效"——
  但种族清洗不需要战术机动，**他们不需机动也能杀人**；
  ②"迫使米洛舍维奇保存防空"——**保存下来的防空整场都在限制北约的高度与航线**，
  这是把"必要"说成"美德"；
  **极尖锐的反事实**："如果米洛舍维奇满足于蹲守并熬过轰炸，
  他本可以轻易质疑联盟的长期凝聚力"——**不是北约赢了，是米洛舍维奇犯了错**；
  Ellis 上将"**运气起了主要作用**"、北约领导人"判断得完全错了"；
  **Adam Roberts 对 1995 年神话的解构**——塞族此前已在地面失利（被逐出克拉伊纳）、
  1995 年轰炸不是针对塞尔维亚本土，**而这个神话直接导致了 1999 年的误算**；
  Jumper"30,000 架次不损失一名飞行员，使空权看起来确实是无风险的、太容易的选择"；
  **Mason 的"自我威慑"与圣乔治比喻**（"如果圣乔治的第一优先是部队防护，
  他现在就不会是英格兰的主保圣人"）；
  Ralston/Jumper **"渐进主义可能是未来、效率可能居次"**；
  **全书对转型最凝练的表述**："使 1999 年的渐进主义比越南更能忍受的，
  是隐身、精确防区外攻击与电子战的进步——
  **转型的意义不在于打得更好，而在于允许政治犯更多错误**"

**更新 3 页**：
- `events/operation-deliberate-force-1995.md`——**重要修正**：追加"十·补、
  '神话化'的警告"一节（引 Adam Roberts），并在评价节前加交叉提示。
  **1995 年就其设计目标而言是成功的，但读成"空权独自迫使屈服"是神话；
  1999 年的决策者正是按这个神话行事。** 两说并存、因果联系写明。
- `sources/lambeth-transformation-us-air-power.md`（第 6 章读完，剩余第 7—9 章）
- `index.md`

**本批关键判断**

1. **一场胜利之后，赢的一方内部职业判断与政治判断分离得这么彻底，本库仅见**：
   肯定它的是总统、国防部长、报纸；否定它的是前空军参谋长、空军参谋长本人、
   1995 年的得胜指挥官、本次战役的空战指挥官。
2. **"当时正在计划打到十二月"** 与"他们赢了"的叙事直接冲突，且出自美方自己的规划。
3. **"不是北约赢了，是米洛舍维奇犯了战略错误"**（加速清洗，剥夺了北约退出的政治空间）——
   与 Woods 侧"萨达姆 1-23 评估全合理、结论全错"是同类事件。
4. **史学修正了一条既有页面**：1995 年"审慎力量"的成功被 Lambeth（引 Roberts）
   判定为被神话化，而它正是 1999 年误判的来源。这是本库最好的一条
   "史学如何影响决策"的实例，已回改批次七的页面（不覆盖，追加并交叉标注）。
5. **"转型 = 允许政治犯更多错误"** 是全书对二十年技术进步价值最凝练的定义。

**检查**：全库 765 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次十二：第 7 章前半（太空支援沙漠风暴／作战性太空文化）

**读取范围**：行 11857—12310。The Synergy of Air and Space、
Space Support to Desert Storm、The Creation of an Operational Space Culture。

**新建 2 页**

- `concepts/space-support-desert-storm.md`——**本库此前对太空层完全空白**，此为技术基础层：
  战前两个世界（有飞行资格的"操作者" vs 出自头顶侦察与采办秘密世界、
  主攻核威慑的太空专业人员），
  **互相轻蔑的原始用词："技术宅"（techies）、"口袋火箭"（pocket rockets）、
  "太空学员"、"太空极客"**；
  **"aerospace"一词 1958 年由空军参谋长 White 创造**，
  但**1985 年 Friedenstein 中校在《空军大学评论》主张"aerospace 没有条令基础、
  太空是独特的"——战前最强声音是分离而非整合**；
  1990-08-02 入侵当天**第一批到场的不是飞机、军舰或地面部队，而是在轨的美国太空系统**；
  七类贡献：GPS（**在轨仅 16 颗、比全覆盖少 5 颗、1 颗故障靠法尔肯基地现场写软件救活**、
  **每天七个长达 40 分钟的"悲伤时段"**、PLGR 紧急采购 **13,000 台／4,500 进战区**）、
  DSCS（**3 颗卫星／128 个战术终端／85% 通信量／首次因作战重新定位卫星**）、
  DMSP（**用土壤湿度分析确定"左勾拳"路线**）、DSP（**30 秒探测尾焰／飞毛腿飞行仅 7 分钟**、
  靠伊拉克三次试射"意外之喜"调校系统）、
  侦察与 BDA、Landsat 与 SPOT（**"非机密"产品的价值**）；
  鲍威尔"**卫星是最重要的单一因素**"；
  McPeak"第一场太空战争"＋Lambeth 的限定（**不否认是支援，但"全套阵容首次直接支援各级作战"本身就是分水岭**）；
  **对库内 BDA 页的重要补充**：Lambeth"主要是程序问题与敌人剥夺信息，而非能力局限"
  （与 Putney 逐条机制并列），并补 **尾注 9：精确武器可观察损伤本小——越准越难评估**
- `concepts/space-operational-culture-lambeth.md`——建制与文化层：
  **机制一句话：让一个"受益者"去管"供货方"**（Horner 作为沙漠风暴 JFACC 出身、
  是太空支援的受益者）；
  **TAC/SAC 解散的副产品：ICBM 划归 AFSPC**——导弹部队"终于从飞机人的拇指下解脱"，
  而 AFSPC 得到一群"**作战使命既极其严肃、又几乎永远不可能真正执行**"的战士
  （**让太空人变成战士的，是一群从未开过火的人**）；
  1992 年蓝带小组（Moorman 主持）诊断"只重采办运营卫星、极少注意为地面战士利用它们"；
  **1993-11-01 太空战争中心（SWC）**成立，以武器中心与空战中心为范本；
  **SWC 要解决的三个真实缺陷**：循环时间慢、**高度机密信息"过度分隔"造成僵局**
  （**同一病症第四次出现**：1991 SCI 帐篷／1995 波斯尼亚／1999 RC-135／太空领域）；
  Strike II 1994（空中 F-15E 靠卫星坐标夜袭模拟机动飞毛腿）；
  把太空塞进蓝旗、红旗、武器学校（**"在手指扣在扳机上的人当中形成太空素养基础"**）；
  **五任 CINCSPACE 连续为作战飞行员**（Horner→Ashy→Estes→Myers→Eberhart，附背景表）；
  **结论句："太空推动"（space push）→"操作者拉动"（operator pull）**，
  同时保留"资深太空人可能私下怀疑这是不是受欢迎的发展"；
  海军太空司令部司令"**海军没有太空就在功能上死在水里**"

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **本库第一次有了太空层**：七类贡献逐一对应到具体系统，且都带缺陷
   （16 颗卫星、七个悲伤时段、30 秒 vs 7 分钟）。
2. **"让受益者管供货方"** 是本库记录过的最干净的一条组织变革机制。
3. **"从不打仗的导弹部队把作战身份带进了太空社群"**——最精微的一处讽刺。
4. **"过度分隔导致所需材料从未送到最需要它的人手里"** 是本库同一病症的第四次记录，
   而且这次是在太空领域——说明它不是某个单位的失误。
5. **"越准越难评估"（尾注 9）** 是本库 BDA 页缺的一条因果，
   与 Putney 侧"判读技艺消亡"互补。

**检查**：全库 767 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次十三：第 7 章中后段（太空作战媒介／太空军归属之争）

**读取范围**：行 12310—12800。Space as a New Medium of Operations、
The Promise of Space Power in New-Era Warfare、Growing the Integration of Air and Space。

**新建 3 页**

- `concepts/space-as-operational-medium.md`——2000 年的战略判断：
  **四类任务**（太空支援／力量增强／太空控制／力量运用），
  后两类当年"几乎完全没有开发"与"会突破政治可接受性"；
  **太空控制当时能做的"几乎全部就是干扰或物理摧毁地面卫星站"**；
  力量运用清单（天基激光拦弹道导弹、天基非核超高速动能武器打地面点目标，
  **"甚至可能包括装甲车辆"**）；
  **"经济重心"用美国自己的卫星指自己**（在轨超 1,000 亿美元＋年 70 亿商业产业）；
  **GPS 悖论：JDAM 完全依赖实时 GPS 引导，而 GPS 信号微弱易被阻断**；
  **商业卫星扩散**（3 英尺分辨率、法国 1980 年代中期与俄罗斯 1992 年引领、
  1994 年克林顿批准出售、十年内十余颗民用卫星、结束先进国家垄断）；
  **最惊人的一条反事实："如果伊拉克能获取实时商业卫星信息，
  左勾拳的震撼效果极可能会被削弱。幸运的是苏联人选择不告知萨达姆，
  尽管他们几乎肯定知道"**；
  伊拉克气象卫星下行链路与**一台未经授权的 Landsat 接收机**被炸
  （因无法只切断对方而不切断盟友）；
  **2020 年推演："他们打掉我们大部分天基能力。我们的军事力量就这样停摆了"**；
  反卫星武器会先服役、天基对地打击在"更下游"；
  太空带来的三样新东西（开火前控制态势、持久存在、不被还击的参与者）；
  **Moorman 的成本反驳：替掉一架预警机需要 25—40 颗卫星，"一种非常昂贵的方式"**
- `concepts/space-service-rivalry-1996-98.md`——军种归属之争：
  1996 Corona 会议《愿景声明》**"air force → air and space force → space and air force"
  三个词序**（词序即优先级）；
  **Horner 1997："空军大致处于陆军 1920 年时的位置"、即"一种否认的状态"，
  且最尖刻地说这"几乎变成了空军的一次角色与任务抢夺"**——
  说话者本人正是把太空拉进作战体系的那个人；
  1998 年参议员 Bob Smith 的最后通牒（**"这不是太空战争；这是利用太空支援空中战争"**），
  指控空军只把太空当信息媒介、天基导弹防御与空天飞机投资"微不足道"、
  未把太空军官提到最高将领层；
  **陆战队司令 Krulak："那片海就是太空，空军说'那是我的'，我说'你别想拿走'"**；
  空军答复"必须先完善走路再奔跑"——**同一事实，双方得出相反结论**
- `events/dudayev-killed-1996.md`——**本库对车臣战争唯一页面**，
  且是作为"太空利用的意外后果"案例引入：1996-04-24、
  俄罗斯情报定位后传给对地攻击机、据报发射射频寻的导弹、
  **在他用卫星野战电话通话时**；媒体称两枚导弹由便携电话天线与中继卫星之间的信号制导；
  **俄国防部拒绝确认或否认**——本库逐条标来源层级，技术细节不作已证实

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"左勾拳的成功部分依赖苏联选择不告诉萨达姆"** 是本批最惊人的一句，
   与 Woods 侧"伊方读不懂公开信息"拼成完整图景：既读不懂，也没人告诉。
2. **"经济重心"被用来指美国自己的卫星**——罕见的自我指向用法。
3. **"那不是太空战争，是利用太空支援空中战争"（Smith）** 与
   **Horner"角色与任务抢夺"** 并列——**内部人拆自己的台，比外部批评更重。**
4. **"为每个 JFACC 设常设太空支援小组"** 是 1991 年 SCI 帐篷问题的制度化答案。
5. **杜达耶夫页严守来源层级**：Lambeth"很可能"、媒体"据报"、俄方"拒绝确认或否认"，
   不写伤亡、不作首例引申。

**检查**：全库 770 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次十四：第 8 章前半（空权论战两条线、理论之争、Pape 之争）

**读取范围**：行 13150—13500。Untangling the Air Power Debate、
The Dispute over Air Power Theory、Does Strategic Bombing Work?（前半）。

**新建 1 页**

- `concepts/two-air-power-debates.md`——**全书的方法论骨架**：
  Lambeth 指出**两条并行但分离的论争被混为一谈**：
  ① 理论之争（战略轰炸能否迫使屈服？空权能否独立赢得战争？）；
  ② **条令与地盘之争（哪种运用概念最值钱、作战角色如何分配、预算份额）**——
  **他判断第二条远比第一条重要，而第一条已"大体 moot"**（不是"无效"，是"提法被技术变革绕过"）；
  思想史接线：**杜黑**（打民众与工业中心、"征服制空权"既必要又充分）→
  **米切尔**（同样相信打敌地面与海上力量）→
  **1930 年代空中战术学校的"瓶颈目标"**（"以相对较小力量、几乎外科手术般精确
  使敌人战争生产停顿"）→ **沃登的重心**——本库第一次把这条线完整接上；
  三条被引判词：Ziemke"战略轰炸对空军身份的核心性正如新约对天主教会"、
  Record"不可修复地玷污了空权的信誉"（**Lambeth 反驳：把萨达姆赶下台从来不是明确目标，
  这是在指责空权未能完成一件从未被要求做的事**，附布什回忆录尾注）、
  **Pape 33 场战略空中战役"战略轰炸不可能是决定性的"**；
  **对 Pape 的两面评价**：他对"战略空权倡导者高估恐吓"的批评是对的，
  但把"战区 vs 战略"当成对立、且无法给 Horner 归类（Watts："通不过常识检验"）是错的；
  **核心方法论一击——"虚假二分"**：Pape 说三分之二以上精确弹药打的是"战区"目标，
  Lambeth 说这恰好证明"**这些表面上战区的行动产生了清楚明确的战略结果**"，
  **因为共和国卫队自始就被列为 CENTCOM 计划中的"战略"目标**；
  真正的贡献被争论遮住：**"迅速夺取制空权，再利用那种主导地位摧毁或瘫痪
  敌方多样的军事力量来源，使自己的地面部队以最小困难与损失完成剩余任务"**；
  Ziemke 的反讽："**把战略轰炸等同于空权，反而把空权最具决定性的方面
  排除在它自己的效能标尺之外**"；
  **1991 年的两种意图**（近期逐出科威特 vs 磨掉伊拉克"此后"的棱角）——
  这个区分解释了本库 Woods 侧与 Hallion／Putney 侧为何记录得不一致

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"moot"不是"无效"**：Lambeth 说的是**问题的提法**被技术变革绕过去了。
   读者若简化成"Lambeth 认为战略轰炸无用"就完全错了。
2. **"虚假二分"是本批最有用的分析工具**：它同时解释了本库冲突页里
   "空权因果"那一组为什么吵不清——**各家对"战略/战区"标签的用法不同，统计口径就不同**。
3. **"瓶颈目标"→沃登重心**的思想史接线，是本库第一次接通。
4. **"两种意图"的区分**让 Woods 侧（第二种意图的长期后果）与
   Hallion／Putney 侧（第一种意图的实施）不再显得互相矛盾。

**检查**：全库 771 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次十五：第 8 章中段（杜黑过时／"战略"定义／空权能否单干）

**读取范围**：行 13500—13830。Does Strategic Bombing Work?（后半）、
Can Air Power Do It Alone?

**新建 1 页**

- `concepts/douhet-obsolete-and-strategic-definition.md`——
  ① **两种意图的成绩单**：第二个意图（影响伊拉克"此后"）表现"不那么响亮"而招致最严厉斥责，
  但 Lambeth 说那是"不恰当的衡量标尺"；
  基础设施攻击**不超过全部攻击架次的 10%**；
  **Gordon & Trainor（两位陆军出身作者）："空中战役几乎已经赢得了战争"**；
  ② **GWAPS 的官方判定**：少有证据表明基础设施攻击起了关键作用，
  **摧毁伊拉克几乎全部石油产能"没有产生重要的军事结果"**
  （战争结束得太快，燃料短缺来不及影响）；
  ③ **"23,000 个架次未达 30% 损耗指标，但第二个目标达成了"**——
  与 Putney 侧 50% 指标页吻合，**并说明那个指标是坏指标**；
  ④ **"战略"一词的正确定义（Builder）**：不是平台或目标类型，而是**决定性作战效果**
  （"直取咽喉""聚焦于目的""转化性""改变游戏规则"）；
  1991 年真正的"战略"焦点：**毁态势感知与集体行动能力 → 迅速制空权（sine qua non）
  → 剥夺伊军协调反击能力**；
  ⑤ **条令对立**：**AFM 1-1（1992）讲"摧毁敌人进行战争的能力"（效果）
  vs JP 1-02（1994）仍按"关键制造系统/电力系统/运输系统"等目标类型定义**，
  "为当前辩论中对战略空战的所有其他错误处理定了调"——
  与 Chain 1988、Putney `counterland` 术语问题三条互证；
  ⑥ **杜黑"过时而非错误"**：他的前提是"空权除了无差别破坏民用目标别无他能"，
  **这个前提不存在了**；"以惩罚为导向的战略现已过时——
  除非一个人想做的只是为一桩过失寻求报复，或阻滞敌人战后的经济与社会恢复"；
  ⑦ **"空权能否单干"的边界划定**：Record 在打稻草人、
  **尾注 28 一条反证：Glosson 曾告诫施瓦茨科普夫"需要一场能打十五个回合的空中战役"、
  "将是一场马拉松，而不是冲刺"**；
  鲍威尔"**在每一场战争中，都必须是步兵在战场上举起胜利的旗帜**"、
  "**这类战略是为希望获胜而设计的，它们不是为获胜而设计的**"；
  **Warden 个人确信可以只靠迅雷达成目标，但"从来连遥远都算不上是空军这个法人的主张"**；
  **Horner 因不同意而把他留在利雅得参谋部之外**；
  **英国部队司令 Hine 的自问"依赖这一点是否明智？"**——"我确信空权会非常有效甚至决定性，
  但带着一个不利的地面力量对比去开战，风险太高了"

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"杜黑过时而非错误"**——因为前提消失，不是因为推论错。这个处理比简单否定诚实得多。
2. **"战略 = 决定性作战效果"（Builder）** 与"1991 年战略实际所指"必须一起读，
   否则会退化成"战略 = 基础设施"。
3. **AFM 1-1 vs JP 1-02 的对立**把术语问题变成制度问题：**空军的条令对、
   参联会的通用词典错**——而词典是全军的语言。
4. **鲍威尔"为希望获胜而设计，不是为获胜而设计"** 与 **Hine"依赖这一点是否明智？"**
   并列为"对不确定性的定价"；并注明 **1999 年科索沃用的正是这种战略，却奏效了**
   ——**反例并列，不裁断。**
5. **Glosson"马拉松不是冲刺"** 一条尾注推翻了"空权鼓吹者以为能速胜"的整个指控。

**检查**：全库 772 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次十六：第 8 章后段（军种地盘之争）

**读取范围**：行 13830—14170。The Battle over Resources and Doctrine、
Interservice Rivalry Escalates（前半）。

**新建 1 页**

- `concepts/roles-and-missions-battle-1990s.md`——Lambeth 说这一场"远比理论之争重要"：
  **"四支空军问题"（Nunn, 1992）**＋JP 1-02 的"纵深攻击"定义（FSCL 后 15 英里以上）；
  **角色／职能／使命三个词的制度区分**（第 10 编／国防部长／CINC），
  Lasswell 上校"陆军打陆战、空军在空中作战、海军在海上作战、陆战队从海上向岸投送"；
  **McPeak 的"四场战斗"分区**：近距（含其上方空域）归地面司令、
  纵深与高空归空中司令、后方/两栖/海上分归陆军/陆战队/海军；
  **他自称这不是给空军"三分之二"的花招**；**"接缝"（seams）由战区 CINC 管理**；
  三条反对：**Garner"Air Force uber alles"**、
  **McPeak 主张陆战队"退出空运业务、ATACMS 与 F/A-18"并放弃太空主张**、
  **Otis"FLOT 已不存在，线性战场概念失效，控制权应归地面司令"**——
  **两人都用"技术变了"论证，结论相反**；
  **McPeak 退役后的自述："本质上是零和博弈"、"各军种默默串通把它关在地下室里，
  像某个疯狂的亲戚"**；委员会**回避了核心问题**，把争论赶回条令与长期规划，
  于是有 DAWMS／QDR／NDR；
  **Lynn："触及各军种的制度身份、各司令部的作战概念，
  甚至触及本部最神圣的部分——各组成部分的预算份额"**；
  空军把 1991 年战果换成新概念：**"精确空中力量可在美国地面部队抵达之前
  迟滞、阻止并可能击败敌方装甲进攻"，且"过早投入地面部队会招致不必要友军伤亡"**

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **空军的论证是道德论据而非预算论据**（"早点派地面部队会多死人"），
   这解释了为什么陆军反应如此激烈——**它直接威胁陆军的核心职能**。
   与 AEF 页的"heavying up"是同一论证的两种表述。
2. **"接缝由唯一不属于任何一方的人来管"**（战区 CINC）是本页最好的制度洞察，
   与 JFACC 页同一逻辑：**联合的难题不是谁听谁的，是谁有权切分。**
3. **McPeak 与 Otis 的对照**：两人都说"技术变了"，
   一个推出"分区管理"，一个推出"FLOT 消失、无需分区"——
   **同一个前提，相反的结论。**
4. **"制度身份＋作战概念＋预算份额"三层（Lynn）** 是本库关于
   "军种之争为什么难解"最好的一句概括，与 Karlin 侧"铁三角"结构相通。

**检查**：全库 773 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉝ Lambeth 批次十八（完）：第 9 章后半 —— 全书正文读完

**读取范围**：行 15140—16150。The Changed Essence（后半）、A Struggle between New and Old、
Effecting a New American Way of War。

**新建 3 页**

- `concepts/air-power-payoffs-and-limits.md`——四项回报与三项限度：
  **朝鲜对照补完**（"空权不能独自阻止北朝鲜入侵""不会像沙漠风暴那样单方面打 40 天"）；
  **回报一：态势感知不对称**（Hobbes"盲人国里独眼人为王"；
  但"地下室的一支连队""人群中 12 名恐怖分子"仍做不到，**且这对地面部队一点也不更轻松**）；
  **回报二：做以前做不到的事、以更少做更多**；**回报三：开战即控制态势，
  "同时"取代"顺序"**（"初次攻击甚至可能是隐蔽的——进入计算机系统"，
  而 1999 年已发生）；**回报四：持续压力与关闭敌人指挥能力**；
  **"不必粉碎敌人，只需扰乱其集体行动能力"**；
  Watts"空地战斗日益由来自空中的间接火力主导"；
  **全书最大判断："最大效果是救人"**＋Hartmann"用脑飞不用肌肉飞"
- `concepts/kuhn-paradigm-air-land-struggle.md`——**全书最出人意料的一节**：
  用库恩框架处理军种之争；**"老范式不会被过于轻易放弃，这是健康的"**；
  **"所谓的新范式绝非不言自明地是空天范式"**（Larry Welch 四条新能力
  "绝非空中与太空力量的专有属性"）；两条压力（钱与伤亡敏感）；
  **民调数据推翻"公众怕死人"的前提**：战前无人支持开战 → 开战后 68—84% 支持、
  地面战前 79% 只要空战 → **地面战开打后 75% 认为打得对**
  （**公众跟着结果走，不跟着伤亡走**）；
  **告诫一至九**：承认做不到什么／承认对方仍提供什么／Neustadt 式说服
  （"那正是他们自身利益所要求的"）／**否认杜黑"拥有制空权就是拥有胜利"
  （"那句话在 1921 年首次说出时是假的，今天也一样假"）**／
  与城市工业轰炸告别／**缺一套"打地面部队"的理论**（Murray：计划者"只是把目标堆积起来"）／
  **TACWAR 模型三条具体指控**（不允许在 SAM 网上开洞、打 GCI 站点"是浪费的"、
  武器与目标可以完全错配）／别再谈"主导性空天力量"／需要当代的"胜利"概念
- `concepts/new-american-way-of-war-lambeth.md`——全书收尾：
  Mason"不靠承诺与抽象理论，靠以可接受代价确保政治目标的能力"；
  **澄清空军高层从未主张空权万能**，且一些高级空军人员认为
  **前沿地面部队可能是最佳地区威慑**；
  **"1947 年设定的目标（摧毁意志）未实现，实现的是陆军的靶子（摧毁军事力量）"**；
  **"政治正确的联合"**（politically correct jointness）与 1981 年伊朗人质营救反例；
  **真正决定战争方式的是战区 CINC，不是军种参谋长**（"空军参谋长再雄辩也只被视为硬件积累者"）；
  **"TAC 与 Warden 在 1990 年 8 月那道裂痕今天还在"**（把批次三"Adams 在休假"拉成全书线索）、
  Haffa"空军可能不再作为独立军种存在"；
  **奥古斯丁定律"2054 年一架飞机吃掉整个国防预算"**；
  **三种低成本反制**（打 JSTARS/AWACS/加油机、打运输机、打前沿基地、终至 WMD 反威慑）
  ＋ **Patton"别以为发明能代替苦战"**；
  **最后三条限定**（空权不能无地面/水面参与而胜；空权不必然更重要；
  **地面力量从"达成胜利"变为"确保胜利"，且只有地面部队能施加最后一击**）

**更新 2 页**：来源页（**全书正文读完**）、`index.md`

**本批关键判断**

1. **全书说话的对象不是空军，是战区 CINC**——这解释了为什么全书反复强调
   "能给 CINC 什么"而不是"空军多强"。
2. **"绕过了难以捉摸的目标（意志），直接走向咽喉（军事力量）"**——
   空军 1947 年的目标未实现，实现的是陆军的靶子，这才是军种摩擦的真正来源。
3. **TACWAR 三条指控说明：不是空军吹牛而陆军不信，是双方的模型不描述同一个世界**——
   模型要求"杀死全正面所有 SAM"，而实战只打了几个节点。
4. **"公众跟着结果走，不跟着伤亡走"**（战前无人支持 → 开战后 68—84% 支持）
   推翻"美国公众怕死人"这个常见前提，与科索沃"自我威慑"构成三角：
   **决策层的顾虑大于公众的顾虑。**
5. **"缺一套打地面部队的理论"** 是全书最重的自我批评，
   而且它把 1991 年那个"幸运地成功了"的部分指认为**没有理论支撑的部分**。

**全书完成**：18 批，共新建 **31 页**（来源 1、概念 25、事件 5），另更新既有实体页 1。
未读仅 Acronyms 与 Index（工具层）。

**检查**：全库 778 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量）；
表格 alias 违规 0；`SCHEMA.md` sha256 仍 `191cd20f951e`。

## 2026-11-18 · 来源㉞ Gansler《Defense Conversion》（MIT Press 1995）批次一

**来源**：`/mnt/share/test/Defense conversion  transforming the arsenal of democracy (Gansler, Jacques S)...pdf`
（Internet Archive 2022 扫描 OCR，300 页，sha256 `d815cf2e2439…`）
**入库**：`raw/papers/gansler-defense-conversion/{gansler-defense-conversion.pdf, .txt}`（15 MB / 11,370 行）

**读取范围**：Foreword、Preface、第 1 章 The Challenge（行 300—900）。

**新建 3 页**

- `sources/gansler-defense-conversion.md`——书目与作者位置（TASC 高级副总裁、
  前国防部副部长帮办）、核心论点（**"把产业转型为大体上一体化的军民结构"**，
  既不维持现状也不全转民用）、**史料性质：这是一本主张书（advocacy），不是中立史**、
  出版下限 1995、OCR 状况（**正文可引，表 1.1 等表格全废，本库不使用本书表格数据**）、
  章目与行号对照表、本书在本库中的位置（**补的是"造武器的工厂与人"这一层**，
  与 Lambeth 记的同一场裁军互为两面）
- `concepts/post-cold-war-defense-drawdown-gansler.md`——
  **裁军量级**：现役减 25 万、**国防产业裁员近 200 万**（算上间接效应至少翻倍）、
  预算 -8%、采购 -25%；参议员 Pryor 估"**1992—1997 每天 1,000 人失业**"；
  **产能利用率 35% vs 高效 85%**；工人承担最多（军种先保人员经费）；
  **最重的一条：同期 IBM 1992 亏 50 亿、1993 亏 80 亿以上、1986—1994 裁 18 万人，
  波音 1992 裁 1 万、1993 裁 2.8 万**——**国防裁员的困难不在于人多，
  而在于能接收这些人的公司同一时期也在裁人**；
  **四次裁军对照**（二战：提前规划＋需求旺＝好得出奇；朝鲜：无援助但不需要；
  越战：**二十多个联邦项目仍然很难**）⇒ **援助项目数量不是关键，
  产业可转换性与宏观需求才是**；"和平红利"没来（1993 年 118 起自决运动、
  前苏联四国约 30,000 件核武器）；1989 年民调"**日本以三比一被视为最大威胁**"、
  商务部首次进国安会、"**利息支出超过国家安全支出**"
- `concepts/weapon-cost-growth-and-procurement-cycle-gansler.md`——
  **四宗罪**（太贵、太慢、不可靠、保障费高）；成本量级（几千→几百万、
  轰炸机 ~10 亿、舰艇 30—50 亿）**与 Lambeth 引的奥古斯丁定律是同一件事两个版本**；
  **16.5 年 vs 6—18 个月**是全书核心矛盾（**制度尺度而非技术是瓶颈**）；
  1995 年十条需求清单（含"**定位并摧毁移动目标**"，而 1999 年科索沃发现没做到）；
  **"部队规模 vs 装备现代化"取舍**（Gansler 立场：该保装备，因此主张削减航母与重装师）；
  **"十年窗口"**；"设计上就要便宜"是文化变革

**更新 2 页**：`index.md`（新增来源㉞ 入口与两页）、来源页（批次记录）

**本批关键判断**

1. **本书是"主张书"，引用纪律已写进来源页**——数据标〔Gansler 口径〕，
   且其立场（长期在国防工业界与国防部任职、主张军民一体化）须一并交代。
2. **两次跨来源印证**：① 成本增长／奥古斯丁定律（Lambeth）；
   ② "制度尺度而非技术是瓶颈"（Lambeth 的太空任务迁移页）。
3. **"能接收裁员的人的公司也在裁员"** 是本批最重的事实，
   也是此后所有再就业方案绕不过去的硬约束。
4. **四次裁军对照的结论反直觉**：援助项目多寡不决定成败。

**OCR 甄别**：封面 `Gansler` 误识为 `bansler`、`1978` 作 `m.978`、
`1,200` 作 `1,20c`、`20ooD` 类错位；**表 1.1（核化生与导弹扩散表）几乎全废，
只剩零散 x/X 与乱码，本库不使用**，仅记表题与出处。

**检查**：全库 781 个 md，YAML bad 0；除 log/SCHEMA 外断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉞ Gansler 批次二：第 2 章前半（产业政策先例／产业脆弱性）

**读取范围**：行 1330—1650。The Cold War Defense Industry 前半：
产业政策争论、政府扶植先例、Industrial Vulnerability、Avtex、
下层供应商四面夹击、四个重组例子之坦克段。

**新建 2 页**

- `concepts/us-industrial-policy-precedents-gansler.md`——**全书最反直觉也最有力的一节**：
  **"美国一直有事实上的产业政策"**（农业与住房各约 250 亿美元补贴）；
  **"规则驱动 vs 计划驱动"**（美国让法官裁决成为国家政策，政府与产业基本敌对；
  日本计划驱动、由工程师与商人推动）——**Gansler 的论证策略不是"学日本"，
  而是"我们已经在做，只是不说"**；
  **四个先例**：NACA 1915（"尽管发明了飞机，美国在飞机工业上却落后于若干欧洲国家"；
  任务是"为美国飞机工业取得世界领导地位"；下初始订单以求达到低成本产量；
  **该部门至今仍是美国最大的单一出口产业**）、
  晶体管（陆军通信兵赞助研究、补贴工程、资助生产规划、**成为初始保证买方**、
  标准化、传播成果 → **到 1955 年出现相当大的产能过剩**）、
  数控机床（空军在主承包商工厂采购安装维护一百多台、付钱让人学，
  **1951—1957 年该产业研发支出增长八倍**）、计算机与 RCA 通信；
  **工具三分法：研发（NACA）／购买力（计算机与半导体）／专利控制（RCA 与通信）**；
  **"市场决定谁死，政府决定结构"**——对政府角色的精确界定，
  且明言当前"监管增加只是使不可避免的改变更困难"
- `concepts/defense-industry-vulnerability-tiers-gansler.md`——
  **四个脆弱性变量**（部门依赖度／企业规模／管理文化／**工艺技术的商业可适用性**）；
  表 2.1 国防销售占比（造船 80%／弹药 84%／飞机约 55%／通信设备 51%／
  半导体 34%／计算设备 10%）**——其中"飞机"一格 OCR 损坏（`ay)`），
  按后文"约 50/50"推定为 55／45，已标"推定值须回 PDF 核对"**；
  **造船的例子：维修交给公共厂还是私营厂，直接决定私营造船业存亡**
  （私营造船就业 1990 年约 13 万 → 1998 年 3 万，理事会预测"2000 年美国可能连一家开着的船厂都没有"）；
  **"为保住船厂多造一艘核潜艇＝每艘约 30 亿美元"**——
  国防采购事实上在承担产业政策功能，但从未被如此设计；
  **Avtex 人造丝厂**（唯一国防资格来源、1988-11-03 关闭、政府花 1,800 万美元维持、
  供给航天飞机喷管与 MX／三叉戟 2）；
  **下层供应商的四面夹击**（预算削减＋主承包商收回自制＋**下层无"购买美国货法"保护
  而被更便宜的外国来源取代**＋主承包商收缩供应商名单）
  ⇒ **"正是在这些企业当中，商业与军事世界存在最明显的工艺共通性"
  ⇒ 全军民一体化的落点在下层，不在顶端**；
  **"太多"与"太少"用同一套预算工具、方向相反**；最难的是政治，
  解法是**基地关闭委员会式的"全有或全无投票"**

**更新 3 页**：来源页（批次记录与页脚）、`index.md`

**本批关键判断**

1. **"别只看靠不靠国防，要看机器能不能干别的活"**——第四个变量是全书论证的枢轴。
2. **"太多"与"太少"方向相反却共用一套工具**，这个矛盾 Gansler 自己承认，
   并把破局点放在政治上（全有或全无投票）。
3. **救下层供应商最划算**，因为它们的工艺最接近民用；
   反过来说，只救主承包商救下的是最难转民用的部分。
4. **"为保船厂多造一艘潜艇 30 亿美元"**说明产业政策已经在发生，
   只是以采购决定的形式、且未被当作政策来设计。

**OCR 甄别**：表 2.1 与表 2.2（前 25 大承包商）**大面积损坏**
（如 `Lis?`、`9° 809898520`、`The Mh`、`oilph3`），
**本库不使用表 2.2 的任何数字**；表 2.1 只用正文明确引述的那几格，
且"飞机"一格标为推定值。

**检查**：全库 783 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉞ Gansler 批次三：第 2 章后半＋第 3 章

**读取范围**：行 1650—2170。Four Examples of Restructuring（坦克／飞机／电子／服务业）、
"defense conversion" 词义批评、Growing Foreign Involvement 全章。

**新建 2 页**

- `concepts/four-sector-restructuring-cases-gansler.md`——
  **四个案例构成一条"可转换性梯度"**（坦克最不可转 → 飞机半 → 电子民用领先 → 服务人力为主）：
  **坦克**：一家企业（通用动力）经营两家政府所有的厂，
  **"当陆军决定建立第二家坦克厂时，它选择不让另一家企业来经营"**——
  没创造竞争而是打击竞争；**"俄国人在同一家工厂造坦克和铁路车辆"**；
  **下一代坦克的病根："陆军坚持独特规格"，而不是让坦克装甲与发动机
  与"大型卡车陶瓷发动机"的商业生产要求兼容**（同一生产线可同时造卡车与坦克陶瓷发动机
  → 巨大规模经济）；
  **飞机**：1992 年销售额 728 亿、商业贸易顺差 237 亿、**美国最大单一出口产业**；
  **波音不是国防部任何飞机的主承包商，洛克希德现在不做任何商业业务**；
  波音与麦道把军民运输机业务拆成不同设施以避开国防部负担——
  **"无论是美国商业产业还是国防部，都没有从潜在的协同效应中获益"**；
  引 Tyson"**美国政策真正的错误在于一种杂乱无章的国防产业政策**"；
  对照日本：MITI 定为国家级重点，四家公司拿防卫厅钱做工厂现代化，
  **"在同样的机器上、在同样的工厂里"造 FSX 与波音 777 主要结构件，
  每家 75—85% 经费依赖军方**，且已取代诺斯罗普与 LTV 成为美国商业运输机主要供应商；
  **喷气发动机是全书中唯一已军民一体的子系统**（GE 与普惠在军民两界持续竞争、
  政府持续出钱改进），但警告"可能萎缩到只剩一家"；
  **电子**：国防部研发与装备预算 **50% 以上由电子产业提供**；
  **"硬固定在汽车发动机缸体上的芯片超出军规温度范围 10 度、成本远低于军用、
  可靠性更高、性能先进两到三年"**；
  **"前十大半导体生产商中有五家表示因政府强加的负担与特殊要求而拒绝国防业务"**；
  **服务业**：1993 年联邦服务采购 1,030 亿（国防部 620 亿）；
  **"1980 年代中期海军以每小时 6.50 美元采购有学位的工程服务"**、
  **"没有商业组织会以'有工程学位证书、体温 98.6 度'为依据购买工程师"**；
  FFRDC（Aerospace／Mitre）无竞争获经费且不缴联邦税，今天做的工作与私营企业完全相同；
  **政府从服务的"零售者"变成"批发者"**；
  **"defense conversion"一词的七种含义**（社区调整／工厂转换／再培训／制造技术培训／
  技术转移／转型为一体化基础／研发转向双用）⇒ **"没有就应当做什么产生共识"**
- `concepts/foreign-dependency-defense-industrial-base-gansler.md`——
  **《购买美国货法》管主承包商、不管零件供应商**（1933 年至今）；
  **石原慎太郎"停供半导体可让美国六个月跪下"＋实际发生过的展示：
  MITI 迫使京瓷子公司 Dexcel 向战斧导弹项目扣留先进陶瓷技术**；
  **海湾战争期间"国防部代表被派到世界各地奔走，恳求特别安排以加快外国部件销售"**
  ——本库关于 1991 年最有价值的侧面记录之一；
  **核心概念替换："问题是脆弱性，不是外国依赖"** ⇒ **自给自足的冲动是错位的**；
  外资所有清单（1991 年 Thomson-CSF 试图收购 LTV 国防部门被公众压力逼退；
  Matra 买 Fairchild；**Singer 被拆卖给加拿大/日本/英国/德国四国买家**；
  美资外资所有 1976 年 2,500 亿 → 1990 年 2.2 万亿；
  **日本酸素买下美国唯一半导体稀有气体厂**、**美国最后两家商业硅制造商卖给德日**；
  十年内 100 家计算机、45 家半导体、35 家先进材料、20 家航空航天公司被外资买下）；
  **因果：一座芯片厂 2.5 亿—10 亿美元，美国企业难以获得长期融资，被迫出海找钱**
  ⇒ **"不是不想卖给自己人，是买不起"**；
  **Exon-Florio／CFIUS：1988—1992 审查 700 案，只拒一案（疑为间谍掩护的中国机构）
  ⇒ "该法被认为是一只纸老虎"**，原因是**没有总体目标 ⇒ 每案都是特例 ⇒ 都能找到理由**；
  技术转让：**两条冷战前提都不成立了**（军民技术难以区分、且民用往往更先进）；
  **Matrix Churchill**（萨达姆内弟经伦敦母公司买下俄亥俄机床公司，
  商务部批准为"玻璃纤维厂"，**而它也可造导弹壳体**）；
  **FSX**（**"日本缺的不是造部件的能力，是总体设计、系统工程与集成"**；
  美方商务部/国防部/国务院无协调立场，且供应商在国际谈判中互相竞争）

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"陆军坚持独特规格"是整本书最具体的病根**：不是军品不能转民，
   而是**军品被要求不能与民用共线**——而这条要求来自采购制度，不是技术。
2. **"在同样的机器上造 FSX 与波音 777 部件"** 是对手给出的军民一体化实物图像；
   **75—85% 经费来自军方却同时在给波音做件**，说明"依赖军方"与"服务商业"不互斥。
3. **"前十大半导体厂商有五家拒绝国防业务"** 比任何理论论证都直接：**卖方不卖了**，
   而拒绝理由是**行政负担**，不是利润。
4. **"问题是脆弱性不是依赖"** 是全书最精确的概念替换，
   决定了政策答案是"多来源"而非"自己造"。
5. **海湾战争"满世界求零件"** 与空袭胜利并列，不矛盾——同一场战争的两个切面。
6. **Exon-Florio"700 批 699"** 的因果链（无总体目标→每案特例→都能通过）
   与第 2 章"市场决定谁死、政府决定结构"是同一论点的两面。

**OCR 甄别**：本章表格（表 2.2 前 25 大承包商）仍大面积损坏，**未使用其任何数字**；
正文中 `1,20c`／`M-1`／`FSX` 等专名清晰可辨；`Sémiconductors` 为 OCR 重音符误加。

**检查**：全库 785 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉞ Gansler 批次四：第 4 章（收缩路径／壁垒／国会保生产线）

**读取范围**：行 2170—2520。Initial Post-Cold War Developments：
五条收缩路径、企业实例、反垄断/环境/设备壁垒、Barriers to Effective Downsizing。

**新建 2 页**

- `concepts/defense-firm-contraction-paths-gansler.md`——
  **时间差与螺旋**：预算 1980 年代后半期就开始降，但装备交付到 1990 年代初才骤降
  （积压订单＋长生产周期），**1982—1992 销售额反而翻倍**（航空航天 700 亿→1,400 亿），
  而**1992 年底工厂利用率仅 35%**；**"成本上升→产量下降→成本再上升"的下行螺旋**；
  **部门降幅**（装甲 -55%／飞机发动机 -49%／弹药 -49%／飞机 -47%／电子 -39%／
  导弹 -34%／通信 -32%／舰船 -29%，**弹药到 1994 年降近 80%**）；
  **对政府的批评："里根与布什两届政府都主张政府不建指导方针，
  且关键决定以随机方式作出，导致低效、混乱与浪费"**；
  **五条路径**（坚持国防／外销／卖给其他政府市场／多元化／退出）；
  **通用动力"想买买不到、于是把自己一项项卖掉"**
  （导弹→Hughes、飞机→Lockheed、运载火箭→Martin Marietta、坦克与潜艇待售，
  **几年内缩编 50,000 人以上**）；Loral/Martin Marietta/Lockheed 反向收购，
  **"裁完员工后股价飙升"**；
  **七个多元化实例**（西屋做安保/气象雷达/订票/邮件分拣/车队跟踪/电动车电力；
  **休斯做客机航电与高科技街机**；TRW 做空管与国税局税务设备；
  Martin Marietta 为邮政做分拣、为 HUD 管计算机；**Lockheed 替洛杉矶收停车罚款、拆核武器**）；
  **三类壁垒**：**反垄断用错地方**（FTC 阻挠坦克弹药与夜视设备两起合并，
  陆军曾论证"只够养一家供应商"；三层论证：五角大楼既是规制者又是唯一客户／
  市场定义无法确定／国际化使唯一美国企业仍在竞争市场）、
  **环境清理**（核废料处置超 1,800 亿美元）、
  **过时资本设备**（折旧压死新业务、税法需允许快速注销）；
  **"许多国防企业对长期多元化说'算了吧'，转而寻求短期利润"**
- `concepts/congress-industrial-base-politics-gansler.md`——
  **四角联盟**（军种＋产业管理层＋劳工领袖＋国会代表团，**资本与劳工在此同向**）；
  **六条拨款记录**：FY92 加 **80 亿美元**项目、理由全是"保持生产线开工"；
  FY93 **B-2 加四架（40 亿）＋B-1 修缺陷 3 亿**；
  **布什要关通用动力的坦克/战斗机/潜艇三条线（连将领都承认军事需求很小），
  国会以"保存国防工业基础"为由给钱让三条全开**；
  **5 亿美元新航母初始资金（军内对是否需要仍在争论）**；
  **"为与对手船厂的两艘驱逐舰相匹配，再买两艘"**；
  **公共部门设施同样被护，即使重复私营部门工作**；
  **"显然，国家安全与项目效率都不是考虑因素"**；
  **机制**："**股东看季度回报，国会看下次选举**"，
  解法是**配对条件**（企业短期利润再投资于转换 / 国会拨款用于长期工厂转换）；
  **与基地关闭委员会的对照：整包表决 vs 逐个决定**

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"想买买不到、于是把自己卖掉"（通用动力）** 是 1990 年代国防工业整合最精确的图景。
2. **"为对等而多买两艘驱逐舰"** 精确暴露机制：**订单的功能是分配就业，不是满足需求**。
3. **"资本与劳工同向"** 是本库关于国防预算难砍最反常识的一条结构观察。
4. **"整包表决 vs 逐个决定"** 解释了为什么军事基地能关、武器生产线关不掉。
5. **七个多元化例子的"不体面"**（收停车罚款、拆核弹、做街机、给国税局做设备）
   才是多元化的现实形态，比任何"技术升级"叙述都真实。

**OCR 甄别**：本批文本清晰；`18 亿/1,800 亿`等数字均按上下文复核
（核废料为 1,800 亿、Avtex 为 1,800 万，两者不同，勿混）。
页码栏 OCR 损坏（`by?`、`me)`、`els!`、`7`），不影响正文。

**检查**：全库 787 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉞ Gansler 批次五：第 4 章末＋第 5 章前半（转换的历史教训）

**读取范围**：行 2863—3230。第 4 章末（克林顿转换计划与联邦培训项目堆叠）＋
第 5 章 Prior Lessons of Industrial Conversion 前半。

**新建 1 页**

- `concepts/conversion-lessons-and-failure-rates-gansler.md`——全书"教训"部分的地基：
  **失败率的硬数据**：33 家大型多元化公司 1950—1986 年 **2,644 次进入新市场**
  （70% 收购／22% 新建／8% 合资），
  **到 1986 年 74% 的不相关收购与 44% 的合资已被剥离，连相关业务多元化也有一半失败**；
  **内部增长反而稍好**（重新部署现有资源者约 20% 存活十年）；
  **收购"特别不成功"**（文化吸收＋管理层无新业务知识），
  但"裁完员工帮助利润的合并有显著短期收益"——与第 4 章"股价飙升"是同一件事；
  **转换四分之三在头三年失败**；国防企业成功率 **20%→35%**，
  相关多元化可达 **60—70%**；
  失败原因含 **"过度工程化（over-engineered）"**——军规不是优势，是成本；
  **欧洲十六项障碍完整照录**，并指出两组成对的结构：
  **"一个客户大批量" vs "多客户小批量"**、**"客户写规格" vs "客户说不清需求"**；
  **最重要的通则：多数成功转移发生在可比的高技术水平之间，而非技术降级**；
  **Melman："军工产业最高管理者本身是转换的主要障碍……除非他们准备学习，
  或者被不受'必须忘掉一套不合适的技能'所累的新人取代"**；
  **卢卡斯模式被明确否定**（工人＋意识形态驱动、缺管理层支持、十年失败），
  **"市场拉动"胜于"技术推动"**；
  **三个案例**：波音-伏托尔（**"更多注意力给了工厂重装设备，而不是设计工程师的再培训"**、
  车辆因可维护性与耐久性不合格几年内停用）、
  罗尔（赢下所有能投标的地铁合同、**不懂"按成本设计"、过度指定系统**）、
  **雷神**（专门获取营销技能，收购 Amana 改造微波炉，
  **商业销售 15%→50%，同期裁掉国防工厂 15% 劳动力**）；
  **两条原则：不要把军民目标塞进同一个产品；不要等客户来定义产品**；
  **时间尺度：Harwell 十年／Matra 二十年（1970 年钟表首战失败）／MBB 三十五年／
  瑞典估八到十年／选定后还需两年规划**——
  **与"国家只有几年窗口"构成全书核心矛盾**；
  失败代价（格鲁曼 1,500 万、麦道 6,900 万收购后亏 3.33 亿关停）；
  **技术转移最佳做法：商业设计师与用户从一开始就在设计桌上**
  （英国铁路混合研究团队；**西德工人在坦克与铁路车辆之间来回流动**）

**第 4 章末读段（未单独建页，记入日志）**：克林顿政府承诺
**1994—1997 财年共 203 亿美元"转换计划"**（1997 财年单项 52 亿），
分配为再培训 40 亿／社区援助 10 亿／双用技术 50 亿／民用技术 100 亿；
**联邦有 125 个在运项目、每年超 180 亿美元，密歇根一州就有 70 个项目由 9 个部门监管；
国防转换委员会查明共有 58 个人援助项目与 86 个社区与企业援助项目，
总审计局发现"它们之间的协调几乎不存在"，且"没有聚焦任何长期解决方案"**；
1994 年共和党大胜后这些拨款开始遭到严重攻击。

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"连相关业务多元化都有一半失败，样本还是专业多元化的大公司"**——
   这一句限定了后面所有乐观说法。
2. **"过度工程化"是全书最精准的词**：军规不是优势，是成本（与"汽车缸体芯片"呼应）。
3. **转换的瓶颈不在机器，在人的设计哲学**（波音-伏托尔的原话）。
4. **"需要的转型要二十年，可用的窗口只有几年"** 是全书核心矛盾，本批首次量化。
5. **"工人在坦克与铁路车辆之间来回流动"** 证明工艺共用是物理事实，
   要克服的是制度不是技术。
6. **联邦 125 个项目、协调几乎不存在、不聚焦长期方案**——
   与第 1 章"越战后二十多个项目仍然很难"的历史结论完全吻合。

**OCR 甄别**：本批第 5 章开头夹有一整页图表扫描残片（约行 3010—3040，
满页乱码如 `ggihaw 0 diltea id Ret Ceoreine`），**已整段跳过，未引用任何内容**；
正文部分清晰。`Rohr`／`Kaman`／`Raytheon`／`Matra`／`MBB`／`Hagglunds` 等专名可辨。

**检查**：全库 788 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉞ Gansler 批次六：第 5 章后半＋第 6 章开头（三种政策选项）

**读取范围**：行 3230—3600。第 5 章末（转换工程/管理人员、核心能力、VHSIC、
政府支持经验、基地关闭、八项考虑与九步）＋第 6 章 The Choices。

**新建 2 页**

- `concepts/core-competence-and-rd-targeting-gansler.md`——
  **最反直觉的通则**："专门化资产对盈利的贡献与其在其他市场的适用范围**成反比**"，
  因此"成功的多元化倾向于发生在靠近本行的地方"；
  **核心能力而非产品相似性**是方法论枢轴；
  **Stansaab**（军用空中预警 → 民用空管 → 医院监护，
  共同点是"**分布式项目的集中监测**"；医院那一跳**必须增加懂医院的新人**）；
  **"制度结构与公司政策甚至比兼容的技术更重要"**（解法：吸收或适应）；
  **Spectra 实验**（1986—1992 投 2,500 万／17 家／**13 家盈利／成功者 70% 收入来自商业**；
  失败的四家"**考虑解决方案，不考虑产品**——像工程师那样，没受过完成任务的训练"）；
  **VHSIC 案例**（国防部本意是帮美国重返商业半导体，
  但按传统做法**直接与大型武器制造商签约**，
  由它们挑商业元件供应商作分包——**结果元件被规定成军专用**；
  若反过来资助商业元件商、由它们给国防企业分包，
  "几乎肯定能开发出同时满足军民需要的产品"）；
  **政府能做**：第一买主（半导体→超级计算机，但"迫使政府采取长期视角，
  而它过去一直不愿"）、补贴初创、坚持 50% 成本分担；
  **政府不能做**：立法转换、救助/拉长/额外采购（除非企业真正自我改造）、
  单靠保护主义（须有时限且最终自救）；
  **基地关闭：1.5 个新岗位／158,104 个新岗位替代 93,424 个；
  代价是短期大量裁员与地方困苦**；**罗斯威尔 1967（一夜失去三分之一人口、
  失业超 20%、房价崩溃，靠"快速反应、强领导、清晰愿景、社区支持"复原）**；
  1989 年宣布关闭的 86 个基地中 **26 个受化学污染（5 个严重）**；
  **八项考虑**与**九步建议**（**顺序本身是论证：换管理层在第四步，
  改造厂房设备在第八步——而现实多数计划从第八步开始**）；
  收尾引语（改写丘吉尔）"**转换可能是最糟糕的选择——除了所有其他选择之外**"
- `concepts/defense-industrial-structure-options-gansler.md`——第 6 章开篇：
  **"即使没有冷战结束也必须改组"**（成本上涨＋开发周期长＋军民技术隔离
  本身就不可持续，**冷战结束只是加速器**）；
  **三种政策选项**：国有化（穆勒／加尔布雷思）／公用事业式管制／市场竞争；
  **国有化的关键追问："这会导致公共控制，还是仅仅提供一个政治庇护所？"**；
  **公共设施效率约低 30%、更难关闭**；"更多出于沮丧而非逻辑"，
  **但保留让步："在少数部门里可能确实是最好的方案"**；
  **公用事业管制的现状矛盾**：承包商受联邦采购条例控制，
  **却从未被正式列为"受管制"**——因为**国防部在微观层面（焊接规格、检验细节）
  管制，而不是宏观层面（结构、利润、定价）**；
  **航空、卡车运输、核电的经验：管制者被俘获、管制阻碍变化**

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"制度结构比技术更重要"** 与 **VHSIC**（同样的钱、因签约对象不同，
   一个产出军专用、一个可产出军民通用）合起来，是全书最有力的一组论据：
   **决定技术形态的不是技术政策的口号，是合同的签约对象。**
2. **九步建议的顺序**（换管理层第四、改造厂房第八）**与现实多数计划从第八步开始**
   完全对应——这一条把第 5 章前后两部分扣上了。
3. **"公共设施效率低 30%、更难关闭"** 回答了第 4 章"为什么政府船厂关不掉"。
4. **"管制在微观不在宏观"** 是全书对"国防工业有管制无政策"最精确的表述，
   与 Exon-Florio"700 批 699"是同一诊断的第三个版本。
5. **"即使没有冷战结束也必须改组"** 使 Gansler 的方案不只适用于裁军时期。

**OCR 甄别**：本批文本清晰；`VHSIC`／`Stansaab`／`Spectra`／`Roswell`／`Vickers`
等专名可辨；第 5 章末"50% cost sharing"处 OCR 作 `SO percent`，
按上下文（政府坚持产业承担一半）录为 50%。
第 6 章"利润往往显著高于……"一句在页界处截断，**本库未补全，如实标出未完**。

**检查**：全库 790 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉞ Gansler 批次七：第 6 章中段（军民一体化 · 全书核心方案）

**读取范围**：行 3600—3780。The Choices 收束、Civil/Military Integration 全节。

**新建 1 页**

- `concepts/civil-military-integration-gansler.md`——**全书核心方案**：
  **公用事业管制收束**（利润高于国防业、成本转嫁客户、
  "**唯一受益者可能只是国防产业自己**"；国会每逢此事就推、
  1980 年代加强管制产生了第 2 章的不良结果）；
  **所选路径**："政府作为独家买方必须以**促进而非取代**自然市场力量的方式行使权力"；
  **防误读关键段**："**让官僚把资本从一家企业转移到另一家企业以培育中意赢家的
  国家计划方式，并不是这里所提议的**"——他要减少国防专属规则，
  不是增加政府挑选赢家的权力；末引"谁来监督监督者"（莫尔／奥威尔）；
  **三种形态**：双用研发（共同要求）／双用工厂（共同工程、生产、保障）／
  双用设备（零件、材料、软件）→"**真正的互操作性**"；
  **"设计即双用"为三者中最重要**，且**明确否定 spin-off（军用转民用）与
  spin-on（民用改军用）两个流行模型**——因为"**国防已不再在技术上领先，
  商业也无法容忍国防的开发周期**"；
  **结构判断：只留少数国防专属工厂（主要武器总装与测试），
  "大多数主要承包商运营，以及几乎所有低层级与供应商层级的运营，都可以是双用的"**
  ——与第 2 章"下层最接近民用"首尾呼应；
  **软件占现代武器成本约 25%**；
  **MIMIC 案例（全书唯一完整的存在证明）**：
  ARPA 项目，设计准则**同等重视低成本与高可靠性**（而非仅"最高性能"）→
  **军用部署之前就被汽车业用于防撞与收费**（校车盲区雷达，
  **首次使用据称救了一名钻到车下的孩子**）→
  民用大批量使供应商（休斯与德尔科合资）重设计工艺，
  **成本 8,000→200 美元（40 倍）**→ 国防部回头买便宜货；
  成功前提：**放弃国防常规规则、从一开始用商业做法与标准**；
  **Perry 估计每年省约 300 亿美元、采购人员减 20% 以上**；
  **四条理由**（更低成本更高质量／快速获取最先进技术／
  **危机 surge 的备用产能**——"唯一替代方案是养大量常年闲置且必将过时的军事能力"／
  **更多采购竞争**）+ 宏观第五条（**每年 350 亿研发＋500 亿采购进入商业部门**）

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **MIMIC 是"存在证明"而非提议**：四步机制（加低成本准则／豁免国防规则／
   民用大批量压成本／国防回头买）是全书唯一被完整验证过的路径。
2. **"这不是我要提议的"** 防误读段必须保留——Gansler 要的是**减少国防专属规则**，
   与中文语境里"加强产业政策"的方向相反。
3. **"备用产能"理由最被低估**：军民一体化是唯一既能省钱又能 surge 的方案；
   纯国防产能必常年闲置并过时。
4. **"设计即双用"否定 spin-off 与 spin-on**，理由极其朴素：
   **国防不再领先，商业等不了**。这一条把 1995 年与冷战时代的假设彻底切开。

**OCR 甄别**：本批清晰；`MIMIC`／`gallium arsenide`／`Hughes and Delco`／
`ARPA` 可辨；`8,000 each to $200` 数字完整。
"利润往往显著高于……"一句在上一批末尾被页界截断，本批已接上（"国防产业的利润"）。

**检查**：全库 791 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉞ Gansler 批次八：第 7 章全章（国防专属工厂／手工式产业／公共 vs 私营）

**读取范围**：行 4163—4680。A Few Defense-Unique Plants 全章：
上限估算、Efficient and Effective Downsizing、Public versus Private。

**新建 3 页**

- `concepts/defense-unique-plants-ceiling-gansler.md`——
  **"不同（different）≠ 独特（unique）"**：独特的唯一标准是"是否必须为它单独建厂做设计、
  制造或保障"；**陆军火炮与铁路车轴共用同一台旋转锻造机**；
  **上限：Kutscher 1990——320 万军工相关私营岗位中不到 50 万在难转工厂
  ⇒ 国防专属部门应小于全产业 15%，且可能显著更少**
  （趋势：装备电子密集化＋柔性制造普及）；
  **"放手不管造成每一个危机都在真空中被处理"**四种局面
  （只剩一家是否该救／外国买家／公共 vs 私营没钱支持两者／
  资助下一代研发还是多造一件上一代）——**这一节把前几批所有零散案例收进一个框架**；
  **商业世界性能升成本降周期缩 vs 国防部成本同速上升、时间更拉长**；
  波音 737 生产周期 13→6 个月、降本 25—30%、UPS 货机 28 个月 vs 通常 38 个月；
  **国防部 1991 年从概念到首次生产平均 198 个月（16.5 年），且预算越砍项目越长**；
  **"时间就是钱"两条机制＋"技术一旦验证，唯一维持优势的办法是迅速建造并部署"**
- `concepts/craft-industry-downsizing-gansler.md`——
  **"四十年的重大错误假设：把国防工业看作大批量生产产业"**，
  正确位置是 **craft industry（手工式产业）**：**按技能而非按产品设计产线**；
  而现状"工厂只做一个产品、没订单就空着"恰与灵活多用途相反；
  **补贴对象应是"少数关键武器系统工程团队"而非工厂**；
  **维持竞争的具体机制**：一家造当前一代并更新、另一家开发下一代，**来回交替**＋
  **"竞争性分配"维修工作**；经济论证"维持团队成本可能小于垄断加价"；
  **反垄断三级退让**（放宽市场定义→"两家到一家"符合国家利益→国家安全压倒反垄断）；
  **外国供应商的作用是保持竞争压力**；
  **"某部门一分钱采购都没有"**的两个办法（联合生产／只养少数关键设计与生产工程师）；
  **"擅长金属切削的厂不会重视复合材料"→ 换技术路径即第二来源**；
  **政府理想角色四步**（定产业目标／逐部门分析最低需要／设定企业数与规模与技术领域／
  逐项目给指导）＋"避免管理、把决定移出政治过程"＋**借日本"行政指导"概念**
- `concepts/public-private-duplication-gansler.md`——
  **那个反讽**："**世界经济中唯一一直在显著走向社会主义的主要部分，
  是美国国防部的工业基础**"（1990—1992 每年 150 家私有化、1986—1992 累计 3,250 亿）；
  **四类公共/准公共部门**（大修厂／兵工厂／实验室／FFRDC），
  **缩减速度远低于私营部分**（因"悠久历史与非常强大的政治支持"）；
  **大修厂**：二战"保险单"逻辑→冷战后三条反驳
  （**短促冲突没时间返修**、**私营在越战与沙漠风暴中就在战区有维护人员**、
  国际公司例行全球维护）；**1991 年 69% 维修在建制内、30 多处设施、
  175,113 文职＋3,031 军职、140 亿修理＋90 亿改装**；
  **兵工厂/船厂**：农夫-士兵模式遗产、公务人员"极难被解雇"；
  **造船专项研究：私营效率高 33%**（与第 6 章"低 30%"同量级互证）；
  **实验室：700 多个、年 200 亿美元（政府研发 1/3、全国 1/6）**、
  三大核实验室各近 8,000 人；**对比 IBM 3,200 人、贝尔实验室 1,400 人**；
  军种理由"**买得聪明**"——**Gansler 明确承认"有相当的有效性"**；
  **FFRDC**：核实验室从二战保密遗产扩张到"巨大过剩产能"；
  系统工程类（兰德起源：**付不起公务员薪水吸引最好的工程师**），
  **而原始理由已消失**——私营专业服务产业能提供同样服务，
  且许多家同样"只服务政府以保持独立性"

**更新 3 页**：来源页、`index.md`

**本批关键判断**

1. **"不同 ≠ 独特"** 是全书方案的语义基石，把"不能转"从产品属性改成了工厂属性。
2. **"不到 15%"** 是政策分水岭：**"国防工业不能转民用"最多只对 15% 成立**。
3. **"手工式产业"不是"小规模"，是另一种生产逻辑**：按技能设计产线，而非按产品。
4. **"每一个危机都在真空中被处理"** 把前七批的零散案例（Avtex／Exon-Florio／
   船厂归属／多造潜艇）收进一个框架——本库认为这是第 7 章最有结构价值的一段。
5. **"补贴工程团队而不是补贴工厂"** 比"多造一艘潜艇 30 亿"便宜两个数量级。
6. **"全世界在私有化，唯独美国国防工业在国有化"** 解释了本章所有建议遭遇的抵抗性质：
   **不是效率问题，是意识形态问题**。
7. **FFRDC 的原始理由在事实上消失**（私营已能提供同样服务且同样独立），
   比"效率低"是更强的论证。

**OCR 甄别**：本批清晰；`Kutscher`／`FFRDC`／`MITRE`／`Aerospace`／`Sandia`／
`Los Alamos`／`Lawrence Livermore` 可辨；`198 months` 与第 1 章 `16.5 years` 一致，
**系同一事实的两处表述**（已互注）。
"显然存在某些独特的能力……"一句在批末页界处截断，**未补全，如实标出未完**。

**检查**：全库 794 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉞ Gansler 批次九：第 8 章前半（壁垒与"分离是程序性的"）

**读取范围**：行 4773—5140。Current Barriers to Integration：摩托罗拉无线电、
5,000 条法律、明朝引语、DSB/GAO/Brooks 对撞、Background 全节。

**新建 2 页**

- `concepts/integration-barriers-gansler.md`——
  **摩托罗拉无线电案**：沙漠风暴期间陆军急需无线电，
  摩托罗拉给警察的型号完全合用，但**法律使"以非最低价卖政府"成为犯罪**，
  摩托罗拉无法证明给的是最低价（地方分销商给警察折扣）→
  陆军求高层签豁免未果（**无国会批准无人有权违法**）→
  **解决办法是让日本从摩托罗拉买了再作为其对战争的贡献送给美军**；
  **体量**：**5,000 条法律条文／125,000 页规章／32,000 份规格／数十万人日常执行**；
  **明朝引语**："官僚统治已发展到如此高级阶段，
  以致数千人的一切隐秘需求与欲望、连同个人抱负，
  都不可逆转地与这个庞大的现状绑在一起"——
  Lambeth 判断"这也是 20 世纪末转型的主要问题"；
  **DSB(1987) vs GAO vs 众议员 Brooks 三方对撞**：
  DSB 建议半导体采购用商业做法；GAO 称其"非基于坚实事实证据"、
  未证明 CICA 阻碍商业采购、**未讨论商业与政府运营的根本差异**；
  Brooks 承认"无疑会为纳税人省数十亿"但抨击其"试图把限制性竞争合法化"、
  指责国防部"会不择手段，包括使用伪造的研究"；
  **Lambeth 式判断："不是 Brooks 错了，也不是 DSB 错了，
  而是他们试图通过国防采购追求两个不同目标"**——
  **公平与信任 vs 效率与有效，"目前全部重量压在一侧"**；
  **"即便每年数十亿美元的节省，也不能压过公平与信任问题"**；
  **最根本的制度缺口："多花的数十亿不在任何预算案里，
  被吸收进武器单价" ⇒ 增加立法与监管"不存在任何财政约束"**
- `concepts/procedural-separation-gansler.md`——全书最完整的因果解释：
  **"在绝大多数工业领域，分离的原因不是技术性的，而是程序性的"**；
  **"5 人 vs 680 人"**（波音：政府 5 人监督全部商业飞机业务 vs
  国防部 680 人监督数量远少的军用飞机）——**而航空安全是人命关天的领域**；
  **第二个原因：国防采购被用作社会政策工具**（高失业地区、少数族裔企业、
  工会化工厂、小企业），**附加要求未计入社会成本，账单落在国防部头上**；
  **10 万美元以下必须买小企业 → 买不到备用半导体（因为芯片厂商不是小企业）**；
  **白手套 32 美元 vs 商业同款 20 美元**；**衬衫纽扣间距规格 →
  行业标准的钉扣托板不能使用，需单独军用托板**；
  **行政成本**：四倍人员／三比一管理比例／206 家企业调查三倍行政成本；
  **总成本两项研究并列不裁断：30—50% vs 200—500%**；
  企业三种反应（设独立工厂／干脆拒绝国防合同）；
  **曼斯菲尔德修正案（1970）**："明文禁止把企业独立研发分摊到国防合同，
  除非完全用于国防"，**持续二十多年**；主张双用者"要么被封口、要么被解职"；
  **1992 年才被推翻**；
  **MSPB 1992：31,000 名合同官"因规则而无法创造与创新"**；
  **"公众与国会都没有区分浪费（数十亿）与欺诈（数百万）"** →
  改革选了更快的那条路（加监督），结果效率更低；
  **1980 年代两次改革的后果**：成本型竞争（低报价再求救助）
  与采购过失刑事化（**小企业负担不起辩护成本，被迫认罪**；qui tam 奖励）

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"分离的原因是程序性的，不是技术性的"** 是全书对"为什么改不动"最本质的回答；
   而 **5 人 vs 680 人** 是最有力的一条证据（航空安全用商业做法）。
2. **曼斯菲尔德修正案**证明军民分离曾被**法律强制**，不只是制度惰性；
   这条证据把全书从"建议"抬到了"纠正一项错误立法"。
3. **"浪费（数十亿）与欺诈（数百万）被混为一谈"** 把责任分给了公众与国会，
   而不只是官僚——这是全书最不讨好的一个判断，也最难反驳。
4. **"加监管不存在任何财政约束"**（成本被吸收进武器单价、不上预算案）
   是全部壁垒中最根本的一条机制。
5. **白手套与衬衫纽扣**两个小案例比任何统计都有说服力：
   **规格的目的是"可写、可比价、可公平投标"，不是性能。**

**OCR 甄别**：本批清晰；`Mansfield`／`CICA`／`MSPB`／`qui tam`／`Motorola`／
`Rock Island Arsenal`／`Lehman` 等可辨；
两处页码栏损坏（`LW   ls`）不影响正文；
"30 to 50 percent"与"200 to 500 percent"两个研究数字**并列照录、未裁断**。

**检查**：全库 796 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`）；表格 alias 违规 0；`SCHEMA.md` 未改。

## 2026-11-18 · 来源㉞ Gansler 批次十：第 8 章中段（成本型合同与军用规格）

**读取范围**：行 5140—5500。需求流程末（IDA 对「按成本设计」的评估）／
Cost-Based Contracting 全节／Military Specifications and Standards 前半。

**新建 2 页**

- `concepts/four-barriers-survey-gansler.md`——
  **两场丑闻的机制**：备件丑闻的真因是**间接费用按销售额分摊**
  （一把 12 美元的锤子被算成 500 美元，是会计结果不是贪污），
  而公众"相信同样比例适用于导弹、飞机、舰船"→ 要求更多审计 → 国会照办；
  "ill wind"贿赂案之后加的是**额外的刑事化立法**，
  效果是"在政府与产业关系中引入更大的恐惧、不信任与隔离"；
  **国防部几乎不反抗**，GAO 说"有很多演说，但没有朝向改变的真诚努力"，
  原因是**"检查者、审计员与督察员越多，责任就越分散"**（对个人是降风险，对组织是加成本）；
  **企业自己排的壁垒顺序（严格照录）**：① 武器需求流程几乎排他性地关注性能；
  ② 成本型（非价值型）合同系统；③ 独特军用规格与标准；④ 专门采购法律；
  附加项中单列**"政府保留随时更改设备的权利（单方面更改单）"**——
  **商业最怕的不是规格高，是规格可以随时变**；
  **200 家企业调查**：**"压倒性地把联邦合同的要求、而不是独特技术需要，列为首要原因"**；
  **两个传统官方理由（军品没商业市场／商业部门没能力做军品）被企业自己否认**；
  **89% 说不同产品可在单一运营中制造，200 家中只有 4 家说完全不行**；
  **需求流程的翻译链**：任务需要 → 逐级认证至参联会主席 → 演化成"一架轰炸机"→
  速度高度载弹量 → 规格 → RFP；成本只问"会不会破银行"和"能不能拨出第一年"，　
  理由是**"我们需要这个系统，到时候再想办法怎么付钱"**；
  **85% 的生产与保障成本在设计阶段就已锁死**；
  **"单引擎还是双引擎"**——最大单项后勤成本，却几乎完全在性能层面辩论，
  这个例子乘以数千个决定就**排除了并行工程**；
  **反事实**：摧毁一个指挥中心可以选"低速类货机在防区外放巡航导弹"或
  "有人高速突防轰炸机"，**巡航导弹选项已可用数十年、便宜若干数量级，
  却被需求流程挡在高级决策者之外**——**"没有重大的资源约束，传统的军事做事方式总会胜出"**
- `concepts/cost-based-contracting-and-milspec-gansler.md`——
  **IDA：89 个系统只有 32 个应用了按成本设计，且只在全面生产阶段、
  不在概念形成阶段**（而政策 1973 年宣布、1975 年成指令、1983 年还更新过）——
  **政策存在 ≠ 政策生效**（与曼斯菲尔德修正案同类，本库第三次记录此模式）；
  **成本型合同**："如果有一项做法迫使分离，那就是它"，
  哲学根源是**"对市场资本主义力量的信任 vs 不信任"**；
  三个反商业后果：**"just-in-case"库存 vs 准时制**、
  **有便宜的工人也优先用贵的**（只要成本可证明）、
  **合同官把注意力放在占成本 10% 的利润上、然后去验证那 90% 的成本**——
  **政府宁可多付 90% 也不肯多赚 10%**；
  **"最大的谬误"：武器贵不是因为暴利，国防承包商利润甚至低于受管制的产业**；
  **两套账本**：Intel 花 **200 多万美元**改会计系统以迎合国防部，然后放弃；
  **IRS 与 SEC 甚至不用政府的人核证成本，只用独立注册会计师，只有国防合同要**——
  而 Gansler 承认**"这样做成本远超节省，但这不是问题的关键"**；
  **监督体量**：企业要出政府人员**两倍**的人力供数据；
  同公司同型产品的军品部门**行政人员按销售额计是民品的八倍**；
  **B-2：国防部 183 名全职驻厂代表＋GAO 现场代表（1990—1993）＋
  1981—1990 年间近 150 次议员访问＋州与地方从空气质量查到工人安全**，
  而**"其中没有一项是为了降低 B-2 的基本成本"**；
  出路是**独立会计师事务所＋作业成本法**，真正门槛是**"一旦政府在哲学上承诺"**；
  **军规六条滥用完整照录**，含**"描述本质非军事的项目：牙签、狗嘴套、钱袋、芥末"**、
  **"详述怎么做而不是需要什么"**、**"自动施加于分包商"**；
  附属文件"许多已绝版"

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **89 个系统／32 个应用／且用错阶段**：这是全书最硬的"政策失效"证据。
   与曼斯菲尔德修正案、第 2 章"陆军坚持独特规格"构成同一模式的第三次出现。
2. **"盯着 10% 的利润、验证 90% 的成本"** 是全批最精确的机制：
   **政府宁可多付 90%，也不肯让承包商多赚 10%。** 这是考核指标问题，不是腐败。
3. **IRS 与 SEC 都不用政府的人核证，只有国防合同要**：这条论证绕过了
   "国防特殊"的说法——税收与证券同样关乎巨额金钱与公众信任，用的却是独立会计师。
4. **B-2 的 183 名驻厂代表＋GAO＋150 次议员访问，"没有一项为降低成本"**：
   这套系统运作得很好，只是它在做的事不是降低武器成本。
5. **89% 可同厂生产、200 家中只 4 家说不行**，且企业**自己否认了两个官方理由**——
   这是全书方案唯一的实证基础，方法也干净（让企业自己排理由）。

**OCR 甄别**：本批清晰；`IDA`／`Northrop`／`just-in-case`／`cost-plus-fee`／
`activities-based costing`／`form, fit, and function` 可辨；
两处页码栏损坏（`fense employers.`／`130.`）；`$2 million` 处原文有一处
可疑字形但语义与上下文一致（Intel 半导体供应商），照录并标"200 多万美元"。
末句在页界处截断（"要求只引用主文件来避免它……"），**未补全、如实标出**。

**检查**：全库 798 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`，属 1982 年黎巴嫩线，与本书无关）；
表格 alias 违规 0；`SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉞ Gansler 批次十一：第 8 章后段（采购实务／行为惯例／后勤）

**读取范围**：行 5500—5880。军规后半、Procurement Practices、
Business Practices、Logistics Support。

**新建 2 页**

- `concepts/procurement-practices-absurdities-gansler.md`——
  **先修正常见误解**：军规曾是事实上的国家标准，
  **一份 1982 年航空航天报告称约 5,000 项军规被定期用于造商用客机**；
  领先地位已反转：**军标移动电源是 25 年前的设计**，
  效率更低、污染更大、可靠性更差，**无商业供应商故只能专门造、花大价钱**；
  空军自查索引：**45% 的规格超 5 年、29% 超 7 年**；
  **五种替代核证方式**（第三方认证如 UL／合格制造商／国际标准／
  国防部评估承包商内部标准／验收测试）；
  **DFARS 211 早禁止对商业物品用军规，"问题当然是，它并不常被适用"**
  ——**"政策存在 ≠ 政策生效"第四次**；1994 年国防部长指示＋国会法案，
  他写"影响仍有待观察"；
  **马丁·马丽埃塔同一颗通信卫星的两份提案：
  给私营企业 1,000 美元／10 页，给政府 100 万美元／10,000 页**——
  **产品一样、客户不同、成本差 1,000 倍**；
  周期 **9—12 个月 vs 2 个月**（小型）、**18—36 个月 vs 5—6 个月**（大型）；
  **抗议制度**：1984《竞争与合同法》鼓励落败者抗议，
  **1984—1991 申诉增 63%（2,071→3,372）**；
  软件密集系统（布鲁克斯法）**超 90% 授标被抗议、约 40% 需重竞标**，
  《平等司法机会法》还由政府支付抗议者费用；
  他的评语**"这些法律显然正在达成其预期目标——然而代价是效率与有效性"**；
  **GAO：同型号商用示波器卖陆海空三军，需应对 205 条合同条款，
  重叠仅 12%**；出路是**《统一商法典》**；
  题眼：**"今天的目标是完美——包括绝对公平与防止任何错误……完全缺失的是对效率的任何考虑"**；
  戈尔工作组第一条采购建议：**把 1,600 页《联邦采购条例》从僵硬规则转为指导原则**
  （与"125,000 页规章"口径不同，一处标出）
- `concepts/logistics-and-business-practices-gansler.md`——
  **一年一预算**：**美国是世界上唯一按一年做财政规划的国家**，
  其他国家用滚动多年预算（每年辩论第五或第六年、放出一年的钱）；
  **唯一例外是海军北极星／海神／三叉戟项目（至少三年承诺），
  持续受国会与 GAO 赞扬**；风险可按**精算**处理而不必逐年计提；
  **企业计划（Enterprise Programs，1980 年代）**允许按里程碑做多年预算，
  **而国防部选择不用，因为会失去预算灵活性**；
  **"国会改约 50%、国防部改几乎全部，双方都有责任"**——
  **"政策存在 ≠ 政策生效"第五次，但拒绝理由是主动的**（灵活性 vs 效率）；
  **分阶段采办**：每个点都要证明"应该继续"、**为重大决定停六到九个月**，
  而**商业的可见性与控制更多、只是进度驱动**；
  **试验与鉴定**：商业"找失效并持续改进" vs 军事**期末考／审计**，
  **"测试被设计成不会失败"，故学到的东西极少，缺陷发现晚而非早**——目的倒置；
  **数据权**：政府要全部专有数据**以便能创造未来的竞争者**，故许多企业拒绝国防业务；
  **后勤（本页最硬）**：**波音承诺任何商用飞机零件 24 小时内送达全球**；
  **卡特彼勒同一批零件：商业渠道本土 1—2 天／海外偏远 2—4 天且超 4 天退钱，
  军方渠道本土 21—36 天／海外 50—68 天**——**变量只有一个：走谁的渠道**；
  **沙漠盾牌每日申请峰值 35,000 件 vs UPS 平均 1,150 万件／日**；
  **"承包商不会到场"被战争本身反驳：越战与沙漠风暴承包商都在场，
  沙漠风暴有三十多家企业 4,500 人在波斯湾**，
  且这些人多为前军人、由企业培训过新装备；
  **保障可写进合同、按报销人工材料计、不付待命费**

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **波音 24 小时 vs 卡特彼勒军方渠道 68 天**，且是**同一批零件**：
   全书最无可辩驳的对照，变量被压缩到一个（走谁的渠道）。
2. **试验与鉴定的目的倒置**（"测试被设计成不会失败，所以学不到东西"）
   是全章最深的一层——不是激励不足，是**目的本身被换掉了**。
3. **企业计划：国会立了法，国防部选择不用**——"政策存在 ≠ 政策生效"的第五次，
   且这次拒绝是**主动**的：对官僚而言**灵活性比效率值钱**。
4. **"国会改 50%、国防部改几乎全部，双方都有责任"** 是全书对军方自身最公道的一句。
5. **4,500 名承包商就在波斯湾**：对"承包商不会到场"的反驳来自 1991 年那场战争本身。

**OCR 甄别**：本批清晰；`Polaris/Poseidon/Trident`／`Enterprise Programs`／
`Underwriters Laboratory`（原文如此，实为 Laboratories）／`Caterpillar`／
`Uniform Commercial Code`／`DFARS 211`／`Intelsat`／`Geosat` 可辨；
`today’s equipment ts` 一处字形错误（应为 is），按文义照录；
"美国是世界上唯一按一年做财政规划的国家"本批已读完整句，前批截断处补全。

**检查**：全库 800 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`，与本书无关）；表格 alias 违规 0；
`SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉞ Gansler 批次十二：第 9 章前半（三部分战略与公众信任）

**读取范围**：行 5919—6280。A Three-Part Transformation Strategy 前半
＋ Public Trust 前半后半。

**新建 2 页**

- `concepts/three-part-transformation-strategy-gansler.md`——
  开篇第一句是最后一句：**"归根结底，转型取决于个别工厂管理者的日常决定"**
  （政策只创造条件）；
  **三部分战略逐条照录**：① 移除壁垒＋提供指南与激励；② 通过鼓励迅速应用
  最先进产品与制造技术确保关键技术领导地位；③ 劳动力各层级的人力资源开发；
  **"改革推力必须由产业引领"**；
  三项政府投资回报率〔Gansler 口径〕：**研发 15—25%／劳动技能至少 15%／
  基础设施约 12%**；
  **本批最重要的数字矛盾：初始转型需 3—5 年、完全实施最多 10 年，
  而政治官员平均在位 2.5 年**——"政府来回摇摆，没有长期一致持续的方向"；
  国会那一环他定性为"不是政治问题，而是特殊利益不在美国最佳利益轨道上"，
  论证是**把 10 万美元以下采购锁给小企业＝把小企业关进萎缩市场**；
  **七种市场调节工具**（产业联合体／多家企业分领域资助／补贴资本投资／
  融资激励／直接采购创造第二来源／幼稚产业保护／贸易政策），
  但**"最好的手段是重大合同授标"**——因为授标是已有动作、不需新立法；
  具体化为三句可写进授标的话：**"这个部门要三家"／"关键工程与制造在国内"／
  "军民在同一厂房"**；**并给予机床、超级材料、软件、电子元件与坦克飞机同等关注**；
  明确否认**"高度干预主义工业战略"与"美国通产省（MITI）"**，
  **"重点不是单个企业，而是部门的结构"**；
  **国会工作人员那句"这行不通——因为有承包商贪婪"**（承认逻辑清楚、能省数十亿，
  然后说行不通）；
  **公众五关切全部有效**（必要／公平价格／符合预期／公平可及／欺诈滥用），
  而现行制度解决不了且鼓励滥用：**"镀金"因为利润按成本百分比给、
  不投资效率因为降成本会降利润**；只有两条路，
  而**"自由市场是美国方式，监管更容易实施"**
- `concepts/market-tools-for-public-trust-gansler.md`——
  **"几代领导人几乎每天都在说教自由市场，却一直选监管"**（知行不一，不是缺认识）；
  **六项工具**：① **扩大竞争并改变竞争单位**——用性能规格取代详细设计规格、
  用共同的形式配合功能规格（航空公司让产品可互换的做法）；
  **功能竞争的具体三选项：有人突防轰炸机／防区外飞机发射导弹／陆基弹道导弹**
  ——正是第 8 章说"被需求流程挡在决策者之外"的那组，本批变成采购规则；
  ② **类比市场调研**（避免 12 美元锤子卖 500 美元）；
  ③ **按以往业绩而非未来承诺选商**（新进入者交"投标样品"、小企业可获特别贷款），
  并指出**"当前体系只需做到够用，注意力放在下一次投标"**；
  ④ 单一来源的四种监控（独立市场与成本分析／长期监控唯一生产者／
  总有更新的替代品／持续监控国内外市场）；
  ⑤ **停权与除名 → 企业自律 → 可撤掉外部监管**（不需立法的改动）；
  ⑥ 本来就有的民事法律＋专家称"可接受的风险"，条件是"更好的培训"；
  **最难的一项他直接承认监管失败**：**"当前的监督系统运作得不好——如果它运作的话"**
  （而是否必要正是加监管最多的地方），唯一出路是需求流程内部改变＋功能竞争；
  **猪肉桶政治**："选区看作好处、地方新闻正面报道、全国新闻不鸟
  （读者假定'国会就这么办事'）、议员不指责同僚因为自己也在做"，
  他的办法**"把成本放在聚光灯下"**——本库注明这是他自认力度不足的建议；
  **"买家不该关心供应商赚多少，只要自己拿到公平价格"**；
  **"buying in"（低报再解释）是承包商与军种双方共同参与**，不可只归一方

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **3—5 年／10 年 vs 官员平均在位 2.5 年**：全书最根本的矛盾，
   比任何武器成本数字都重要——**要做的改革比做决策的人的任期长二到四倍。**
2. **"这行不通——因为有承包商贪婪"** 是全批最有分量的一手记录：
   对方承认逻辑与节省，问题在信念层，因此前八章的数字都不起作用。
3. **"最好的手段是重大合同授标"**：不需要新立法与新预算科目，
   且把 MIMIC 从示范项目升级为授标条件。
4. **"当前的监督系统运作得不好——如果它运作的话"**：他对最难的第五项
   （是否必要）的直接让步，而它恰是监管最密集处。
5. **功能竞争的三选项与第 8 章的反事实成对**：控诉与方案在同一组例子上闭合。

**OCR 甄别**：本批清晰；`MITI`／`Hart Senate Office Building`／
`Rayburn House Office Building`／`buying in`／`bid samples` 可辨；
两处页码栏损坏（`152.   Chapter9`／`procurement` 被拆行）；
一处 OCR 断行（`"` 单独成行后接 `an acceptable risk`）按文义合并。

**检查**：全库 802 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`，与本书无关）；表格 alias 违规 0；
`SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉞ Gansler 批次十三：第 10 章前半（技术领导力）

**读取范围**：行 6766—7150。Technological Leadership 全节前半
＋ Government Role 前半。

**新建 2 页**

- `concepts/technological-leadership-criteria-gansler.md`——
  **四项互补投资**（研发／资本设备／基础设施／教育与培训）＋
  **"赢的国家不是做出原始研发的，而是最快把产品推向市场的"**；
  研发回报率**每年高达 50%**〔Gansler 口径〕；
  **基础设施的历史类比**：上一代以国家安全为由修公路→刺激汽车业，
  这一代是信息基础设施（公共品故私营投资不足）；
  企业研发投资不足的四种原因（无法利用回报／风险太大／
  益处更多归公众／**尤其是负面短期利润影响**）；
  **"这不仅是投多少钱，还有花在什么上、多有效率；以及花在哪里——
  如果制造转移海外，工程很快就会跟上"**（与 FSX"部件能买、系统集成只能从整机学"
  互为两向印证）；
  **"多个小项目比一两个'大科学'项目回报更高"**；
  **五项判据（本页核心）**：**critical／fast-changing／
  linked（食物链：半导体→计算机→电信）／leveraged（不被现有投资水平淹没）／
  vulnerable（易丧失快速获取）**——第五项直接接第 2 章"脆弱性而非依赖"；
  **"大多数美国产业、政府与劳工领袖都是技术文盲，往往有法律金融营销背景"**
  ＋**"利益冲突立法阻碍高科技管理者进入政府"**＝自我强化循环，
  他称"可能是致命缺陷"，因为**政府出全国约 50% 研发资金**；
  **1994 财年政府研发 755 亿美元、56%（425 亿）为军事**；
  **非国防研发占 GNP：日 3.0%／德 2.75%／美 1.9%（1990）**——已标口径；
  **范内瓦·布什 1945《科学：无尽的前沿》**：确立联邦科学政策，
  **但政府不承担技术开发角色**；当时"技术强科学弱"，**今天正好相反**；
  **他给自己方案列的两条风险**：政府投资不够市场驱动、
  **可能只是替代产业的钱而不是净增益**；Branscomb 三条指南；
  **"预期价值必须在投资之前被明确识别"**
- `concepts/arpa-model-and-rd-tax-policy-gansler.md`——
  **五项资助纪律**（成本分担／产业参与启动与设计／投资多元化／
  **项目选择脱离政治过程**／严格评估）；
  **制度要求**：NSF 与国防部 DDR&E 式的协调组织＋招有工业经验的人＋
  类似 DSB 的外部意见渠道；
  **FCCSET（布什末期，"fix it"）→ NSTC（克林顿更名、升到国安会同级、总统亲任主席）**，
  跨机构委员会、不控预算与项目；
  **六领域 FY93 投入**：先进制造 14 亿／高性能计算与通信 10 亿／
  全球变化 15 亿／先进材料 20 亿／生物技术 43 亿／STEM 教育 23 亿美元；
  **ATP**（NIST 主管、前竞争性通用技术、要求成本分担）／
  **TRP**（1993、ARPA 管理、双用、初始 5 亿、**近 3,000 份提案**）；
  **IR&D 1990 年 36 亿美元、承包商自选方向、政府全额报销**——
  与第 8 章"政府要所有图纸"构成**同合同内的两种信任度**；
  **ARPA 模式五条内核**：少数项目主管＋被给予的自由／
  **执行 100% 在政府之外**／**按"最佳想法"而非报价授予**／
  **同时给不止一家以维持竞争**；
  **"设政府实验室本质是与产业竞争，效果差得多，应劝阻"**，
  而**"近期国会立法显著偏向使用政府实验室"**；
  **税法漏洞完整照录**：**可扣除研发额只相当于企业全球销售额中的美国份额**，
  外国政府又不认海外登记的支出 ⇒ **要么放弃扣除，要么把研发搬出去**；
  **受影响最直接的是资助美国大部分私人研究的大企业**（转移相对容易）

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **五项判据**（critical/fast-changing/linked/leveraged/vulnerable）
   是全章最可搬用的工具，且每一条都能否证一个具体申请。
2. **"制造转移海外，工程很快跟上"** 与 FSX 案例是同一因果的两向印证：
   **能力跟着整机走，整机跟着制造走。**
3. **ARPA vs 政府实验室**：两种做法都已存在、结果不同——
   **少量主管＋自由＋外部执行＋按想法授予＋多家中标**；
   而"立法偏向政府实验室"说明制度惯性又反向走了一步。
4. **税法漏洞**是本批最具体的一条：**不是美国研发贵，
   是美国的研发在海外卖得越多、扣得越少**，于是最先搬走的是最有能力做研发的企业。
5. **"政府出全国一半研发资金，而多数领袖是技术文盲"**：
   钱最多的一方最不懂技术，且利益冲突法把懂的人挡在外面。

**OCR 甄别**：本批清晰；`FCCSET`／`NSTC`／`ARPA`／`ATP`／`TRP`／`IR&D`／
`Branscomb`／`DDR&E` 可辨；表 10.1 表头**完全损坏**（`ee ee ee` 一行），
**不引用其表头，仅记表题与所列政策工具**；两处页码栏损坏
（`171`／`173`／`175` 前有多余空格）；
`the council cam provide` 一处字形错误（应为 can），按文义照录。

**检查**：全库 804 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`，与本书无关）；表格 alias 违规 0；
`SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉞ Gansler 批次十四：第 10 章后半（贸易、联合体、并行工程）

**读取范围**：行 7150—7530。税法余下、技术情报、小企业融资、贸易政策、
联合体、CRADA、标准、Branscomb 五条、Defense Needs、Manufacturing 开头。

**新建 2 页**

- `concepts/trade-policy-and-consortia-gansler.md`——
  **财政部的回应"我们需要这些税收来缓解赤字"**，Gansler 评"不灵活的短视
  将不可避免损害国家利益：让别国获得美国最先进技术、把资金从培养下一代
  科学家工程师的美国大学抽走、在别国培养最先进工程师"；
  **技术情报对照（本页最强的一组数字）**：美国情报界监控全球军事技术趋势、
  **"很少提供给国防界以外的人"**；日本科技厅 1988《日本的未来技术：展望 2015 年》，
  **JETRO 是通产省"情报部门"，1957 年成立，有 300 多名政府官员驻美使领馆、
  200 名日本记者协助，数据由通产省在各产业间分发**——
  与本库"情报存在但没送到需要它的人手里"线索**又对上一次**；
  **SBA 贷款"现在主要针对餐饮生意"**、SBIR 应针对关键技术、
  **"防止拿政府钱本身变成一门生意"**；
  **Scherer（哈佛）：美国企业获得高技术进口保护后，实际上削减了该领域的研发投资**；
  **保护主义是"以邻为壑"的负和博弈**；
  **Vernon 的机制**：保护主义联盟三十五年的策略是**"确保问题总是个案处理而非系统处理"**
  ——与第 4 章"基地关闭委员会把逐个决定变成整包表决所以有效"**是同一杠杆的镜像**；
  **Borrus："高科技竞争曾经是企业之间的，现在已是国家及其政府之间的"**；
  **1984《国家合作研究法》→ 头五年一百多个联合体 → 1989 扩展到生产**；
  **"对右派说绕过反托拉斯、对左派说能规划"**的双向修辞；
  **NAE 四条标准**：① 在美国落后的领域；② 特定狭窄目的；
  ③ **存续期限在成立时确定**（预设退出）；④ **促进行业上下游关系、
  没有内部竞争者**（防止变卡特尔）；
  **Stevenson-Wydler 1980（技术转移成为机构"责任"）→ 联邦技术转移法 1986
  （授权 CRADA，1989 扩到 GOCO 实验室）→ "CRADA 如野花般生长"**，
  指出从"应当做"到"可以用合同做"隔了六年；
  **标准**：私营标准过程"缓慢且资金不足"、政府可资助加速＋鼓励双用标准，
  **"没有标准就会在不合格产品上重复努力"**（与 205 条合同条款那页对上）；
  **Branscomb 五条**＋**"必须敢于停掉项目、启动多种途径、对失败不能有惩罚"**
  ——与"采购过失刑事化"构成正面冲突：**同一个政府两种要求**
- `concepts/concurrent-engineering-and-flexible-manufacturing-gansler.md`——
  **两条路**：找突破（需"更愿意接受偶尔的技术失败"）或把下一代造便宜；
  **McElroy 1958 年："我想要一个机构，确保没有任何重要的事情
  因为不符合某个人的任务而留待未做"**——ARPA 是为绕开军种本位而设，
  三部分战略里唯一的"制度新建"建议；
  **并行工程四例（两军两民）**：波音弹道系统部 **30% 成本节省＋67% 检验比例下降**；
  麦道 TAV-8B **图纸更改 −68%、废品 −58%**；惠普仪器 **开发时间 −35%、现场故障 −60%**；
  约翰迪尔 **开发成本 −30%、开发时间 −60%**；
  **"质量改善要求采购更少系统"**这个反直觉推论（故有制度阻力）；
  **16 天 vs 16 年（本页最惊人）**：沙漠风暴中美国亟需地面车辆敌我识别技术，
  **ARPA 用 16 天设计并交付一套全新系统（完全绕开国防部所有规定的程序）**，
  而国防领域新产品实现周期**平均超过 16 年**——
  **方法（绕开程序）与结果（快 365 倍）直接相连**；
  **380 亿美元年度研发几乎全给"新产品最大性能"，先进制造只留"微不足道的数额"**；
  制造技术的新焦点是**信息技术与仿真建模**（"再造"，不是仿真现有流程）；
  **作业成本法试行 1991—1993 从 11 家活跃参与者降到 2 家**——
  **示范项目会死，授标条件不会死**（与第 9 章互补）；
  **造船：德国 16 个月 vs 美国 30 个月**，"可以想象美国重回造船业"；
  **NSA 保密电话：开发时间 5:1、生产成本 10:1**——双用最硬的一次量化，
  且它是保密要求最强的项目；
  **"总会需要少数非常昂贵的投资"**（新飞机研发 20—40 亿美元、
  新发动机或新半导体设施各超 10 亿美元）——对"15% 上限"的限定；
  **柔性制造**：定义是"在小批量里达成大批量效率"、五大理念
  （准时制／产品工艺一体化／全面质量管理／企业集成／**工人赋权**）、
  **关键指标是缩短换线时间**、**主要由日本人发展**

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **16 天 vs 16 年**：全书最有冲击力的数字对，且方法—结果直接相连，
   不留给"美国人不行"的误读空间。
2. **Scherer 的发现（保护使被保护者减少研发）**：推翻保护主义最常用的自我辩护。
3. **Vernon 的"个案化 vs 系统化"**与基地关闭委员会"整包表决"
   **是同一杠杆的镜像**——本库能给出的最清晰的制度原理。
4. **JETRO 300 名官员＋200 名记者** vs **美国情报"很少提供给国防界以外的人"**：
   "情报没送到需要它的人手里"的第五次记录，且这次是和平时期的。
5. **NSA 保密电话 5:1／10:1**：双用主张最硬的一次量化，
   且出自保密要求最强的领域。
6. **作业成本法 11→2 家**：方法再好，没有授标条件就会死。

**OCR 甄别**：本批清晰；`JETRO`／`Scherer`／`Vernon`／`Borrus`／`NAE`／`CRADA`／
`Stevenson-Wydler`／`McElroy`／`TAV-8B`／`John Deere` 可辨；
**判断一处原文错误**：Vernon 的机构原文被 OCR 成大学名相近的字形，
按上下文（"also of Harvard"）与人物身份照录为哈佛，**未改动引文内容**；
`a crying need nor just for` 一处字形错误（应为 not just），按文义照录；
`process ehanges`（应为 changes）、`mainly developed by the Japanese`
被拆行致 `largely developed` 前有断字，均已按文义还原并在此说明。

**检查**：全库 806 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`，与本书无关）；表格 alias 违规 0；
`SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉞ Gansler 批次十五：第 11 章前半（劳动力）

**读取范围**：行 7870—8260。第 11 章 The Critical Work Force 前半
（含 Current Problems and Potentials、Engineers versus Lawyers）。
注：本章标题是 **The Critical Work Force**（目录行 147 记作 Human Resource
Development，实为章题不同，以正文页眉为准）。

**新建 2 页**

- `concepts/critical-work-force-gansler.md`——
  **框架句**：旧批量生产模式把工人当**成本**（泰勒制：把每个工人所需步骤分解到最少，
  故技能需求很少，机器取代劳工）；精益模式把劳动力当**最有价值的资产**——
  **过去一百年的工厂是为低技能工人设计的**，所以要求能动性不是意愿问题；
  **劳动力占 GDP 约 70%**；
  **实际工资 1978 年后下降，到 1990 年低于 1964 年**（Figure 11.1，劳工统计局）；
  **"美国工人的梦想越来越难以实现"**；**2000 年劳动力 80% 已在就业**；
  **Public Agenda 五数字**：**23% 说发挥了全部潜力／44% 不多投入／
  75% 说能更有效／73% 说努力与薪酬无关／73% 认为这是努力下降主因**；
  并照录他的双向结论（管理层要鼓励＋工人要自我提升＋
  **多数人高估自己的技能且离校后几乎不提升**）；
  **美国商会：只有 9% 的美国工人相信自己是生产力改进的主要受益者，
  多数认为提高生产力会让他们失业**（其他国家工人期望随公司成长受益）；
  日本劳动省：**自动化企业中整整一半不得不增人以跟上订单**，
  丰田"带人情味的自动化"；
  **功能性文盲**：**13% 美国学生离校无最低阅读技能**（英 10%／法德荷 4%／日 1%）；
  **每五名成年人一名功能性文盲**（不会读招聘通知、不会找零）；
  **每十人中一人受毒品或酒精成瘾损害**；
  **在岗者 20% 功能性文盲 vs 日本 2%**；
  **3,000—4,000 万人在岗且功能性文盲**；**一线工人三分之一是高中辍学生**；
  **5,000 万人需要额外培训才能有效履行现有工作**；
  **21—25 岁三项测试按族裔分列完整照录**（找新闻信息 60/40/25、
  看公交时刻表 25/7/3、两份菜单找零 44/20/8）；
  **只有 11% 获得公司正式培训**；**40% 的工人现职不到两年**；
  **维护设备花设备成本 11%，维护员工技能花薪资成本不到 2%**；
  **Marshall 与 Tucker："我们的一线工人可能是所有主要工业国家中技能最低的"**；
  **大学/非大学工资差 1979 年 30% → 1989 年 80%**；
  **即时培训（just-in-time training）优于通用再培训**——
  转换立法大部分培训"针对正在离开岗位的工人"，而通用再培训无效
  （无动机、新岗位未界定）；
  **临时性劳动力占 25%、预计 2000 年达三分之一**；
  **晋升机会从五分之一降到三十分之一**（扁平化的生产好处与激励灾难由同一决定产生）
- `concepts/engineers-versus-lawyers-gansler.md`——
  **小学一年级就把孩子对科学的兴趣关掉了（康奈尔 Corson）**；
  **全国科学教师协会公开承认 50% 成员没资格教其所授课程、小学阶段估计 95%**；
  **工程师知识半衰期约五年**，而多数教学与从业者离校远超此年限；
  **死亡螺旋全文照录**（教得差→无兴趣→企业缺工程师→迁往海外→
  更少岗位与激励→螺旋下行）；
  **制造工程：1987 年全国仅两校授学位、42 名毕业生 / 75,735；
  从业者仅 4% 有工程学位**——与第 10 章"380 亿研发几乎不给先进制造"同构的人才侧；
  **0.5% vs −0.3%**（多 10% 大学生学工程 → 增长率每年 +0.5%；
  法学院人数翻倍 → 每年 −0.3%）与 **100:1,000 vs 1,000:100** 之比；
  **律师数字**：**1987 年日本 18,000 vs 美国 50 多万**；
  **每 6,693 人一名 vs 每 360 人一名**；**1990 年美国 756,000**；
  **美国一年毕业的律师比全日本现有还多**；
  **司法部 FY82—FY88 +30.4% vs 教育部 −31.6%**；
  **1993 年华盛顿 80,000 名游说者**→"持续如洪水般的规制与诉讼，
  与效率正好相反"——**规则数量与制定规则者的职业供给有关**（接第 8 章 5,000 条法律）；
  **激励错位**：产业高管来自法律/金融 vs 日德来自技术界，
  **"市场激励会在上大学时劝阻学生"**；与英国衰落的类比照录；
  **反向论证（本库特别标注）**：**美国工程研究生一半以上是外国学生，
  许多人回国后成为欧美日高技术企业的骨干**——
  **底层教育差与顶层培养强同时成立**；若"人才在不在国内"是问题，
  **解法在移民与薪酬政策，不在教育部**

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **"维护设备 11%、维护员工技能 2%"**：全章最有说服力的一句，
   因为不需要价值判断——同一家企业在两件事上的投入比是 11 比 2。
2. **"只有 9% 相信自己是生产力改进的受益者"**：最令人不安的数据，
   **它是预期问题不是技能问题**——当改进必然伤害做改进的人时，任何培训都没用。
3. **"1990 年实际工资低于 1964 年"＋"2000 年劳动力 80% 已在就业"**：
   政策目标不在学校，在已经在岗的几百万人。
4. **"1987 年全国两所学校授制造工程学位、42 个毕业生"**：
   在提倡柔性制造的国家里，几乎没人在学校里学过怎么造东西。
5. **反向论证**：美国培养的工程师大量回国成为对手的骨干——
   本库据此指出解法不在教育部而在移民与薪酬政策，且这一条与"底层教育差"不矛盾。

**OCR 甄别**：本批清晰；`Taylorism`／`Public Agenda`／`Marshall and Tucker`／
`Corson`／`automation with a human touch` 可辨；
**Figure 11.1 图形数据不可读**（仅存轴标与年份乱码），
故未引用图中任何数值，**只引用正文"1990 年低于 1964 年"这一表述**；
两处页码页眉损坏（`f iit`／`202   Chapter 11`）；
`國際`一处应为"国际"，已改；`recéived`／`teh`类字形错误按文义照录。

**检查**：全库 808 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`，与本书无关）；表格 alias 违规 0；
`SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉞ Gansler 批次十六：第 11 章后半（学校、兵役培训、国际对照）

**读取范围**：行 8260—8660。学生补贴余下、The School System、Industry、
Government Education and Training、Training in Other Countries。

**新建 1 页**

- `concepts/schools-and-training-comparative-gansler.md`——
  **NSF：约 75% 拿系里资助的工程研究生是外国公民**，
  资金部分来自州补贴学费与**国防部研究经费**；
  **"这些工程专业实际上充当了一个美国补贴的技术转移项目"**——
  **"国防部实际上在相当程度上补贴了美国的外国竞争者"**
  （本库注明这不是排外论证，他的解法是提高本国基础教育）；
  **机构臃肿三对照**：政府就业已超制造业就业；
  **陆军军官 +7%、士兵 −3.5%（1980—1991）**；
  **学校非教学人员 +102%、学生 −8%（1965—1985）**；
  **纽约市 7,000 名官僚、每生每年近 7,000 美元**（"行政涅槃"）；
  **"问题基本上不是钱"**：每生实际支出 **1970 年约 2,700 → 1992 年超 5,000 美元**，
  而 **SAT 语文 460 → 420**；
  **1945 vs 1985 学校问题清单**（嚼口香糖/上课讲话 → 毒品/抑郁/自杀/怀孕/强奸）
  ——本库明确标注**两份调查不可作等价量化比较**；
  **联邦只占教育支出 6%（1980 年 9%）**，
  而他认为分权是可取的（**"研究表明校长与教师的独立性是最大贡献因素"**），
  联邦该做的是**国家测试标准、公布各校结果、研究信息技术潜力**；
  **教育部研发预算仅 3.5 亿美元＝本部预算不到 1%、全国教育支出的 0.1%**——
  与第 10 章"380 亿几乎不给先进制造"同一种错配；
  **国防部每年培训 25 万新兵（从基础读写到电子技师与飞行员）**，
  裁军将使美国失去**最大的成人基础教育与技能培训项目**，
  且**"在别处很难替代，因为军事环境与同辈群体的影响是独特的"**——
  全书唯一无法市场化替代的论点；
  **"每隔四到八年把公司所有高管换成该行业没经验的人"**的类比；
  利益冲突解法是**回避＋监督**（比第 10 章更具体）；
  他国视公务员为精英队伍 vs 美国视政府为"最后才考虑的雇主"；
  **德国学徒 170 万 vs 美国 30 万（人口仅四分之一）、企业出资约 70%、
  17 岁中 50%+ 注册、书面考试与认证保证可转移**；
  **瑞典 58%/54%/43% 过去一年参加过教育，学习圈 260 万人（人口 840 万）**；
  **1992 年：每百名雇员美国 12 条建议 vs 日本 3,664 条；提建议者 9 vs 75**；
  **Roos 表 11.1（1989，本页核心否证）**：
  建议数 **日本本土 61.6 → 北美日资 1.4 → 北美美资 0.4**；
  新工人培训小时 **380.3 / 370.0 / 46.4**；
  团队劳动力占比 日本 69.3%、欧洲全部 0.6%（另两格 OCR 损坏不可用）；
  **本库分析**：培训差 8 倍是雇主带来的（可复制），
  但**给了 370 小时的日资美国厂，建议数仍只有日本本土的 2%**
  ⇒ **培训可以复制，参与习惯不能靠培训复制**——这是对他"培训是关键"的最强限制；
  **18,000 日本人在美留学 vs 900 美国人在日；5,000 日本科学家在美实验室 vs <150**；
  **1993 年日语成为 MIT 第一外语、哈佛第二**；
  **英国国家小学课程＋每校自主预算；法国学前 85%/100% 覆盖**；
  落点是**"教师素质——而这恰恰是美国没有强调的"**（页界截断）

**更新 2 页**：来源页、`index.md`

**本批关键判断**

1. **Roos 表 11.1 是全书最好的一次混合设计比较**：
   同时控制国别与雇主国籍，于是能分离出——
   **培训可以转移（日资在美国也给 370 小时），参与文化不能转移（建议数只剩 2%）**。
2. **"美国补贴的技术转移项目"**：75% 的受资助工程研究生是外国公民，
   钱一部分出在国防部账上——这是"人才外流"最具体的会计形式，
   而他的解法不是限制外国人，是提高本国基础教育与教师地位。
3. **国防部每年培训 25 万新兵，是美国最大的成人基础教育项目**：
   裁军的代价被算到了本库没有预料的地方，且**无法被市场化替代**。
4. **教育部研发 3.5 亿／占全国教育支出 0.1%** 与 **380 亿几乎不给先进制造**：
   **两条最大的资源错配，错法完全一样**。
5. **1945 vs 1985 的问题清单**冲击力最大，但也最需要小心——
   本库已标注两份调查不可作等价量化比较。

**OCR 甄别**：本批清晰但**表 11.1 三格损坏**：
`FAM}`（团队占比，北美日资）、`I hes8)`（团队占比，北美美资）、
`733`（欧洲培训小时，**推定 73.3**）；
表格数字与正文引述的"日本 61.6 / 北美日资 1.4 / 美资 0.4"
与"380.3 / 370.0 / 46.4"**一致，可交叉验证**，故这三个数字可用。
其余：`recéived`、`teh`、`govern-` 类断字按文义照录；
"administrative nirvana"直译为"行政涅槃"并保留英文。

**检查**：全库 809 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`，与本书无关）；表格 alias 违规 0；
`SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉞ Gansler 批次十七：“把价格变成一项军事要求”

**读取范围**：行 8710—9100。第 12 章 Achieving Civil/Military Integration
前半：马基雅维利引语、三个必须理由、60—75% 壁垒、CAS 改编码案、
Sixteen Specific Government Actions 第 1—13 条。

**新建 1 页**：`concepts/sixteen-government-actions-gansler.md`

**本页的核心是一句话**：第 4 条——
**“把一件武器的价格变成军事要求的一部分——类似于性能”**，
**“这一单一步骤将明确创造激励，去引入其他所有效率导向的变革”**。
落实方式：**对目前施加于武器项目的每一项法律、规章、规格与标准，
以及未来拟议的那些，评估其不利的成本影响。**
→ 与第 8 章“85% 的成本在设计阶段就锁死”正好接上：
**如果价格不是要求，就永远不会在概念阶段被讨论。**

**开篇引马基雅维利**（本页最重要的自我定位）：
**“创新者会遭到所有在旧条件下过得好的人的敌视，
而在新条件下可能过得好的人，只是他的半心半意的拥护者”**——
与第 11 章“只有 9% 的工人相信自己是生产力改进的受益者”是同一心理机制。

**可行性估计（第 12 章最实用的一句）**：
**现有壁垒 60% 到 75% 可由行政部门（主要是国防部）无需立法移除**，
其余须国会处理；而**两个最难的障碍是成本型合同与采购流程，
“两者都因国防部的极端解释与适用而变得更糟”**。

**CAS 改编码案（1992-04-17）**：在**总统暂停新规章令**期间发布，
理由是**“经济影响预计微小，因此不需要监管影响分析”**；
而**安达信称之为过去二十年最重要的规章之一**，
结论是**供应商更少、价格更高**。
→ 机制：**不知道影响，所以不必评估；不评估，所以永远“影响微小”。**

**其余要点**：
- 第 3 条：**80% 商业销售的设施 ⇒ 其产出的国防专属物品可定为“商业物品”**
- 第 7 条：**主承包商必须向下传递 80 多条条款，还自己再加**；
  **超过 50% 的成本在供应商与零件层**（接第 2 章“下层最脆弱”）
- 第 9 条：**后勤保障应以承包商为常态，建制能力只在前线这类情况下才正当**
- 第 11 条：**达到 20% 商业销售＋质量与作业成本法认证 ⇒ 豁免全部国防专属法律**
  （不用罚款不用补贴，用豁免权作奖品，对政府零成本）；
  **审工艺质量而不只是产品质量**；帕卡德委员会 1986 年统计质控受阻
- 第 12 条：**允许合并到两家甚至更低，但须用“扩大的市场定义”维持竞争**
- 第 13 条（首次见到）：**1980 年代买的新设备按国防部会计规则
  必须在商业工作上摊销，造成对工厂一体化的重大抑制**——
  **最想转换的企业，恰好因为过去听政府的话而转换不了**
- 对国会：**“从帝国式规则制定者地位下来”**，每项立法须经
  独立的成本与结构影响分析

**OCR 甄别**：本批清晰；`Machiavelli`／`CAS Board`／`Arthur Anderson`（原文如此，
实为 Andersen）／`Packard Commission`／`Panel 800` 可辨；
`60 and 7S percent` 一处字形错误（应为 75），按上下文照录为 75% 并注明；
`Dob’s`（应为 DoD's）多处字形错误按文义照录。

**检查**：全库 810 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`，与本书无关）；表格 alias 违规 0；
`SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉞ Gansler 批次十八：第 12 章中段（文职削减与全有或全无）

**读取范围**：行 9100—9300。第 14—16 条、Table 12.1 十六条全表、
The Defense Production Act、Complementary Broad Government Actions 前半。

**新建 1 页**：`concepts/government-downsizing-and-all-or-nothing-gansler.md`

**本页最有价值的是第 15 条的推理链**：
**“如果没有刻意移除不再需要的政府人员，
只会出现人员从一个职能转移到另一个职能；
某一领域移除的规章与过度监督，会在别处增加”**
⇒ **唯一办法是把文职劳动力减少 30% 到 50%**。
→ 这是一个量守恒式判断：**规章总量不取决于需要多少监管，
取决于监管者的数量**；也解释了第 8 章“国防部几乎不反抗加监管”——
**对一个机构来说，人就是权力本身。**
对照：戈尔 1993 工作组建议五年削减 **252,000 人（约 12%）**；
**30—50% 是 Gansler 主张，比现实方案激进四五倍**，已标明。

**最好的制度设计（基地关闭委员会模式的扩展）**：
国防工业的公共部门（大修厂、实验室、兵工厂）在国会影响力太强，
**“可能无法一个一个地关掉”**，因此建议设立
**“国防工业公共部门合理缩减委员会”**，以基地关闭委员会为模板、
由国会授权，**定期提交全有或全无的平衡削减清单**
（或直接用基地关闭委员会本身）；
**同样的“全有或全无”用于立法**（卡内基委员会研究亦认可），
理由：**“仅仅是为了让国会去做他们知道必要、却无法让自己单独去做的事”**。
→ 这是对第 7 章“703 个实验室、69% 维修在建制内”给出的唯一可行解法。

**Table 12.1 十六条完整照录**（OCR 清晰）。
**本库发现全表的共同语法**：第 6、7、11 条都带“除非获得书面豁免”——
**不是禁止，是“默认商业、例外需签字”，举证责任被反过来。**

**《国防生产法》第三条**：历史用途是刺激海外依赖材料的国内产能
（两阶段、政府作“最后买家”）；
**1992 年重新授权把重点转向双用**；
**新用法（本页最漂亮的一处制度复用）：资助行业标准原型、测试与鉴定，
但不进入生产，生产与营销由竞争的企业自己负责**
（实例：开放式架构数字控制机床控制器）；
**而“只能采购与采购承诺”的限制只是 OMB 与国防部之间的一纸跨机构协议，
改起来很容易**——卡住的不是法律，是没人去改那张协议。

**多年预算（与第 8 章接上并给出具体方案）**：
**没有其他发达国家按一年期财政计划运作**；
建议**滚动三年**（国会预算流程已为此准备）；
**两年不够**，理由是第二年末的不确定性。

**另外**：第 16 条要求**基于产出指标**监测转型，
而**外部顾问小组不应拥有自己的权力**（避免出现两套倡议）。

**OCR 甄别**：本批清晰；`Table 12.1` 文字完整可读；
`Dob’s` 字形错误按文义照录；
`buyer of last resort`／`continuing resolutions`／`all-or-nothing` 可辨。

**检查**：全库 811 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`，与本书无关）；表格 alias 违规 0；
`SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。

## 2026-11-18 · 来源㉞ Gansler《Defense Conversion》批次十九 + **全书验收收口**

**读取范围**：行 9300—9540。第 12 章末（出口管制、技术情报、
Overcoming the Resistance to Change）+ **Conclusion**。
**ch1—ch12 正文全部读完**；Notes（p.241 起）与 Index 未读。

**新建 1 页**：`concepts/why-this-reform-might-succeed-gansler.md`

**本页核心是七条失败原因**（可复用清单）：
① 目标未被实施组织与最高管理层完全接受；② 威胁到岗位／存在被感知的利益冲突；
③ 意图传达很差；④ **没有激励，而变革对风险厌恶群体意味着风险**；
⑤ **预测了节省就削减资源，没有认识到变革本身要花钱、收益需时间**；
⑥ **领导层无持续支持，实施期常长于政务官任期**；⑦ **没有产出指标**。
→ 本库判断：**第 5 条是一切"效率改革"的共同死因——
改革被当成省钱项目立项，于是它一开始就没有启动资金。**

**他自问"为什么这次会成功"的两个答案**：
① **危机真实**（"一场国防部危机就在眼前"）——
**过去的改革可以失败，因为失败不致命；现在市场消失了**；
② **领导层对齐**（佩里在国防部，克林顿/戈尔/国家经济委员会同方向），
"这是过去不曾成立的条件——当时国防部与白宫内许多人都主张现状良好"。
**七条失败原因 + "启动动作（重组、发指令）不能算成就" +
"至少五年，或许三年才见可测影响" + "必须有超量的沟通"** 全部照录。

**技术情报那句补上了本库一条长线索的制度原因**：
**"历史上美国对国际数据收集采取非常狭窄的看法——主要因为美国通常领先——
所以唯一感兴趣的是收集关于潜在军事对手的情报"**
⇒ **收集目的决定了分发给谁**（回应第 10 章 JETRO 300 人的对照，
以及本库"情报存在但没送到需要它的人手里"的五次记录）。

**出口管制**：清单可大幅缩短，**"多数情况下经济竞争力比国家安全更值得关切"**；
例：**喷气发动机热端设计**是一直成功管制的双用产品。

**结论**：六步变革（准备／承诺／部署／行动／强化／测量反馈）；
**"字面上数百亿美元"**〔Gansler 口径〕；
**最后一句是警告清单而非希望**：**"规模小、高度补贴、低效、无效、
无竞争力、技术上过时，既无激增能力、也无任何民用益处"**——
本库逐项对应到前文证据（15% 上限／公共部门与国会保线／效率低 30%／
45% 规格超 5 年／第 3 章／备用产能论点）。

---

## Gansler《Defense Conversion》全书验收（19 批）

**来源**：Jacques S. Gansler, *Defense Conversion: Transforming the Arsenal
of Democracy*, MIT Press, 1995（Twentieth Century Fund 资助）。
Internet Archive 扫描 OCR 版，300 页；原文存
`raw/papers/gansler-defense-conversion/`（PDF 15M + TXT 692K）。

**产出**：**34 页**（来源 1 + 概念 33），分 19 批，覆盖 ch1—ch12 正文全篇。

**页目（按章）**
- 来源页：`sources/gansler-defense-conversion`
- ch1：`post-cold-war-defense-drawdown-gansler`、
  `weapon-cost-growth-and-procurement-cycle-gansler`
- ch2—ch3：`us-industrial-policy-precedents-gansler`、
  `defense-industry-vulnerability-tiers-gansler`、
  `four-sector-restructuring-cases-gansler`、
  `foreign-dependency-defense-industrial-base-gansler`
- ch4：`defense-firm-contraction-paths-gansler`、
  `congress-industrial-base-politics-gansler`
- ch5：`conversion-lessons-and-failure-rates-gansler`、
  `core-competence-and-rd-targeting-gansler`
- ch6：`defense-industrial-structure-options-gansler`、
  `civil-military-integration-gansler`
- ch7：`defense-unique-plants-ceiling-gansler`、
  `craft-industry-downsizing-gansler`、`public-private-duplication-gansler`
- ch8：`integration-barriers-gansler`、`procedural-separation-gansler`、
  `four-barriers-survey-gansler`、`cost-based-contracting-and-milspec-gansler`、
  `procurement-practices-absurdities-gansler`、
  `logistics-and-business-practices-gansler`
- ch9：`three-part-transformation-strategy-gansler`、
  `market-tools-for-public-trust-gansler`
- ch10：`technological-leadership-criteria-gansler`、
  `arpa-model-and-rd-tax-policy-gansler`、`trade-policy-and-consortia-gansler`、
  `concurrent-engineering-and-flexible-manufacturing-gansler`
- ch11：`critical-work-force-gansler`、`engineers-versus-lawyers-gansler`、
  `schools-and-training-comparative-gansler`
- ch12：`sixteen-government-actions-gansler`、
  `government-downsizing-and-all-or-nothing-gansler`、
  `why-this-reform-might-succeed-gansler`

**全书五个最重要发现**
1. **"军民分离的原因是程序性的，不是技术性的"**（ch8）——**89% 的企业说
   不同产品可以在同一设施里造，200 家中只有 4 家说不行**，
   而企业压倒性地把原因归于**联邦合同要求**而非技术需要；
   同时**企业自己否认了两个官方理由**（军品没商业市场／商业部门没能力）。
2. **"政策存在 ≠ 政策生效"在本库的第五、六次记录**：曼斯菲尔德修正案（1970，
   明文禁止把企业独立研发分摊到国防合同，1992 才推翻）、
   按成本设计指令（1975／1983，**89 个系统只有 32 个应用，且只在生产阶段**）、
   DFARS 211（早禁止对商业物品用军规，**"问题是不常适用"**）、
   企业计划（1980 年代国会立法允许多年预算，**国防部选择不用**，因为失去灵活性）。
3. **波音 24 小时 vs 卡特彼勒军方渠道 68 天，且是同一批零件**（ch8）——
   全书最无法辩驳的对照，变量被压到一个（走谁的渠道）；
   旁证 **沙漠盾牌每日申请峰值 35,000 件 vs UPS 1,150 万件／日**，
   以及 **沙漠风暴期间三十多家企业的 4,500 人在波斯湾**（反驳"承包商不会到场"）。
4. **把价格变成军事要求的一部分**（ch12 第 4 条）——全书一句话总结；
   落实法：**对每一项法律、规章、规格、标准评估其成本影响**。
   与之配套的机制是 **"80% 商业销售的工厂 ⇒ 其产品可定为商业物品"**，
   以及 **"20% 商业销售＋认证 ⇒ 豁免全部国防专属法律"**（用豁免权当奖品，零成本）。
5. **"某处移除的规章会在别处增加"⇒ 不减人就不可能真正减监管**（ch12 第 15 条）——
   本库读到的最准的官僚系统观察，是一个量守恒式判断：
   **规章总量取决于监管者的人数，而不是需要多少监管。**
   而他主张**文职减 30—50%**，比戈尔工作组的 252,000 人（约 12%）激进四五倍。

**四处需要用户裁定的判断**
1. **本书是"主张书"而非战史**：数据与论点一律标〔Gansler 口径〕。
   最典型的是**研发回报率每年 50%**、**Perry 的每年省 300 亿美元**、
   **转换需要 20—35 年 vs 只有几年时间**这三处内在张力。
2. **ch11 "1945 vs 1985 学校问题清单"**（嚼口香糖→强奸与自杀）：
   本库已标注**两份调查不可作等价量化比较**，但保留其冲击力。
3. **ch11 "美国工程研究生一半以上是外国学生、许多人回国"**：
   Gansler 据此批评教育，本库反向指出**底层教育差与顶层培养强同时成立**，
   若"人才在不在国内"是问题，**解法在移民与薪酬政策**——
   这条标为"本库判断"，与他的原意并列保留。
4. **OCR 不可用的部分**：**表 1.1（核化生与导弹扩散）几乎全废**、
   **表 2.2（前 25 大承包商）大面积损坏**、**表 10.1 表头损坏**、
   **表 11.1 三格损坏**（两格团队占比、欧洲培训小时推定为 73.3）、
   **第 5 章开头一整页图表残片**、**Figure 11.1／11.2 图形不可读**、
   **Notes（p.241 起）与 Index 全为乱码扫描件**。
   **本库一律未使用这些表格与图形中的数据**，仅记表题与出处；
   可与正文交叉验证的（表 11.1 的建议数与培训小时）已注明。
5. **Notes 未读**——因此本书**所有引文无法回溯到原始出处**，
   只能标"据 Gansler 正文"；若日后需精确引用某一数字，须回 PDF 的 Notes 页核对。

**检查**：全库 812 个 md，YAML bad 0；断链 1 处（存量
`entities/people/avner-halutz`，属 1982 年黎巴嫩线，与本书无关）；
表格 alias 违规 0；`SCHEMA.md` sha256 前缀 `191cd20f951e` 未变。
