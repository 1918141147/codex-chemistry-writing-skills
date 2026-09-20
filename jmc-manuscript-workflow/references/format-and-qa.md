# Final-Format Rules and Quality Assurance

## Word and JMC style conventions

Use the user's latest accepted DOCX as the visual authority unless it conflicts with the current JMC submission template or explicit author instructions. A published, typeset JMC paper guides prose and editorial logic, not submission page geometry. In the absence of a manuscript baseline, apply a restrained ACS/JMC manuscript format and verify current author instructions when needed.

- Use consistent English scientific voice and tense throughout.
- The first body paragraph immediately below a section or subsection heading has no first-line indent. Subsequent body paragraphs use the manuscript's established first-line indent (the prior accepted format used approximately 0.33 in/0.85 cm).
- Keep section and subsection headings bold and unindented according to the baseline.
- Format compound numbers in bold wherever they function as compound identifiers, including body text, captions, schemes, and experimental procedures.
- Keep punctuation and parentheses around compound numbers unbolded unless the whole heading/caption is intentionally bold.
- Italicize chemical locants and prefixes where appropriate, such as *N*-, *O*-, *S*-, *p*-, and *m*-; preserve stereochemical italics and superscripts when required.
- Use true subscripts in chemical formulas and true superscripts for citation callouts or stereochemical notation where the document style requires them.
- At first occurrence, write `full name (abbreviation)`; use the abbreviation thereafter. Do not redefine common abbreviations repeatedly.
- At first occurrence, give the full natural-product name and its manuscript code; use the confirmed codes thereafter when the user prefers that convention.
- Keep figure and scheme numbering, in-text references, captions, and placement synchronized.
- Format references in JMC/ACS style with a consistent hanging indent. Preserve reference numbering unless references are deliberately added, removed, or reordered.

## Citation integrity

- Verify bibliographic facts, DOI, journal, year, volume, issue, pages/article number, and final publication status when current accuracy matters.
- Prefer primary literature for chemical history, biological mechanisms, and group achievements.
- Cite the exact paper that supports the exact sentence. Do not attach an entire cluster of group publications to a vague prestige claim.
- If a paper was formerly early-view, accepted, or in press, check whether final bibliographic details now exist before submission.
- Do not cite an example manuscript merely because its prose structure was imitated.

## Editing discipline

- Identify the current accepted source file before editing.
- Preserve all content outside the requested scope, including images, relationships, captions, comments, and reference numbering.
- Use short, sequential version names such as `v5`, `v5a`, or `v6`; do not overwrite the accepted baseline.
- When the user says “other content unchanged,” verify that only the intended paragraphs or XML parts changed.
- Re-read Chinese comments and annotations after editing to ensure none were accidentally retained as manuscript prose.

## Cross-component synchronization

Whenever chemistry changes, check all of the following:

1. Scheme structure and compound numbers;
2. Scheme reaction-condition line;
3. Results and Discussion description;
4. Experimental procedure;
5. product formula and NMR/HRMS label;
6. SAR text and figure labels;
7. abstract, Figure 1, and conclusion if the lead or route changed.

Whenever pharmacology changes, check:

1. assay name and model;
2. compound, dose/concentration, control, and statistics;
3. figure caption and panel references;
4. Results claim strength;
5. abstract, Figure 1 mechanism, and conclusion;
6. Experimental methods and abbreviations.

## Lessons encoded from the prior manuscript process

- **Theme drift:** disease background, anti-inflammatory screening, AD models, and mechanism can become disconnected if the study theme is not confirmed first. The intake gate prevents this.
- **Unsupported group narrative:** “our group has long pursued…” must be grounded in user-approved papers and claims.
- **Premature pharmacology:** a pathway sketch or planned experiment is not a result. Use chemistry-only mode or request the minimal data package.
- **Probe/lead confusion:** do not call an optimized active compound a probe without probe-level evidence and use.
- **Over-detailed synthesis in Results:** retain design logic and product sets in Results; move quantities and operations to Experimental/SI.
- **Scheme-method mismatch:** the detailed method governs reagents and conditions; update captions and overview text together.
- **Telescoped intermediate overclaim:** an intermediate used directly without spectra must remain an intermediate, not a fully characterized isolated product.
- **Scale ambiguity:** confirm fixed mass versus fixed mmol before calculating. Calculate product mass from formula, limiting amount, and stated yield.
- **Formatting drift:** compound bolding, italics, chemical subscripts, first-use abbreviations, paragraph indents, and reference hanging indents need a final global pass.
- **Scope creep:** do not reintroduce pharmacology or text the user deleted, and do not change unrelated sections while addressing a local revision.

## Final QA checklist

### Scientific and narrative

- [ ] The confirmed study theme is consistent from title through conclusion.
- [ ] Every mechanistic or pharmacological claim has a traceable source.
- [ ] Lead selection follows from reported data and does not use `probe` incorrectly.
- [ ] Each subsection opens with rationale and closes with the result's consequence.
- [ ] No unsupported numerical value or causal statement remains.

### Chemistry

- [ ] Compound numbers, structures, formulas, routes, and product labels agree across all files.
- [ ] Detailed procedures preserve actual addition order and conditions.
- [ ] Masses, mmol, yields, and solution volumes recalculate correctly from the confirmed scale.
- [ ] Unisolated intermediates are not assigned invented masses or spectra.

### Formatting

- [ ] First paragraphs below headings are unindented; later paragraphs follow the baseline indent.
- [ ] Compound identifiers are bold; chemical italics, subscripts, and superscripts are correct.
- [ ] Abbreviations are defined once and used consistently.
- [ ] Figure/Scheme captions and callouts match the current artwork.
- [ ] References use consistent JMC formatting and hanging indents.

### Document integrity

- [ ] Only requested content changed.
- [ ] Embedded media and relationships remain intact.
- [ ] The output opens without repair warnings.
- [ ] The final DOCX was rendered and visually inspected when tooling allowed; otherwise the limitation is disclosed.
