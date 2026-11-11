# Codex Chemistry Writing Skills

[中文](#中文) · [English](#english)

## 中文

这是一个面向药物化学、天然产物半合成与有机合成论文写作的 Codex Skills 合集。仓库目前包含两个可独立安装、也可联合使用的 Skill，覆盖从 JMC 主文论证到 Supporting Information（SI）实验与表征整理的完整流程。

两个 Skill 均采用证据优先原则：以作者指定的最新稿件、原始实验记录、谱图、仪器报告和药理数据为事实依据；不补写来源中不存在的条件、数值、结构、机制或结论。

### 包含的 Skills

| Skill | 适用任务 | 主要产出 |
| --- | --- | --- |
| [`jmc-manuscript-workflow`](./jmc-manuscript-workflow/) | 天然产物半合成、类似物优化、SAR、药理验证以及 JMC Word 手稿的新稿撰写、续修和数据核对 | 主文结构与论证、Introduction、Results and Discussion、SAR、药理叙事、图表/图注同步、引用与 Word 格式检查 |
| [`edit-si-experimental-procedures`](./edit-si-experimental-procedures/) | 中文、英文或中英混合的合成记录、Scheme 条件、NMR/HRMS 数据和 SI Word 文档 | 规范化实验步骤、General Procedures、Scheme Reagents and conditions、JMC 表征段落、谱图/HRMS 编排和晶体学条目 |

### 如何选择

- 修改标题、摘要、Introduction、Results and Discussion、SAR、药理逻辑、结论、主文图表或整篇 Word 手稿：使用 `jmc-manuscript-workflow`。
- 整理具体合成操作、统一化合物实验步骤、提取 Scheme 条件、处理 NMR/HRMS 或编排 SI Word：使用 `edit-si-experimental-procedures`。
- 同一项目同时包含主文和 SI：先用主文 Skill 固定研究主线、化合物编号和数据权威来源，再用 SI Skill 整理实验与表征；最后交叉核对 Scheme、化合物编号、分子式、收率和分析数据。

### `jmc-manuscript-workflow` 的核心能力

#### 1. 三种工作模式

- **新稿或研究范围发生变化：**先确认文章主题、允许引用的课题组文献以及药理数据范围，再开始撰写。
- **已有手稿续修：**重新打开作者最新修改的文件，沿用已经确认的决定，仅处理当前指定范围，不自动恢复早期版本中已删除的内容。
- **先审阅后修改：**先列出问题位置、数据差异和建议；在用户确认前不改动原稿。

#### 2. 强制的信息确认与来源分级

对于新的研究项目，Skill 会先确认：

1. 改造了什么类型的天然产物或骨架、进行了哪些化学改造、评价了什么活性，以及文章最终落到哪个疾病、模型或机制；
2. “本课题组长期致力于……”等背景段落允许引用哪些课题组论文，以及每篇论文具体支持什么陈述；
3. 是否已有药理数据。若没有，可选择先完成化学部分，或提供最小药理数据包后再写有限度的药理与先导化合物叙事。

原始实验/药理记录负责事实数值，最新稿件负责当前结构、措辞与格式，示例 JMC 文章只用于学习章节逻辑、过渡方式和论断强度，不能替代作者自己的数据。

#### 3. JMC 论证与 SAR 组织

- 将 Introduction 组织为疾病需求、生物学依据、化学机会和本研究目的的递进关系。
- 将半合成结果按药物化学问题组织，而不是按实验时间线堆叠反应。
- 每个 SAR 小节先交代测定背景，再按“结构变量—匹配比较—观察趋势—谨慎解释—下一步设计”的逻辑展开。
- 仅在数据支持时写入浓度依赖、细胞毒性、通路、机制和体内结果，并区分观察、相关性、通路支持与因果机制。
- 未达到化学探针证据标准时使用 `lead compound`，不把先导化合物写成 `probe`。

#### 4. Word、图表与数据一致性

- 保持化合物编号加粗、化学前缀和立体描述斜体、上下标、首次出现的全称与缩写、段落缩进及参考文献悬挂缩进一致。
- 同步 Scheme、反应条件、正文描述、实验步骤、化合物编号、分子式、SAR 图和图注。
- 支持单浓度筛选、剂量反应和 Prism 导出的核对，但不跨越不同实验体系直接比较数值，也不把缺失或未确认的数据写成结论。
- 对 DOCX 采用局部最小修改并生成新版本；工具允许时必须渲染并目视检查。

### `edit-si-experimental-procedures` 的核心能力

#### 1. 实验步骤与 General Procedures

- 保留真实的加料顺序、滴加/分批方式、气氛、温度、时间、终点、淬灭、后处理和纯化过程。
- 统一单位、空格、有效数字、溶剂和试剂缩写以及产品句式。
- 对缺失值使用明确占位符或列入待确认事项，不用常见操作补全未记录的实验。
- 可将系列反应整理为 General Procedure，并保留单个化合物的偏差、纯化、物态、质量和收率。

#### 2. Scheme 条件

- 从相应实验记录独立提取 `Reagents and conditions`。
- 默认保留反应试剂、溶剂、温度、时间及必要气氛；排除用量、收率、淬灭、萃取、干燥和纯化信息。
- 当 Scheme 与详细方法冲突时，以作者指定的实验记录为事实依据并报告差异，不静默拼接两个版本。

#### 3. NMR 与 HRMS

- 按化合物匹配 NMR/HRMS 文件，并保留原始精度、峰型、耦合常数、积分、离子形式、分子式和计算/实测 *m/z*。
- 检查分子式、加合离子、理论值、实测值和 ppm 误差的一致性。
- 不推测缺失峰、不凭结构合理性修正原始数值，也不把不确定的谱图强行分配给化合物。

#### 4. SI Word 文档

- 以作者最新 SI Word 文件为版式基准，按化合物组织合成、表征、NMR 和 HRMS 证据。
- 支持谱图裁切与插入、自动 `Figure S` 编号、HRMS 谱图与报告表格的组合编排。
- 支持 X-ray crystallographic data、精修参数和 CIF 对应信息的整理。
- 完成后检查分页、标题层级、图注、字段、目录、图片清晰度及文档完整性。

### 推荐输入材料

不要求一次提供全部文件，但材料越完整，结果越可靠：

- 作者当前认可的最新主文或 SI DOCX；
- 早期版本（仅用于追溯，不自动恢复旧内容）；
- Scheme/PPT/CDXML、图片及备注；
- 原始实验记录、投料和收率信息；
- NMR/HRMS Word、PDF、谱图或仪器报告；
- 生物活性表、Prism 导出、统计信息和图稿；
- 允许引用的课题组论文及其拟支持的陈述；
- 用于学习写作顺序和风格的 JMC 论文。

### 推荐联合工作流

1. 确认最新版文件、研究主题、改造策略、活性终点和允许引用的课题组论文。
2. 建立文件清单和来源权威关系，明确哪些文件控制化学事实、药理事实、当前措辞和格式。
3. 用 `jmc-manuscript-workflow` 完成或修改主文论证、SAR、图表说明和引用。
4. 用 `edit-si-experimental-procedures` 整理实验步骤、Scheme 条件、NMR/HRMS 和 SI Word。
5. 交叉检查主文、Scheme、Experimental/SI、谱图和表格中的化合物编号与数值。
6. 以新版本名交付，不覆盖作者认可的基线文件。

### 仓库结构

```text
codex-chemistry-writing-skills/
├── edit-si-experimental-procedures/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/
│       ├── jmc-characterization.md
│       └── jmc-si-word.md
└── jmc-manuscript-workflow/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/
        ├── intake-gate.md
        ├── manuscript-architecture.md
        ├── chemistry-pharmacology-rules.md
        └── format-and-qa.md
```

### 安装

#### 方法一：使用 Skill Installer

在 Codex 中调用 `$skill-installer`，提供本仓库地址，并指定要安装的 Skill 子目录。

仓库地址：

```text
https://github.com/1918141147/codex-chemistry-writing-skills
```

#### 方法二：手动安装

1. 克隆或下载本仓库。
2. 将一个或两个 Skill 文件夹复制到全局 Skill 目录：

```text
$HOME/.agents/skills/
```

3. 也可以将 Skill 放入具体项目的 `.agents/skills/`，仅供该项目使用。
4. 如果新 Skill 没有立即出现，请重启 Codex。

### 调用示例

```text
$jmc-manuscript-workflow 请先阅读项目文件，确认文章主题、课题组背景文献和药理范围，再按 JMC 逻辑修改最新版 Word 手稿。
```

```text
$edit-si-experimental-procedures 将这些中文实验记录整理为 JMC SI 英文步骤，同时提取 Scheme 的 Reagents and conditions，并核对 NMR/HRMS。
```

```text
先用 $jmc-manuscript-workflow 完成主文和 SAR，再用 $edit-si-experimental-procedures 按相同化合物编号更新 SI Word；最后检查 Scheme、方法和表征是否一致。
```

### 本次更新重点

- 主文 Skill 增加新稿、续修和先审后改三种模式，以及更严格的来源权威和局部修改规则。
- 完善 JMC 章节衔接、半合成叙事、SAR、药理证据层级、筛选数据和 Word 格式检查。
- SI Skill 新增完整的 Word SI 编排规范，包括按化合物组织谱图、HRMS 报告表格、自动 Figure S 编号和晶体学条目。
- 加强主文、Scheme、实验步骤、NMR/HRMS、图表和结论之间的交叉一致性检查。

### 科学与使用边界

- 始终回查原始实验记录、谱图、仪器报告、统计分析和作者最终稿。
- Skill 不会也不应补写缺失的实验条件、产率、纯度、分析数据、靶点结合或因果机制。
- 示例论文用于学习写作结构，不能作为用户实验事实的来源。
- 当前期刊要求和参考文献状态可能变化，投稿前应再次核对 JMC 官方说明和文献的最终出版信息。
- 使用者对最终科学内容、数据完整性、知识产权和投稿合规性负责。

关于 Skill 的目录结构和使用方式，请参阅 [OpenAI Build skills 文档](https://learn.chatgpt.com/docs/build-skills)。

---

## English

This repository contains two Codex skills for medicinal chemistry, natural-product semisynthesis, and organic-synthesis writing. They can be installed separately or used together to cover the workflow from a JMC manuscript argument to Supporting Information procedures and analytical evidence.

Both skills are evidence-first: the author's accepted manuscript, raw laboratory records, spectra, instrument reports, and pharmacology data govern factual content. Missing conditions, values, structures, mechanisms, and conclusions must not be invented.

### Included skills

| Skill | Best for | Main outputs |
| --- | --- | --- |
| [`jmc-manuscript-workflow`](./jmc-manuscript-workflow/) | New drafts, continuing revisions, SAR, pharmacology, Word editing, and reconciliation of natural-product analogue manuscripts | Manuscript architecture, Introduction, Results and Discussion, SAR, pharmacology narrative, figure/table synchronization, citations, and Word QA |
| [`edit-si-experimental-procedures`](./edit-si-experimental-procedures/) | Raw synthesis records, Scheme conditions, NMR/HRMS data, and SI Word assembly | Experimental procedures, General Procedures, Scheme Reagents and conditions, JMC characterization, compound-grouped spectra/HRMS, and crystallographic entries |

### Choosing a skill

- Use `jmc-manuscript-workflow` for the title, abstract, Introduction, Results and Discussion, SAR, pharmacology, conclusion, main-text figures, or a complete Word manuscript.
- Use `edit-si-experimental-procedures` for detailed synthesis, General Procedures, Scheme conditions, NMR/HRMS, spectra, or a Supporting Information Word document.
- For a combined project, establish the study narrative, numbering, and source authority with the manuscript skill; prepare experimental and analytical content with the SI skill; then cross-check every compound, Scheme, formula, yield, and data label.

### JMC manuscript workflow

- Supports three modes: new/scope-changed manuscript, continuing revision, and review before editing.
- Requires confirmation of the study theme, approved group-publication claims, and pharmacology scope before drafting a new study.
- Uses raw records for facts, the accepted manuscript for current structure and formatting, and example JMC papers only for rhetorical architecture and claim restraint.
- Organizes semisynthesis by medicinal-chemistry questions and SAR by structural variable, matched comparison, observed trend, cautious interpretation, and design consequence.
- Calibrates pharmacology language to the available evidence and reserves `probe` for work that actually establishes and uses a chemical probe.
- Synchronizes Schemes, captions, Results text, Experimental/SI, compound labels, screening data, figures, citations, and Word formatting.

### JMC SI and experimental workflow

- Preserves actual addition order, operations, atmosphere, temperature, time, workup, purification, and observations.
- Produces concise General Procedures and compound-specific procedures without silently supplying conventional but unrecorded operations.
- Extracts Scheme conditions from the same experimental record while excluding workup and purification details by default.
- Matches NMR and HRMS evidence to compounds, preserves source precision, and checks formulas, adducts, calculated/found *m/z*, and ppm error.
- Uses the author's latest SI Word document as the layout baseline for compound-grouped spectra, HRMS report tables, automatic Figure S numbering, and X-ray crystallographic entries.

### Recommended source package

- Latest accepted manuscript or SI DOCX;
- earlier versions for history only;
- Scheme/PPT/CDXML files, figures, and author notes;
- raw experimental records, quantities, and yields;
- NMR/HRMS Word/PDF files, spectra, and instrument reports;
- screening tables, Prism exports, statistics, and figures;
- approved group publications with the claims each paper may support;
- example JMC articles for organization and style.

### Repository structure

```text
codex-chemistry-writing-skills/
├── edit-si-experimental-procedures/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/
│       ├── jmc-characterization.md
│       └── jmc-si-word.md
└── jmc-manuscript-workflow/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/
        ├── intake-gate.md
        ├── manuscript-architecture.md
        ├── chemistry-pharmacology-rules.md
        └── format-and-qa.md
```

### Installation

#### Option 1: Skill Installer

Invoke `$skill-installer` in Codex, provide this repository, and specify the desired skill subdirectory:

```text
https://github.com/1918141147/codex-chemistry-writing-skills
```

#### Option 2: Manual installation

1. Clone or download the repository.
2. Copy either or both skill folders into the global skill directory:

```text
$HOME/.agents/skills/
```

3. Alternatively, place them in a project's `.agents/skills/` directory for project-only use.
4. Restart Codex if the new skill is not detected immediately.

### Invocation examples

```text
$jmc-manuscript-workflow Review the project files, confirm the study theme, approved group publications, and pharmacology scope, then revise the latest JMC Word manuscript.
```

```text
$edit-si-experimental-procedures Convert these mixed-language laboratory records into JMC SI procedures, extract Scheme conditions, and reconcile the NMR/HRMS data.
```

```text
Use $jmc-manuscript-workflow for the main text and SAR, then use $edit-si-experimental-procedures to update the SI Word file with the same compound numbering and cross-check the Scheme, procedures, and characterization.
```

### Highlights of this update

- Adds explicit new-draft, continuing-revision, and review-first modes to the manuscript workflow.
- Expands JMC transitions, semisynthesis logic, SAR, pharmacology evidence levels, screening-data checks, and Word QA.
- Adds full SI Word guidance for compound-grouped spectra, HRMS report tables, automatic Figure S numbering, and crystallographic entries.
- Strengthens cross-document consistency checks across the manuscript, Schemes, procedures, NMR/HRMS, figures, and conclusions.

### Scientific boundaries

- Always verify the original laboratory records, spectra, instrument reports, statistical analyses, and final author-approved files.
- The skills must not invent missing conditions, yields, purity values, analytical data, target engagement, or causal mechanisms.
- Example papers guide writing architecture; they do not establish facts for the user's study.
- Journal requirements and publication records may change. Recheck current JMC guidance and final bibliographic status before submission.
- Users remain responsible for scientific accuracy, data integrity, intellectual property, and submission compliance.

See the [OpenAI Build skills documentation](https://learn.chatgpt.com/docs/build-skills) for the current skill structure and usage model.
