# Codex Chemistry Writing Skills

[中文](#中文) · [English](#english)

## 中文

这是一个面向药物化学与有机合成论文写作的 Codex Skills 合集，包含两个可独立安装和调用的 Skill。

### 包含的 Skills

| Skill | 功能 |
| --- | --- |
| `edit-si-experimental-procedures` | 将中文、英文或中英混合的实验记录整理为可发表的 Supporting Information 实验步骤；提取 Scheme 所需的 Reagents and conditions；按照 Journal of Medicinal Chemistry 风格规范化 NMR 和 HRMS 表征数据。 |
| `jmc-manuscript-workflow` | 为天然产物半合成、类似物优化、构效关系与药理学研究撰写或修改 Journal of Medicinal Chemistry 风格的论文，并在动笔前执行研究主题、课题组文献和药理数据确认。 |

两个 Skill 都遵循“以原始证据为准，不臆造缺失数据”的原则。

### 仓库结构

```text
codex-chemistry-writing-skills/
├── edit-si-experimental-procedures/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/
└── jmc-manuscript-workflow/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/
```

### 安装

#### 方法一：使用 Skill Installer

在 Codex 中调用 `$skill-installer`，并提供本仓库地址以及要安装的 Skill 目录。

#### 方法二：手动安装

1. 克隆或下载本仓库。
2. 将需要的 Skill 文件夹复制到：

```text
$HOME/.agents/skills/
```

3. 如果 Skill 没有立即出现，请重启 Codex。

### 使用示例

```text
$edit-si-experimental-procedures 将这些实验记录和分析数据整理成 JMC Supporting Information 格式。
```

```text
$jmc-manuscript-workflow 根据项目文件修改这篇天然产物类似物研究论文。
```

### 注意事项

- 请始终核对原始实验记录、谱图、仪器报告和最终稿。
- Skill 不应补写来源中不存在的实验条件、收率、纯度或分析数据。
- 使用者对最终科学内容、数据准确性和投稿合规性负责。

关于 Skill 的目录结构和使用方式，请参阅 [OpenAI Build skills 文档](https://learn.chatgpt.com/docs/build-skills)。

## English

This repository contains two Codex skills for medicinal chemistry and organic synthesis writing. Each skill can be installed and invoked independently.

### Included skills

| Skill | Purpose |
| --- | --- |
| `edit-si-experimental-procedures` | Converts Chinese, English, or mixed-language laboratory records into publication-ready Supporting Information procedures; extracts Scheme-ready reagents and conditions; and standardizes NMR and HRMS characterization in Journal of Medicinal Chemistry style. |
| `jmc-manuscript-workflow` | Drafts or revises Journal of Medicinal Chemistry manuscripts involving natural-product semisynthesis, analogue optimization, structure–activity relationships, and pharmacology, with a required confirmation gate for study scope, group publications, and pharmacology data. |

Both skills follow an evidence-first rule: preserve the source record and never invent missing data.

### Repository structure

```text
codex-chemistry-writing-skills/
├── edit-si-experimental-procedures/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/
└── jmc-manuscript-workflow/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/
```

### Installation

#### Option 1: Skill Installer

Invoke `$skill-installer` in Codex and provide this repository URL together with the directory of the skill you want to install.

#### Option 2: Manual installation

1. Clone or download this repository.
2. Copy the desired skill folder into:

```text
$HOME/.agents/skills/
```

3. Restart Codex if the skill does not appear immediately.

### Usage examples

```text
$edit-si-experimental-procedures Convert these experimental records and analytical data into JMC Supporting Information format.
```

```text
$jmc-manuscript-workflow Revise this natural-product analogue manuscript using the supplied project files.
```

### Notes

- Always verify the original laboratory records, spectra, instrument reports, and final manuscript.
- The skills must not fill in experimental conditions, yields, purity values, or analytical data that are absent from the source material.
- Users remain responsible for scientific accuracy, data integrity, and journal compliance.

See the [OpenAI Build skills documentation](https://learn.chatgpt.com/docs/build-skills) for the current skill structure and usage model.
