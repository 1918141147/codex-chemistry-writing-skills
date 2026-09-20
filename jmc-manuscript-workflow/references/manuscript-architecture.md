# JMC Manuscript Architecture and Argument Flow

Use this architecture as a decision guide, not a rigid template. Omit sections unsupported by the user's project.

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

Open the subsection with one or two sentences that define the assay, the starting compounds' activity, and why the analogue set was compared under common conditions. Then analyze matched structural changes in a stable order.

For each SAR paragraph:

1. identify the structural variable;
2. compare relevant compounds or matched pairs;
3. state the observed trend;
4. give a cautious structural interpretation;
5. end with the consequence for the next design decision.

Avoid overinterpreting single-concentration data. Explicitly note when solubility, permeability, cytotoxicity, or assay interference has not been excluded. The final SAR paragraph should justify lead selection using activity, safety window, synthetic accessibility, and data quality as available.

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
