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
