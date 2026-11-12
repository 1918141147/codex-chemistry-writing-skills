# Codex Chemistry Writing Skills 1.1

[中文](#中文) · [English](#english)

## 中文

`1.1` 是 `codex-chemistry-writing-skills` 的第一个独立版本目录。仓库根目录中的原始发布版保持不变；后续更新继续使用 `1.2`、`1.3` 等新目录，以便回溯每次发布。

### 本版内容

本目录包含两个可单独安装的 Skill：

- `jmc-manuscript-workflow`：JMC 天然产物半合成、类似物优化、SAR、药理叙事和 Word 主文修改流程。本版沿用原始发布版内容。
- `edit-si-experimental-procedures`：JMC Supporting Information 的实验步骤、Scheme 条件、NMR/HRMS、谱图、晶体学和 Word 编排流程。本版新增 HPLC 纯度报告装配规则。

### 1.1 新增的 HPLC 纯度报告流程

SI Skill 现在能够在作者最新 SI 的 `HPLC Purity` 部分中完成以下工作：

1. 建立“正式 SI 编号—实验室样品号—原始纯度报告”的交叉映射，并以作者确认的最新 SI 编号为准。
2. 将色谱图、Peak List 表格和图注作为不可拆分的一组处理，避免重排时发生图表错配。
3. 按正式 SI 编号自然排序，而不是按原始文件名或实验室编号排序。
4. 默认将 Peak List 统一为五列：`No`、`Name`、`Retention time (min)`、`Peak area (mAU*s)` 和 `Area percent (%)`。
5. 保留原始峰表数值、精度、峰顺序、总计行和色谱图；不计算、补填或改写纯度数据。
6. 允许仪器图保留原始样品号用于追溯，正式图注使用当前 SI 编号并加粗化合物编号。
7. 默认每页排两个可读报告；报告总数为奇数时，最后一页可以只放一个。
8. 不依靠手动分页符控制成对排版，而使用自然分页、不可拆分容器和适当的报告最小高度。
9. 对缺失或无法确认的报告保留缺口并提示作者，不生成虚构色谱图、纯度值或占位数据。
10. 完成后核对映射、顺序、记录数量、表格列、图注、图表配对、分页和 `References` 边界，并确认 HPLC 之外的内容未被修改。

### 安装

从仓库根目录安装 1.1 版时，使用以下子目录：

```text
1.1/jmc-manuscript-workflow
1.1/edit-si-experimental-procedures
```

可以复制一个或两个目录到全局 Skill 目录：

```text
$HOME/.agents/skills/
```

也可以放入具体项目的 `.agents/skills/` 目录，仅供该项目使用。

### 版本边界

- 原始发布版仍保留在仓库根目录，不在 1.1 发布中覆盖。
- 1.1 仅扩展 SI Skill 的 HPLC 纯度报告能力；主文 Skill 和 SI Skill 的其他规则保持不变。
- 示例或历史报告只能用于版式和映射验证，不能作为新的实验事实来源。

## English

`1.1` is the first self-contained version directory of `codex-chemistry-writing-skills`. The original release remains unchanged at the repository root. Future releases should use separate directories such as `1.2` and `1.3` so that every published version remains recoverable.

### Included skills

- `jmc-manuscript-workflow`: JMC manuscript drafting and revision for natural-product semisynthesis, analogue optimization, SAR, pharmacology, and Word QA. Version 1.1 carries forward the original release unchanged.
- `edit-si-experimental-procedures`: JMC Supporting Information procedures, Scheme conditions, NMR/HRMS, analytical figures, crystallography, and Word assembly. Version 1.1 adds an HPLC purity-report workflow.

### HPLC purity workflow added in 1.1

The SI skill now instructs Codex to:

1. Build and verify a crosswalk between current SI identifiers, laboratory sample identifiers, and source purity reports.
2. Keep each chromatogram, Peak List table, and caption together as one atomic record during extraction and reordering.
3. Sort reports by current SI numbering rather than raw filenames or laboratory identifiers.
4. Standardize displayed Peak List tables to `No`, `Name`, `Retention time (min)`, `Peak area (mAU*s)`, and `Area percent (%)` unless the author requires another template.
5. Preserve all source values, precision, peak order, totals, and chromatograms without recalculation or silent correction.
6. Retain instrument sample labels inside source plots for traceability while using the current SI identifier in the formal caption.
7. Aim for two readable reports per page and allow one final report when the total is odd.
8. Avoid manual page breaks for pairing; use natural pagination and non-splitting report containers.
9. Leave unsupported or ambiguous reports unresolved rather than inventing chromatograms, purity values, or placeholder data.
10. Verify record mapping, order, counts, table columns, captions, image/table pairing, pagination, the `References` boundary, and preservation of content outside the HPLC section.

### Installation

Install either or both version 1.1 skill directories:

```text
1.1/jmc-manuscript-workflow
1.1/edit-si-experimental-procedures
```

Copy them to `$HOME/.agents/skills/` for global use or to a project's `.agents/skills/` directory for project-only use.

### Version scope

- The original release remains at the repository root and is not overwritten.
- Version 1.1 changes only the HPLC purity-report capability of the SI skill; the manuscript skill and all other SI rules remain unchanged.
- Historical reports and examples guide layout and identifier reconciliation only; they do not establish new experimental facts.
