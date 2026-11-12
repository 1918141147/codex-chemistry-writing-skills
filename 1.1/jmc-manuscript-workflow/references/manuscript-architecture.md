# JMC Manuscript Architecture and Argument Flow

Use this architecture as a decision guide, not a rigid template. Omit sections unsupported by the user's project.

## Default manuscript order

Use this order for a new manuscript when the author has supplied no other structure. For a revision, keep the accepted section order unless the author asks to reorganize it.

1. **Front matter.** Title, authors and affiliations, corresponding author and contribution notes where applicable, ABSTRACT, then KEYWORDS.
2. **INTRODUCTION.** Disease or biological need → assay or mechanistic rationale → chemical opportunity and approved group work → current study.
3. **RESULTS AND DISCUSSION.** Material supply and design → chemistry and Schemes → screening and SAR → lead selection and supported follow-up. Keep the chemistry and SAR linked by the design question. Add mechanistic and in vivo subsections only where supported.
4. **CONCLUSION.** Principal SAR, reason for advancing the lead, and the main findings supported by the data.
5. **EXPERIMENTAL SECTION.** Chemistry and Biological Evaluation. Within Chemistry, group general methods, preparation or isolation, synthetic procedures, and compound characterization. Within Biological Evaluation, order the assay methods and statistical analysis to follow the reported experiments.
6. **Back matter.** ASSOCIATED CONTENT and Supporting Information, AUTHOR INFORMATION, ACKNOWLEDGMENTS, ABBREVIATIONS USED when needed, and REFERENCES. Include author roles, funding, and competing interests where applicable. Add a table-of-contents graphic when the submission requires one.

Place figures, schemes, and tables near their first substantive discussion and synchronize callouts. Apply the [Word profile](format-and-qa.md#default-manuscript-profile) by element.

## Title

Prefer an outcome-led medicinal chemistry title:

`[Strategy] of [scaffold/class] Identifies [lead or activity outcome] for [biological context]`

Do not call a compound a probe, drug candidate, target-specific inhibitor, or disease-modifying agent without the corresponding evidence.

## Abstract

Build one continuous argument:

1. unmet biological or therapeutic need;
2. value and limitation of the starting scaffold(s);
3. semisynthetic or synthetic strategy and size/scope of the analogue set;
4. decisive SAR finding and lead selection;
5. mechanism and in vivo findings only if directly supported;
6. restrained significance statement.

Avoid a list of experiments. Include quantitative results when final values exist; retain visible placeholders rather than inventing them when the user is still assembling data.

## Introduction

A useful four-paragraph progression is:

1. **Disease and unmet need.** Define the disease context and limitations of current therapy.
2. **Biological rationale.** Explain the inflammatory pathway, assay, or mechanism that makes the activity relevant. Define each abbreviation at first use.
3. **Chemical opportunity.** Introduce small molecules/natural products, the exact compound class, prior isolation or structural history, and the user-confirmed group research program. The group-background paragraph may cite only the papers approved at intake.
4. **Current study.** State the starting materials, chemical regions modified, purpose of the SAR campaign, lead-selection objective, and the scope of mechanism or animal evaluation. Align this paragraph with Figure 1.

The Introduction should end with what the study does, not a detailed conclusion. If Figure 1 is a combined chemical/mechanistic overview, describe only elements actually shown in it.

## Results and Discussion

### 1. Material supply and medicinal chemistry design

Explain the source of the starting compounds, initial activity or limitation, why two or a few natural congeners are insufficient for SAR, and how the scaffold is divided into modifiable regions. End with the questions the chemistry will answer.

### 2. Semisynthetic modification

Organize by medicinal chemistry logic rather than chronological laboratory notes:

- exposed polar handles such as N-H or O-H;
- ring-state or conformational editing;
- oxidation-state or fused-ring remodeling;
- interconversion routes that connect related scaffold states.

Each paragraph should contain: design question → concise transformation and product set → why the set enables the next comparison. Do not repeat full workup or purification details here.

When a later oxidation campaign arose from the N-H-modified or ring-edited series, make that transition explicit. Do not present oxidation as an unrelated reaction list.

### 3. Biological screening and SAR

Define the assay and the readouts used for comparison. Organize the narrative around successive chemical questions. When N- and O-derivatization tested the same question about accessible polar groups, discuss them together. Connect their outcome to the subsequent choice to change ring state or the fused core when the project history supports that progression. Keep the contrast or exception that affects the next design decision.

- Group related modifications to cover the relevant analogue series without repeating the table row by row.
- Place the matched IDs and decisive readout next to each interpretive sentence when it helps the reader audit the claim, for example `(analogue vs parent, IC₅₀ 3.0 vs 8.0 μM)`.
- Follow key comparisons with a short structural interpretation or design implication. An explanation should identify the chemical feature or context that might matter and stay within the evidence. A second sentence repeating the ranking adds little.
- Explain why the selected molecule advanced, using the evidence for its activity and practical selection criteria. End with the lead and the purpose of its follow-up evaluation.

Use the [data and SAR rules](chemistry-pharmacology-rules.md#screening-data-and-potency) to choose comparable endpoints and calibrate the claim.

### 4. Lead validation and pharmacology

Use only modules supported by the user's data. A common JMC progression is:

1. concentration-response activity and cell viability;
2. unbiased transcriptomic/proteomic prioritization;
3. targeted pathway validation;
4. cytokine or functional output;
5. acute in vivo inflammation/cognition model;
6. disease-relevant model or pathology readout.

At the start of each subsection, connect the new experiment to the unresolved question from the previous subsection. At the end, state what the data establish and what they do not.

Use evidence-calibrated verbs:

- observation: `reduced`, `increased`, `was associated with`;
- pathway support: `attenuated signaling`, `supported involvement`;
- causal mechanism only with direct evidence: `mediated`, `required`, `directly targeted`.

Unchanged protein abundance does not prove absence of pathway involvement. A molecular docking result alone does not establish binding. A disease-model phenotype does not by itself establish disease modification.

## Conclusion

Reconstruct the entire argument in compressed form:

1. fermentation or synthesis enabled a focused analogue collection;
2. the principal SAR rules;
3. why the selected molecule is a lead;
4. the supported cellular/mechanistic/in vivo findings;
5. a restrained next step.

The Conclusion may echo Figure 1 more strongly than the Introduction, but it must not introduce new results.

## Experimental Section and Supporting Information

The Experimental Section records what was done; it does not carry the design argument. Use general procedures for repeated transformations and individual procedures for exceptions, products, characterization, and yields. Follow the actual operation order.

## Figures and Schemes

- Keep each Scheme, its caption, reaction-condition line, Results description, and Experimental procedure synchronized.
- If images are not ready, insert a clear placement marker and a final-form caption.
- Figure 1 may combine representative natural products, design strategy, lead generation, and a supported mechanism overview.
- Use a short Figure 1 caption—normally one or two sentences—without restating the complete mechanism.
- A SAR figure caption should identify the representative derivatives and the biological readout without interpreting the results.
- If a structure overview and screening table are combined, use panel-specific captions and in-text callouts. Follow the [editable layout checks](format-and-qa.md#screening-tables-and-composite-figures).
