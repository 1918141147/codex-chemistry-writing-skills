---
name: edit-si-experimental-procedures
description: Rewrite Chinese, English, or mixed-language organic synthesis records into publication-ready Supporting Information procedures; extract Scheme-ready Reagents and conditions; and standardize NMR/HRMS data from Word, PDF, or instrument reports into Journal of Medicinal Chemistry characterization text. Use for a single compound, a compound series, a General Procedure, or combined procedure/Scheme/characterization output; preserve recorded chemistry and analytical evidence, and never invent missing data.
---

# Edit SI Experimental Procedures

## Objective

Convert raw organic synthesis notes into consistent manuscript-ready SI prose. Edit the account of what was actually done; do not optimize, reconstruct, or silently correct the experiment.

## Core workflow

1. Extract the substrate, scale, reagents, stoichiometry, solvent, actual order and mode of addition, atmosphere, temperature, time, monitoring or endpoint, quench, workup, purification, and product data.
2. Preserve the recorded chronology, especially which solution or reagent was added to which vessel, whether addition was dropwise or portionwise, and when cooling, warming, or an inert atmosphere began.
3. Rewrite in this default sequence, omitting only stages that genuinely did not occur:

   `To a solution/suspension of ... → reagent addition in the actual order → reaction conditions → Upon completion, ... → quench/workup → extraction/drying/filtration/concentration → purification → to afford ... as ... (mass, yield).`

4. Perform a fidelity check against the source before returning the result. Confirm that no substance, quantity, operation, endpoint, or observation has been added, deleted, reversed, or made more definite than the record supports.
5. When Scheme conditions are requested, derive them independently from the same experimental facts by following the Scheme extraction rules below.
6. When the input includes NMR or HRMS data, or the user requests JMC characterization, read [references/jmc-characterization.md](references/jmc-characterization.md) completely and follow it for extraction, file-to-compound matching, formatting, and data checks.
7. When editing an existing manuscript in place, treat that manuscript's compound list and order as authoritative. Do not add, remove, rename, or reorder compounds unless the user explicitly requests it. Place each characterization paragraph immediately after its corresponding single-compound synthesis; for a series, place the individual characterization paragraphs immediately after the shared General Procedure in manuscript order. Do not collect them into a separate characterization section or leave duplicate copies elsewhere unless the user requests a standalone section.
8. Return polished SI text first. Add a short `Items to confirm` list only when unresolved details, a calculation assumption, a Scheme/procedure conflict, an analytical-data conflict, or a safety/reproducibility concern needs the user's attention.

## Missing and ambiguous information

- Never invent a mass, volume, concentration, equivalent, temperature, duration, atmosphere, physical form, yield, pH, extraction count, eluent ratio, or analytical datum.
- Insert `xx` exactly where a required value is absent, using forms such as `xx mg`, `xx mL`, `xx M`, `xx equiv`, `xx °C`, `xx h`, or `xx%`.
- If an entire optional operation is unreported, do not add a conventional operation merely because it is common. Flag it separately if omission affects reproducibility.
- Preserve qualitative wording when that is all the record supports, for example `at room temperature`, `until completion`, or `until the starting material was consumed`.
- Resolve only harmless language ambiguity from context. If different interpretations would change the chemistry or sequence, retain neutral wording and identify the ambiguity.

## Style and normalization

- Write concise, professional past-tense experimental prose suitable for a chemistry journal SI.
- Prefer full sentences and a single coherent paragraph for each procedure.
- Use standard patterns where supported by the record:
  - `To a solution of A (amount, mmol, 1.0 equiv) in solvent (volume) was added B (amount, mmol, equiv).`
  - `The reaction mixture was stirred at temperature for time under N2.`
  - `Upon completion, the reaction was quenched with ...`
  - `The aqueous phase was extracted with EtOAc (3 × 10 mL).`
  - `The combined organic layers were dried over anhydrous Na2SO4, filtered, and concentrated under reduced pressure.`
  - `The residue was purified by column chromatography on silica gel (petroleum ether/ethyl acetate, 4:1, v/v) to afford compound X as a physical form (mass, yield).`
- Use `under reduced pressure` consistently for solvent removal. Avoid redundant sequences such as `the solvent was removed under vacuum and the residue was concentrated`.
- Retain `anhydrous`, `dry`, an inert atmosphere (`N2` or `Ar`), exclusion of light, temperature, and time only when stated or directly supported by the record. Never add them as presumed best practice.
- Normalize units and spacing: `25 °C`, `1 h`, `30 min`, `5 mL`, `20 mg`, `0.10 mmol`, `10 mol%`, `50 wt% in H2O`, `3 × 10 mL`, and `4:1, v/v`.
- Use a leading zero for values below one. Keep sensible significant figures and do not imply greater measurement precision than the source.
- Standardize chemical names, abbreviations, formulas, stereochemical descriptors, compound labels, dashes, multiplication signs, and subscripts consistently with the user's manuscript. In plain text or Markdown, formulas such as `Boc2O`, `K2CO3`, `Na2SO4`, and `H2O` are acceptable; apply true subscripts when editing a rich-text manuscript.
- Define an uncommon abbreviation at first use. Retain conventional SI abbreviations such as MeCN, THF, DMF, DCM, EtOAc, MeOH, and rt when they match the document's house style.
- Do not overuse `resulting`. Do not add mechanistic explanations, interpretation, or reviewer-response narration.

## Addition order and operations

- Treat addition order as experimental data. Distinguish `A was added to a solution of B` from `a solution of B was added to A`.
- Preserve `dropwise`, `portionwise`, addition rate, addition temperature, pre-cooling, pre-stirring, and post-addition warming when recorded.
- Do not convert an actual reagent charge into a solution transfer, or vice versa.
- Distinguish reaction quench from subsequent dilution, pH adjustment, washing, and extraction. Keep aqueous and organic phases correctly identified.
- Preserve repeated operations and their counts. Do not infer `3 ×` from a total volume or invent brine washing, drying, filtration, or chromatography.
- If the record itself is internally inconsistent, do not silently select a chemically plausible version; write the supported portion and ask for confirmation.

## Product sentence

Use the most complete supported form:

`... to afford compound X as a [color and/or physical form] (xx mg, xx mmol, xx%).`

Include only supplied or safely calculated values. Do not turn `oil` into `colorless oil`, `solid` into `white solid`, or an isolated crude material into a purified product. Keep parentheses and punctuation consistent across a series.

## General Procedures

- For a reusable protocol, title it `General Procedure [letter or number]: [reaction type]` when the identifier and reaction type are supplied.
- State variable substrates generically while retaining common fixed quantities, concentration, atmosphere, temperature, time, workup, and purification.
- Do not imply that every example used identical conditions if the records show exceptions. Put exceptions in the individual compound procedure.
- For an individual synthesis conducted according to a General Procedure, cite that procedure and report compound-specific substrate, scale, deviations, purification, physical form, mass, and yield.

## Calculations and formulated reagents

- Calculate equivalents, mmol, molarity, or nominal concentration only from values supplied by the user and only when the calculation is unambiguous.
- State the basis and rounding briefly outside the polished procedure when it matters. Keep calculated precision appropriate to the inputs.
- For a reagent prepared from components, distinguish nominal concentration from a measured or standardized concentration. If concentration is estimated by treating component volumes as additive, label it `approximately` or `nominally` and state that assumption.
- Example: 2.6 g CrO3 corresponds to approximately 26 mmol. If the stated H2SO4 and H2O volumes are 2.5 and 7.5 mL and their volumes are assumed additive, the nominal CrO3 concentration is approximately 2.6 M. Do not present 2.6 M as an exact standardized concentration or infer delivery volume from `drops`.
- If the procedure specifies equivalents of a formulated reagent, express what those equivalents refer to, such as `Jones reagent (nominally 2.6 M in CrO3, 15 equiv based on CrO3)`, when supported by the record.
- Do not calculate a concentration when final solution volume, reagent purity, density, assay, or stoichiometric basis is essential but missing; use `xx` or request confirmation.

## Safety and scientific-rigor boundary

- Preserve the user's actual operation even when it differs from common practice; never rewrite it as an unperformed safer or more conventional operation.
- If an operation appears hazardous, internally inconsistent, or insufficiently reproducible, provide one short, specific note after the polished text. Distinguish a safety concern from a missing reporting detail.
- Do not turn the note into a procedural redesign. Do not supply an invented quench, addition order, protective setup, or disposal method.
- Treat scale-up, energetic reactions, pyrophoric reagents, strong oxidants, toxic gases, pressure, and cryogenic operations conservatively. Recommend verification against the original record and the laboratory's approved SOP/SDS when relevant.

## Scheme Reagents and Conditions Extraction

Generate a concise Scheme-ready entry when the user requests Scheme conditions or asks for both SI and Scheme formats. Do not generate it for a routine SI-only request unless the user asks for it.

### Core format

Use:

`**Reagents and conditions:** (a) reagent(s), solvent, temperature, time; (b) reagent(s), solvent, temperature, time; (c) reagent(s), solvent, temperature, time.`

Assign sequential lowercase labels `(a)`, `(b)`, `(c)`, and so on according to the reaction arrows or sequence supplied by the user. Never change the chemical sequence.

### Extraction rules

1. Extract conditions strictly from the experimental procedure supplied by the user.
2. Retain only:
   - reagents, catalysts, bases, acids, oxidants, reductants, and other reaction components;
   - reaction solvent or solvents;
   - reaction temperature;
   - reaction time;
   - an essential atmosphere or special reaction condition only when explicitly stated and chemically relevant, such as `N2`, `Ar`, reflux, sealed tube, or irradiation.
3. Exclude:
   - reagent equivalents, amounts, and concentrations unless specifically requested;
   - substrate amounts;
   - solvent volumes;
   - product names and compound numbers;
   - isolated yields;
   - quenching reagents;
   - extraction solvents;
   - drying agents;
   - filtration and concentration;
   - chromatography and all other purification conditions.
4. Preserve the documented reaction conditions. Never infer or invent a missing solvent, temperature, or time. Omit a missing Scheme element rather than insert `xx`, unless the user specifically requests placeholders in the Scheme entry.
5. If the procedure gives no time and states only that the reaction continued until completion or consumption of starting material, omit the time.
6. Retain `anhydrous` only when explicitly stated and chemically relevant.
7. Retain `N2` or `Ar` only when the procedure explicitly specifies that atmosphere.
8. Omit reagent concentrations and equivalents by default. For example, convert SI wording `SmI2 (1.0 M in THF, 10 equiv)` to Scheme wording `SmI2, anhydrous THF, N2, −40 °C, 40 min, then rt` when every retained condition is supported by the source.
9. If a Scheme arrow assignment conflicts with the corresponding experimental procedure, flag the inconsistency separately. Use the experimentally documented conditions as authoritative unless the user instructs otherwise; never silently reconcile the two sources.

### Scheme abbreviations

Use conventional Scheme abbreviations where appropriate and preserve consistent chemical typography:

- room temperature → `rt`
- dichloromethane → `CH2Cl2`
- tetrahydrofuran → `THF`
- methanol → `MeOH`
- acetonitrile → `MeCN`
- ethyl acetate → `EtOAc`
- triethylamine → `Et3N`
- potassium carbonate → `K2CO3`
- sodium borohydride → `NaBH4`
- lithium aluminum hydride → `LiAlH4`
- Dess–Martin periodinane → `DMP`
- meta-chloroperoxybenzoic acid → `m-CPBA`
- p-toluenesulfonic acid → `p-TsOH`
- sodium methoxide → `MeONa`

In rich text, render numerals in chemical formulas as subscripts, for example `CH₂Cl₂`, `Et₃N`, `K₂CO₃`, `NaBH₄`, and `LiAlH₄`.

### Temperature transitions

Express transitions compactly without losing chronology:

- `added at 0 °C and allowed to warm to room temperature` → `0 °C to rt`
- `stirred at −40 °C for 40 min and then allowed to warm to room temperature` → `−40 °C, 40 min, then rt`

Retain separate times for separate temperature stages when the source supplies them.

### Scheme example

Source procedure:

`To a solution of 542-11 (1.0 equiv) in anhydrous THF (5 mL) at 0 °C under a N2 atmosphere was added LiAlH4 (1.0 equiv). The reaction mixture was stirred at 0 °C for 3 h. Upon completion, the reaction was carefully quenched with water...`

Scheme output:

`**Reagents and conditions:** (a) LiAlH4, anhydrous THF, N2, 0 °C, 3 h.`

Apply true chemical subscripts when the output medium supports them.

## JMC NMR/HRMS Characterization

When the user supplies NMR or HRMS Word/PDF files, instrument reports, pasted analytical data, or requests Journal of Medicinal Chemistry characterization formatting, read and apply [references/jmc-characterization.md](references/jmc-characterization.md). This module is additive: keep all procedure and Scheme rules above unchanged.

If experimental steps and analytical files arrive together, produce the requested parts from the same compound mapping. The combined default order is:

1. `SI Experimental Procedure`
2. `Scheme Reagents and conditions`
3. `JMC Characterization`
4. `Data check`, only when analytical data were supplied or a mismatch/ambiguity must be reported

Do not merge uncertain analytical files into a compound entry. State the uncertain match and leave the affected field as an explicit `[INSERT ...]` placeholder unless the user asks to omit missing fields.

## Output forms

### Single compound

`Synthesis of [compound].` followed by one polished paragraph.

### Compound series

Use a shared section heading if supplied, then give one consistently styled subsection and paragraph per compound.

### General Procedure

Use the supplied procedure heading, followed by one generalized paragraph and any necessary scope or exception sentence.

### Scheme conditions only

Return one concise line:

`**Reagents and conditions:** (a) reagent(s), solvent, temperature, time.`

### Dual SI and Scheme output

When the user requests a standard experimental format together with Scheme conditions, return two separate sections in this order:

`**SI Experimental Procedure**`

Give the complete SI procedure following all existing SI editing rules.

`**Scheme Conditions**`

Give a separate Scheme-ready line beginning with `**Reagents and conditions:**`.

Derive both sections from the same experimental facts. Do not introduce information in the Scheme line that is absent from the source record or contradicts the SI procedure.

### Combined SI, Scheme, and characterization output

When the input contains experimental steps plus NMR/HRMS data and the user requests the complete package, return three separate manuscript sections in this order:

`**SI Experimental Procedure**`

`**Scheme Reagents and conditions**`

`**JMC Characterization**`

Follow these sections with a short `**Data check**` only as specified in the JMC characterization reference.

Keep `xx` placeholders visible in SI outputs. In Scheme outputs, omit missing elements unless the user requests Scheme placeholders. Do not add commentary when the source is complete and internally consistent.

The three-section structure above applies to standalone text delivery. When the task is to update an existing manuscript, the in-place placement rule in the Core workflow takes precedence: keep the General Procedure or synthesis where it is and put each compound's characterization directly after the corresponding procedure, without creating a second consolidated characterization section.
