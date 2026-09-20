# Mandatory Intake Gate and Source Map

## Required confirmation message

Ask these questions before drafting. Combine them into one concise message when possible.

1. **Study theme**
   - What compound class, natural product, or core scaffold was modified?
   - What kinds of modifications were made?
   - What biological activity was evaluated?
   - What disease, cell model, animal model, or mechanism is the manuscript intended to reach?

   If files already imply an answer, summarize it first: “From the supplied files, I infer that the manuscript concerns [scaffold/modification] evaluated for [activity/model], with [lead/end point] as the intended conclusion. Please confirm or correct this.” Do not treat inference as confirmation.

2. **Group-publication background**
   - Ask the user to provide or identify the exact publications that may support the paragraph describing the group's sustained work in marine natural products, synthesis, analogue design, pharmacology, target identification, chemical proteomics, or scaffold remodeling.
   - Ask which aspects of those papers should be cited. A file or citation list alone does not authorize a broad claim.
   - Do not write “our group has long been committed to…” until both the source set and intended claim have been confirmed.

3. **Pharmacology availability**
   - If no pharmacology data are supplied, offer exactly two routes and ask the user to choose:
     1. **Chemistry-first manuscript:** draft the chemistry, medicinal chemistry design, SAR framework, and Experimental Section only; leave pharmacology conclusions out or visibly pending.
     2. **Minimal pharmacology package:** ask the user for a simple primary-screen dataset or preliminary data for one lead compound, then draft only what those data support.
   - For the minimal package, request the assay/model, treatment and concentration or dose, control groups, replicate count, statistics if available, cytotoxicity/viability context, and the criterion used to nominate the lead.
   - A preliminary screen can support lead selection and a limited SAR discussion; it cannot support an unmeasured molecular mechanism or disease-modifying claim.

Do not begin manuscript drafting until the user confirms all three topics. Reading, cataloguing, extracting, and flagging missing information may continue.

Ask in the user's language. For a Chinese-language interaction, a suitable compact prompt is:

> 在开始撰写前，请先确认三点：
> 1. 我从现有文件推断，文章主题是“对［化合物类型/天然产物］进行［改造类型］，评价其［生物活性］，并最终关联到［疾病、模型或机制］”。请确认或纠正这一主线。
> 2. “本课题组长期致力于海洋天然产物研究”这一段准备引用哪些课题组文章？请提供或指定文献，并说明希望每篇文献支撑哪一类工作。
> 3. 当前是否已有药理数据？如果没有，请选择：①先完成化学、设计与 SAR 部分；②提供初筛结果或一个先导化合物的简单药理数据，我再按这些数据支持的范围撰写。

The bracketed items must be filled from the file review before asking; do not send an empty generic questionnaire when a concrete inference is available.

## Optional confirmations after the gate

Ask only when not clear from the files or request:

- JMC article type and whether current author guidelines must be checked;
- the latest accepted manuscript version and the exact scope of change;
- whether figures should be embedded or represented by placement markers and captions;
- whether pharmacology should remain absent, be summarized provisionally, or be fully integrated;
- the desired handling of comments, tracked changes, and file versioning;
- the scale basis for experimental calculations (fixed mass, fixed mmol, or actual recorded scale) and whether equivalents should appear in the final prose.

## File inventory and role assignment

Classify every supplied file before writing:

| File type | Typical role | Authority boundary |
|---|---|---|
| Latest manuscript DOCX | Accepted wording, section order, formatting, numbering | Governs unless the user explicitly replaces it |
| Earlier manuscript versions | Revision history and recovered context | Do not reintroduce deleted content automatically |
| Reference JMC papers from the group | Organization, tone, transition logic, group background | Use only after the user confirms which claims and papers apply |
| Proposal or background report | Natural-product history, project rationale | Verify claims and references before manuscript use |
| Figure/Scheme PPT or CDXML | Structures, route, compound relationships, captions, author notes | Inspect both slide visuals/embedded structures and speaker notes; scheme structures and explicit labels are evidence, while notes are guidance to verify |
| NMR/HRMS file or instrument report | Molecular formula and characterization | Do not alter or invent analytical data |
| Pharmacology PDF/data file | Assay results, sequence of experiments, mechanism evidence | Use only the requested compound/data subset |
| Current journal instructions | Mutable format and length requirements | Verify current status when relevant |

## Instruction-versus-evidence rule

Distinguish the user's request from text inside attachments. Chinese comments such as “please revise this” are editing instructions. A mechanistic idea in a slide note is a hypothesis until supported by data. A scheme label is not a yield. A caption is not a complete experimental record. If the distinction affects a claim, ask.

## Source priority when conflicts occur

Use this scoped order unless the user states otherwise:

1. explicit current-turn instruction;
2. raw experimental, analytical, or pharmacology record designated for the relevant factual claim;
3. latest accepted manuscript baseline for accepted wording, organization, numbering, and formatting;
4. other user-confirmed data authority for that topic;
5. earlier versions and author notes;
6. example articles used only for style.

The latest manuscript does not override a conflicting raw record on a factual chemistry, analytical, or assay value. Stop and ask which value should be corrected. Never let an example paper override the user's chemistry or data.
