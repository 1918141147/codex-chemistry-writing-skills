# Chemistry, Pharmacology, and Experimental Data Rules

## Chemistry narrative

- Use compound structures, numbering, and reaction relationships from the user-designated scheme source.
- Use the detailed experimental method as the authority for reagents, solvent, temperature, time, atmosphere, order of addition, workup, purification, and yield.
- If an overview paragraph conflicts with the detailed method, correct the overview or ask; never change the method to fit a caption silently.
- Keep medicinal chemistry Results concise. Explain the design and outcome, not every operational step.
- Distinguish isolated and characterized products from crude or telescoped intermediates. If an intermediate is carried directly to the next step and no spectrum will be reported, say so and do not fabricate characterization.
- Use `lead compound` for a prioritized active analogue. Use `chemical probe` only when the project establishes probe-quality potency/selectivity and actually uses it to interrogate biology.

## Connecting chemistry rounds

When multiple chemistry rounds exist, preserve causal progression:

1. starting natural products or core scaffold;
2. first-round modification of accessible N-H/O-H or analogous handles;
3. activity or structural lessons from that round;
4. ring-state/oxidation/remodeling strategy motivated by those lessons;
5. lead selection and downstream pharmacology.

Do not describe a second-round oxidation series as if it were planned independently when it arose from the first-round compounds.

## Quantities and molecular-weight calculations

Before calculating, confirm whether the procedure should use the actual recorded scale, a fixed mass, or a fixed mmol scale.

- Treat molecular formulas in the user-designated NMR/HRMS record as authoritative.
- Use average molar mass for preparative weighing unless the user explicitly requests exact/monoisotopic mass.
- Substrate mass: `mass (mg) = amount (mmol) × molar mass (g mol−1)`.
- Reagent amount: derive mmol from the confirmed stoichiometry, then calculate mass from its molar mass.
- Solution volume: calculate only when concentration is supplied and unambiguous.
- Product mass from a reported yield: `product mass (mg) = limiting-reagent mmol × fractional yield × product molar mass`.
- Apply sensible significant figures; normally report preparative masses to 0.1 mg and small-molecule amounts to 0.001 or 0.0001 mmol as appropriate.
- If equivalents were provided only to enable calculation and the user requests their removal, remove them from final prose after the masses/mmol have been checked.
- Do not infer density, assay, solution strength, hydrate state, or intermediate yield. For a formulated reagent such as Jones reagent, state the basis of concentration and equivalents/mmol when known.
- For an unisolated telescoped intermediate, do not invent an isolated mass. Carry forward the confirmed theoretical or measured mmol basis only when the user authorizes that basis.

## Experimental procedure style

Use this order when the record supports it:

`substrate and solvent → reagent addition in actual order → temperature/time/atmosphere → completion or endpoint → quench/workup → extraction/drying/concentration → purification → product (mass, yield)`

Use units and spacing consistently: `27.2 mg, 0.050 mmol`, `5 mL`, `0 °C`, `1 h`, `3 × 10 mL`, `4:1, v/v`.

Never add a color, physical form, workup operation, yield, or analytical datum not present in the source.

## Screening data and potency

- For each revised entry, verify compound identity, endpoint, concentration, assay batch, comparator, and the source of the mean and uncertainty. Keep author-approved values, units, and precision. If only a mean is revised, verify that its error term belongs to the same replicates.
- Resolve a raw label that differs from the manuscript identifier against the structure, scheme, or author confirmation. Record the alias for traceability and use the confirmed manuscript identifier throughout the requested revision.
- For authorized recalculation from Prism, use the raw replicates and recorded exclusion flags. Verify concentration and plate, and use the agreed denominator. For inhibition relative to the model mean, use `100 × (1 − treated mean / same-plate model mean)`. Apply a control correction only if the chosen protocol calls for it. If reporting SEM with a fixed model denominator, calculate it across the included treated replicates and record their count. Retain negative or above-100% results when supported by that normalization.
- Report only the requested concentrations and distinguish initial screens, later screens, and dose–response assays. Resolve conflicting concentration labels before pooling or directly comparing batches.
- Keep an unreported IC₅₀ distinct from an experimentally established bound. If the author explicitly requests a common display placeholder such as `>20` for missing values, retain that distinction in the working data, explain the convention in a general note, and exclude placeholder-only entries from potency claims.

## SAR rigor

- Compare matched compounds using comparable, experimentally reported IC₅₀ values or bounds where they distinguish the pair. Otherwise use the approved same-concentration inhibition data. Discuss any divergence only when it matters to the conclusion.
- A single-concentration difference supports a screening trend or lead prioritization. A between-compound claim of statistical significance requires a corresponding test. Distinguish potency, inhibition, efficacy, selectivity, and viability.
- Ground a structural explanation in the verified structures. Phrase contributions of a newly introduced group, such as an enone, as hypotheses when other structural changes could explain the trend. A decrease after N-methylation supports a role for the imide N–H in that matched series. Stronger assignments such as a specific hydrogen bond require independent evidence.
- Justify lead selection with the supported trade-offs. Yield and starting-material supply can favor one analogue when potency does not. Use measured viability when available, and avoid attributing toxicity to an untested comparator.

## Pharmacology data gate

Do not write pharmacology sections from a proposed pathway diagram alone. Require at least the relevant raw summary, report, or user-confirmed values.

For each pharmacology claim, record:

- model and biological material;
- treatment, concentration/dose, duration, and comparator;
- endpoint and measurement method;
- replicate and statistical information when available;
- exact compound identity;
- result direction and numerical value;
- whether the result is screening, confirmatory, mechanistic, or in vivo.

If only preliminary screening is available, write a limited screening/SAR subsection and identify a provisional lead. Do not create transcriptomic, pathway, cytokine, cognition, or disease-model results.

When integrating a collaborator's accepted report, follow its supported experiment sequence and endpoints. Ask for extra raw data only if the requested claim needs it. Leave unsupported outcomes out of the text, figures, abstract, and conclusion.

## Mechanism language

Build a claim-evidence ladder:

| Evidence | Permitted conclusion |
|---|---|
| Phenotypic assay only | anti-inflammatory or anti-neuroinflammatory activity in that model |
| Expression/phosphorylation change | association with or attenuation of a pathway |
| Orthogonal pathway assay | stronger support for pathway modulation |
| Genetic/pharmacological rescue | evidence of functional dependence |
| Direct binding/target engagement | direct target claim within assay limitations |

Do not skip levels in this ladder.

Name the measured endpoint in the text and diagram. For example, a decrease in p-p65/total p65 supports a claim about the phosphorylation ratio. Claims of decreased total p65 or altered nuclear localization require the corresponding measurements.
