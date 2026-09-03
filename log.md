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
