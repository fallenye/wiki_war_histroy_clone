# War History Wiki Schema

```yaml
schema_name: War History Knowledge Base
schema_version: 1.0
default_language: zh-CN
```

## 1. 知识库定位

本知识库用于长期构建战争史、军事史、军事技术史及相关专题研究知识网络。

知识库以“战争”为主要历史导航入口，但不以任何单一战争、军种、装备类别或第一批摄入资料限定整个知识库的范围。

主要研究对象包括：

- 战争
- 战区 / 战线
- 战役、作战行动与重要军事事件
- 战术、条令、战略与军事理论
- 装备与军事技术
- 部队与军事组织
- 人物
- 具有军事意义的地点
- 跨战争专题
- 时间关系
- 原始资料与研究资料

知识库可以逐步扩展到不同历史时期与战争，例如第一次世界大战、第二次世界大战、朝鲜战争、越南战争、中东战争、两伊战争、海湾战争、阿富汗战争、伊拉克战争、叙利亚内战等。

任何单一来源都不得自动重新定义本知识库的 Domain。

---

## 2. 语言规范

- 综合知识页面默认使用简体中文。
- 摄入报告、任务总结、查询结果和面向用户的自然语言回复默认使用简体中文。
- 英文专有名词、装备型号、部队番号、行动代号、书名和技术缩写可保留原文。
- 重要术语首次出现时，推荐使用“中文名称（English Name / Abbreviation）”。
- `raw/` 层保持原始资料语言，不为了摄入而翻译原始文本。
- 原始引文保持原语言。
- YAML key、文件路径、文件名和机器可读字段保持稳定英文格式。

---

## 3. 核心原则

### 3.1 战争负责导航，实体负责知识

战争是用户浏览知识库的主要入口，但不是所有知识页面的物理归属。

例如，F-4 Phantom II 可能参与多个战争，知识库中原则上只保留一个权威实体页面：

`entities/equipment/f-4-phantom-ii.md`

不同战争的装备索引应链接到同一个实体页面，而不是各自复制一份 F-4 页面。

### 3.2 一实体一权威页面

同一人物、装备、部队、组织、地点或概念原则上只建立一个 canonical page。

新来源遇到已有对象时：

- 优先更新已有页面；
- 增加新的来源；
- 增加新的战争、事件和关系；
- 不创建同义重复页面。

### 3.3 文件夹负责导航，Wikilink 负责关系

不要试图依靠目录结构表达所有历史关系。

跨战争、跨战区、跨事件、跨实体的关系主要通过 `[[wikilinks]]` 和结构化 frontmatter 表达。

---

## 4. 基础目录结构

```text
wiki/
├── SCHEMA.md
├── index.md
├── log.md
│
├── wars/
├── events/
│
├── entities/
│   ├── equipment/
│   ├── organizations/
│   ├── people/
│   └── places/
│
├── concepts/
├── topics/
├── timelines/
├── sources/
│
├── raw/
│   ├── papers/
│   ├── articles/
│   ├── transcripts/
│   └── assets/
│
└── _archive/
```

目录只建立当前实际需要的部分，不要求一次创建大量空目录。

---

## 5. 战争层级

### 5.1 普通战争

通常采用：

```text
wars/<war-slug>/
├── index.md
├── timeline.md
├── campaigns/
├── tactics/
├── equipment/
├── units/
├── people/
└── places/
```

这些子目录主要用于战争内部的 Index / MOC 导航，而不是复制实体正文。

建议导航分类：

- 战役与行动
- 战术与条令
- 装备与技术
- 部队与组织
- 人物
- 地点
- 时间线
- 专题研究

### 5.2 大规模世界战争

第一次世界大战、第二次世界大战等规模巨大、内部结构复杂的战争，可以增加 Theater / Front 层：

```text
wars/world-war-ii/
├── index.md
├── timeline.md
└── theaters/
    ├── european-theater/
    ├── pacific-theater/
    └── ...
```

战区内部可以继续使用与普通战争相同的导航分类。

Theater 不是强制层级。

只有战争规模、历史结构或资料复杂度确实需要时才使用，不得为了目录统一而强行给所有战争增加 Theater。

---

## 6. 页面类型

基础页面类型：

- `war`
- `theater`
- `event`
- `entity`
- `concept`
- `topic`
- `source`
- `comparison`
- `timeline`
- `index`
- `query`
- `summary`

---

## 7. 通用 Frontmatter

所有正式 Wiki 页面都必须以 YAML frontmatter 开头。

```yaml
---
title: 页面标题
created: YYYY-MM-DD
updated: YYYY-MM-DD
type: entity
tags: []
sources: []
---
```

按页面类型增加专用字段。

### 7.1 War

```yaml
---
title: 越南战争
type: war
start_date: YYYY-MM-DD
end_date: YYYY-MM-DD
tags: [war]
sources: []
---
```

### 7.2 Theater

```yaml
---
title: 欧洲战区
type: theater
war: world-war-ii
tags: [theater]
sources: []
---
```

### 7.3 Event

用于战役、战役群、军事行动、突袭、攻势、事件和任务。

```yaml
---
title: 滚雷行动
type: event
event_type: campaign
war: vietnam-war
theater:
start_date: YYYY-MM-DD
end_date: YYYY-MM-DD
tags: [campaign]
sources: []
---
```

允许的 `event_type`：

- `battle`
- `campaign`
- `operation`
- `raid`
- `offensive`
- `incident`
- `mission`
- `other`

单日事件可使用：

```yaml
date: YYYY-MM-DD
```

### 7.4 Equipment Entity

```yaml
---
title: F-105 Thunderchief
type: entity
entity_type: equipment
equipment_type: aircraft
wars:
  - vietnam-war
tags: [equipment]
sources: []
---
```

`equipment_type` 可按实际需要使用：

- `aircraft`
- `ground-vehicle`
- `ship`
- `submarine`
- `missile`
- `weapon`
- `artillery`
- `radar`
- `sensor`
- `electronic-warfare-system`
- `communications-system`
- `air-defense-system`
- `other`

如遇新装备类型，可优先扩展 `equipment_type`，不要为了一个具体型号创建新的顶层 `type`。

### 7.5 Organization Entity

```yaml
---
title: 355th Tactical Fighter Wing
type: entity
entity_type: organization
organization_type: unit
wars:
  - vietnam-war
tags: [organization]
sources: []
---
```

`organization_type` 可包括：

- `unit`
- `formation`
- `command`
- `military-service`
- `government-agency`
- `intelligence-agency`
- `militia`
- `other`

### 7.6 Person Entity

```yaml
---
title: Robin Olds
type: entity
entity_type: person
wars:
  - vietnam-war
tags: [person]
sources: []
---
```

### 7.7 Place Entity

```yaml
---
title: 河内
type: entity
entity_type: place
wars:
  - vietnam-war
tags: [place]
sources: []
---
```

只有具有明确军事、战略、战役或研究意义的地点才建立独立页面。

### 7.8 Concept

用于可以跨事件、跨战争存在的战术、理论、技术和作战概念。

```yaml
---
title: 防空压制（SEAD）
type: concept
concept_type: tactic
tags: [tactic]
sources: []
---
```

`concept_type` 可包括：

- `tactic`
- `doctrine`
- `strategy`
- `technology`
- `intelligence`
- `logistics`
- `electronic-warfare`
- `air-defense`
- `other`

---

## 8. 战争 Index

每个战争必须至少拥有：

- `index.md`
- `timeline.md`

战争 Index 负责导航，不复制大量实体正文。

推荐包含：

- 战役与行动
- 战术与条令
- 装备与技术
- 部队与组织
- 人物
- 地点
- 时间线
- 专题研究
- 主要来源

装备、人物、部队等条目链接到 canonical page。

---

## 9. 时间线规范

时间关系是本知识库的核心结构之一。

至少支持三个层级：

1. 全局时间线；
2. 战争时间线；
3. 战役 / 战区 / 专题时间线。

例如：

```text
timelines/master.md
wars/vietnam-war/timeline.md
```

Event 页面应尽量保存结构化时间字段：

- `date`
- `start_date`
- `end_date`

Markdown 时间线建议格式：

```markdown
# 越南战争时间线

## 1965

- 1965-03-02 — [[rolling-thunder]] 开始
- 1965-07-24 — 某重要防空作战节点

## 1967

- 1967-01-02 — [[operation-bolo]]
```

规则：

- 日期必须有来源支持；
- 日期不确定时必须显式保留不确定性；
- 不得为了时间线完整而制造精确日期；
- 战争时间线可以较详细；
- 全局时间线只收录足够重要的事件；
- Schema 不依赖任何特定 Obsidian 时间线插件。

---

## 10. Topic 专题页

Topic 用于组织不能简单归入单一战争、单一事件或单一实体的研究主题。

例如：

- 越南战争电子战
- Wild Weasel 发展史
- 反辐射导弹发展史
- 苏联防空体系发展
- 雷达与反雷达对抗
- 某类战术的跨战争演变

Topic 页面可以综合：

- 多个战争
- 多个事件
- 多个实体
- 多个概念
- 多个来源

Topic 是研究和视频选题入口，不是实体页面的重复副本。

---

## 11. 来源层

`raw/` 与 `sources/` 分工不同。

### raw/

保存尽可能未经修改的原始资料与提取文本。

### sources/

保存资料本身的结构化描述。

Source 页面示例：

```yaml
---
title: 资料标题
type: source
source_type: book
author:
year:
publisher:
raw_file:
tags: []
---
```

`source_type` 可包括：

- `book`
- `journal`
- `report`
- `archive`
- `memoir`
- `interview`
- `website`
- `article`
- `document`
- `video`
- `audio`
- `other`

重要知识必须可以追溯到 Source 或 raw source。

---

## 12. Raw Frontmatter 与重复检测

Raw source 使用小型 frontmatter：

```yaml
---
source_url:
source_path:
ingested: YYYY-MM-DD
sha256: <hex digest>
---
```

`sha256` 用于重复摄入检测。

计算时以 closing `---` 后的正文为准。

重新摄入时：

- hash 相同：跳过重复处理；
- hash 不同：标记 source drift 或来源版本变化；
- 不得静默覆盖旧 raw；
- 原始 PDF 与综合知识页面必须分离保存。

---

## 13. 文件命名

文件名规则：

- lowercase
- 使用 hyphen
- 不使用空格
- 尽量采用稳定英文名称、国际通用名称或公认缩写

例如：

- `f-4-phantom-ii.md`
- `operation-bolo.md`
- `rolling-thunder.md`
- `robin-olds.md`

页面显示标题可以使用中文或中英组合。

---

## 14. Wikilink 规则

使用 `[[wikilinks]]` 建立有意义的历史关系。

推荐关系：

- 战争 ↔ 战役 / 行动
- 战役 ↔ 部队
- 战役 ↔ 人物
- 战役 ↔ 装备
- 战役 ↔ 地点
- 战术 ↔ 装备
- 战术 ↔ 部队
- 装备 ↔ 部队
- 人物 ↔ 部队
- 概念 ↔ 战争
- Topic ↔ 事件 / 实体 / 概念 / 来源

正式综合页面应尽量具有两个以上有意义的 outbound wikilink，但不得为了满足数量要求制造无意义链接。

---

## 15. 页面创建门槛

创建新页面，当：

- 一个实体或概念出现在两个以上独立来源中；或
- 虽然只存在于一个来源，但它是该来源的核心内容；或
- 对理解战争、战役、装备、部队、人物、战术关系具有明显研究价值。

遇到已有页面时：

- 优先更新已有页面；
- 增加新的来源和关系；
- 不建立重复页面。

不要为以下内容建立独立页面：

- 偶然提及；
- 无研究价值的小细节；
- 无军事意义的普通地点；
- 只出现一次且不是核心人物的人名；
- 身份无法确认的对象；
- 单纯为了增加 Wikilink 数量的对象。

页面是否拆分以“是否已经包含多个可以独立研究的主题”为主要判断标准，不机械按固定行数拆分。

---

## 16. 实体页基本内容

重要 Entity 页面应尽量包括：

- 概述
- 关键事实与日期
- 与相关战争的关系
- 与相关事件的关系
- 与其他实体或概念的关系
- 来源

不同实体可以增加适合自身类型的章节。

---

## 17. Concept 页面基本内容

Concept 页面应尽量包括：

- 定义或说明
- 历史背景
- 战术 / 技术 / 理论演变
- 相关战争与事件
- 相关装备、部队或人物
- 已知争议或开放问题
- 来源

Concept 可以跨多个战争持续增长。

---

## 18. Comparison 页面

Comparison 用于明确的对照研究。

应尽量包括：

- 比较对象
- 为什么比较
- 比较维度
- 表格或结构化对照
- 综合结论
- 局限
- 来源

比较结论必须区分事实、来源观点和综合判断。

---

## 19. Provenance / 来源追踪

所有综合知识页面必须在 `sources:` 中记录参与综合的来源。

单一来源页面通常可以仅依靠 frontmatter 的 `sources:`。

多来源综合页面中，如果某段重要论述明显来自特定来源，应增加 provenance marker，例如：

`^[raw/papers/source-file.md]`

不得删除不同来源之间的差异来制造“统一答案”。

不得把模型自身知识伪装成摄入来源内容。

---

## 20. 史料冲突规则

历史资料之间的分歧本身就是知识的一部分。

当新来源与已有资料冲突时：

1. 不因为出版时间更新就自动认为新来源正确；
2. 检查来源性质：一手资料、二手研究、档案、回忆录、采访等；
3. 检查作者使用的证据；
4. 检查双方统计口径是否不同；
5. 可以同时保留多个有来源支持的说法；
6. 明确注明各自来源；
7. 无法解决时标记：

```yaml
contested: true
```

必要时增加：

```yaml
confidence: high | medium | low
```

不得让模型自行选择一个数字或观点，并删除其他有来源支持的说法。

---

## 21. Index 规则

每个新增正式页面都应能从至少一个合理 Index 或相关页面被访问。

全局 `index.md` 主要负责进入：

- Wars
- Topics
- Timelines
- Sources

不要求全局 Index 平铺列出所有实体。

详细导航由各战争、战区或专题自己的 Index / MOC 完成。

---

## 22. Log 规则

每次正式摄入、批量修改或 Schema migration 都应写入 `log.md`。

日志默认使用简体中文。

建议记录：

- 日期
- action
- source
- SHA256
- 新建页面
- 更新页面
- 跳过内容
- Index 变化
- Timeline 变化
- audit 结果
- 需要人工复核的问题

不要在 log 中保存大量模型内部推理过程。

---

## 23. SCHEMA 管理

`SCHEMA.md` 是知识库核心规范。

普通资料摄入不得自动修改以下内容：

- Domain
- Page Types
- Directory Structure
- 核心 Frontmatter 字段
- War / Theater 层级规则
- Naming Rules
- Source Rules
- Conflict Policy

如果现有 Schema 无法表达新情况，执行任务的 Skill 应提出：

`SCHEMA EXTENSION PROPOSAL`

至少说明：

- 遇到的新情况
- 当前 Schema 的限制
- 建议新增或修改的字段 / 类型
- 对旧页面可能产生的迁移影响

只有用户明确批准后才修改 Schema，并更新：

`schema_version`

---

## 24. 普通摄入更新流程

新来源摄入时原则上按以下顺序：

1. 检查 source 是否重复；
2. 保存 raw；
3. 确认相关战争 / 战区；
4. 搜索已有 event / entity / concept；
5. 优先更新 canonical page；
6. 创建达到门槛的新页面；
7. 增加来源；
8. 建立 Wikilink；
9. 更新相关时间线；
10. 更新战争 / 战区 Index；
11. 必要时更新全局导航；
12. 写入 log；
13. 执行质量检查。

任何单一来源都不得因为自身主题而重新定义知识库整体领域。

---

## 25. 基本质量规则

正式页面应优先满足：

- 来源明确；
- 日期尽量明确；
- 人物、装备、部队身份明确；
- Wikilink 有意义；
- 不重复建 canonical page；
- 不删除有来源的争议观点；
- raw source 不被综合内容改写；
- 页面能够从合理导航入口到达；
- Timeline 日期可追溯；
- 综合正文默认简体中文；
- 专有名词准确；
- 不把推测写成确定事实。

---

## 26. v1.0 暂不强制实现

以下能力保留为未来扩展，不作为 v1.0 强制要求：

- 每条史实独立 Claim 页面
- GIS / 地理坐标与地图
- Order of Battle 专用结构
- 编制随时间变化的结构化数据库
- 装备性能数据库
- Obsidian 自动可视化 Timeline
- Dataview
- 图数据库
- 向量数据库
- OCR 页码级引用
- 图片 / 地图 / 表格知识抽取

只有实际需求出现后再升级 Schema。
