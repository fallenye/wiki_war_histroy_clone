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
