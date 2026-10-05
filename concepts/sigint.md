---
title: 信号情报（SIGINT：Comint／Elint／Fisint）
type: concept
concept_type: intelligence
tags: [concept, cold-war, sigint, intelligence]
sources: [secrets-sigint-cold-war-aid-wiebes]
created: 2026-09-29
updated: 2026-09-29
---

# 信号情报（SIGINT）

**信号情报（Signals Intelligence, SIGINT）**：由截收、分析与参数利用外国**通信及非通信射频发射**而
获得的情报。据 [[secrets-sigint-cold-war-aid-wiebes|Aid & Wiebes《Secrets of Signals Intelligence》]]
（2001）ch1 之定义与分类。本库以此概念页统合“收集/破译”侧，与“对抗/干扰”侧的
[[concepts/electronic-warfare-cold-war-1946-64|电子战（EW）]] 互补。

## 定义与三分支（原书）

- **Comint（通信情报）**：由截收与处理话音、摩尔斯、无线电传、传真、多路（微波中继）与视频信号而
  得；**不含**明文书信邮件、外国公开媒体/宣传广播、反谍调查或战时检查所获通信。
- **Elint（电子情报）**：截收分析外国**电子装置**之发射——最主要目标为各国**雷达系统**（预警、导弹
  探测、地面引导截击、导弹制导、战斗机引导、测高）；经 Elint 可辨其功能与型号、评估其作用距离与能力、
  精确定位。主要服务于军事：**数雷达→定其位→测其程→评其作战体系→研制可干扰防空导弹雷达等之对抗
  措施**。其他目标含导航/无线电信标、**IFF 敌我识别**信号、对抗/干扰设备辐射、导弹制导与引信辐射、
  气象与科研测试装置发射。
- **Fisint（外国仪器信号情报）**：收集处理与**航天/水面/水下系统**之试验与作战部署相关的发射
  （含弹道导弹与有人/无人航天器**遥测**、beaconry、电子询问器、跟踪/引信/解除保险/指令系统、
  视频数据链）——为监视外国武器研发（尤其弹道导弹试验）之主要 SIGINT 手段。
- 新介质：近十年 SIGINT 亦涉**数字数据通信**（NSA 及英语 SIGINT 伙伴称此类数据流代号
  “**Proforma**”，如电子银行转账数据）。

## SIGINT 之内在特性（原书 ch1 归纳九点）

1. **被动收集**、通常不为目标所知；可对**数千英里外**目标收集（截收站无须近目标）→ 一般**政治/物理
   风险小**。**例外**：各方之**海空周边侦察**任务（平台被击毁/俘获）——冷战中共 **146 名** NSA 军/文
   人员殉职（其中 **60** 人死于越南）；**最大一次损失**为 1967-06 以色列攻击 NSA 间谍船 **USS Liberty**
   （34 名海军/陆战队/NSA 文职密码人员死亡）。
2. 客观性与可靠性高（但非尽善）。
3. 覆盖广（含多语言/多领域）。
4. 为冷战期间国安与外交决策者之**首要**情报来源（1966 参议员 Milton Young：NSA 情报对外交政策之
   作用远大于 CIA；1998 John Millis：“决策者与军事指挥官的 **INT of choice**”）；公开使用实例含
   **1964 北部湾事件**、1968 朝俘 USS Pueblo、1958 C-130、1969 EC-121、1983 KAL 007、1996
   Brothers to the Rescue 击落案；1986 对利比亚空袭（据 NSA 截获）。**Humint 单独决定重大政策之例极少**。
5. **最快**之现势情报来源（DIA 前局长 Daniel Graham：“多数收集机构给我们历史，NSA 给我们现在”）；
   NSA 有**专线**送截获至 Fort Meade、另有 SSO 分送网；**1962–1965** 启用 **CRITICOMM**（150 个站
   15 分钟直送华盛顿）；**并在古巴导弹危机后不久设立与白宫的直连线路**，直供总统与国安会关键解密件
   ——绕过 CIA/DIA 分析员。对照：1962 古巴危机时，CIA 在古巴境内的**密写**报告需一周以上才达分析员，
   难民审讯所得常已数月。
6. 产量最大：1964 年 NSA 发出约 **15 万**份成品报告（>400/日）；至 1960s 末翻倍至近 **40 万**/年
   （>1000/日）。对照 KGB：1960 破译 51 国 **209,000** 份外交电报（572/日）；1967 破译 72 国
   **188,400** 份（516/日）。
7. “从不休眠”：全年无休、不受天候影响（对比人力需睡眠、影像受暗夜/坏天气制约）。
8. 灵活、响应任务快——故为冷战快变危机（**朝鲜战争、古巴导弹危机、越南战争**）中**首选**来源。
9. 潜力大于一切其他手段——“破译一主要外方密码体系，一日产出可超其余来源总和”（“一个 break 等于
   一千名安置得当、安全且即时报告的间谍”）；CIA 局长 **Allen Dulles** 亦称 SIGINT 为“最好、最‘热’
   的情报”。

## 本库接口

- 与 [[concepts/electronic-warfare-cold-war-1946-64|电子战·冷战早期]]（Price 卷二）：EW 记**对抗**（干扰/
  欺骗/告警），SIGINT 记**收集**（截收/测向/破译）——Elint 为二者交集（识别威胁雷达以制对抗措施）。
- 相关装备/平台：[[entities/equipment/uss-oxford-agtr-2|USS Oxford（技术侦察船）]]、
  [[entities/equipment/rc-135-signals-family|RC-135 系列]]、[[entities/equipment/ec-121-warning-star|EC-121]]。
- 组织：[[entities/organizations/nsa|NSA]]、[[entities/organizations/gchq|GCHQ]]、
  [[concepts/ukusa-alliance|UKUSA 协定]]。

## 关联

[[secrets-sigint-cold-war-aid-wiebes|来源页]] · [[concepts/ukusa-alliance|UKUSA]] ·
[[entities/organizations/nsa|NSA]] · [[entities/organizations/gchq|GCHQ]] ·
[[wars/cold-war-cuban-missile-crisis/index|古巴导弹危机]] · [[wars/korean-war/index|朝鲜战争]]
