# JMC NMR/HRMS Characterization

Use this module only when NMR or HRMS characterization is supplied or requested. It standardizes supported analytical data without changing the experimental-procedure or Scheme-extraction rules in the parent skill.

## Evidence-first extraction

1. Inspect every supplied Word file, PDF, instrument report, image, or pasted block that may contain analytical data. Use format-appropriate extraction tools, and visually inspect a rendered page when OCR, superscripts, minus signs, decimal points, or table alignment are ambiguous.
2. Build an internal record for each compound with the source filename/page and only the fields actually supported:
   - compound number or name;
   - physical form, isolated mass, yield, and purity;
   - for each NMR spectrum: nucleus, frequency, solvent, chemical shifts, multiplicities, coupling constants, integrations, and any explicitly reported qualifiers;
   - for HRMS: ionization method, acquisition polarity, stated ion/adduct type, formula associated with the calculated ion, calculated m/z, measured/found m/z, and reported ppm error.
3. Preserve the source precision. Do not add decimal places, round away a meaningful discrepancy, or silently normalize a value that may be a transcription error.
4. Never infer missing NMR peaks, physical form, mass, yield, purity measurement, ion type, formula, or m/z value from chemical plausibility.

## Matching multiple files to compounds

Match records in this priority order:

1. an unambiguous compound number or name inside the document;
2. an unambiguous compound number in the filename that agrees with the document;
3. a unique, corroborating combination of identifiers explicitly supplied by the user.

Do not guess from file order, similar molecular weights, a nearby Scheme position, or the order of compounds in the prompt. If filename and document identifiers conflict, or more than one compound is plausible, report the conflict under `Data check`, keep the file unmatched, and leave the affected characterization field as `[INSERT ...]` unless the user asks to omit it.

When many files are supplied, reconcile them before writing. A concise internal mapping such as `compound → NMR source(s) → HRMS source` is sufficient; show it to the user only when it helps explain ambiguity.

## JMC characterization form

Use one continuous characterization paragraph per compound. The standard form is:

`Compound XX. [physical form]; yield [INSERT YIELD]%; purity, >95%; ¹H NMR ([frequency] MHz, [solvent]) δ [signals]; ¹³C NMR ([frequency] MHz, [solvent]) δ [signals]; HRMS (ESI): m/z [ion] calcd for [ion formula] [calculated m/z]; found [measured m/z].`

Apply the following rules:

- Replace `Compound XX` with the supplied compound name/number and retain the manuscript's established naming convention.
- Include physical form, isolated mass, and yield only when supplied or unambiguously calculated from supplied values. Otherwise use `[INSERT PHYSICAL FORM]`, `[INSERT MASS]`, or `[INSERT YIELD]`, or omit the field if the user asks for omission.
- `purity, >95%` may be used as a project-wide house-style default only when the user explicitly supplies it. Treat it as user-supplied information, not as a value extracted from an analytical report. If the source contradicts it or it is unclear that the default applies to a particular compound, use `[INSERT PURITY]` and flag the issue rather than asserting `>95%`.
- Use `[INSERT ¹H NMR DATA]`, `[INSERT ¹³C NMR DATA]`, or `[INSERT HRMS DATA]` for absent required blocks. If the user requests source-only output, omit unsupported blocks instead.
- If a source contains HRMS only, fill only HRMS reliably; leave the other requested fields as placeholders or omit them according to the user's instruction.
- Do not use the parent skill's `xx` convention for missing characterization fields; use the explicit `[INSERT ...]` placeholders in this module.

### Placement in an existing manuscript

When analytical data are being inserted into an existing manuscript rather than returned as a standalone block:

1. Treat the compounds already present in the manuscript as the authoritative scope. Do not add a compound merely because it appears in an NMR or mass-spectrometry source, and do not remove a manuscript compound because its analytical data are incomplete.
2. Preserve the manuscript's compound order and established compound labels.
3. For a single-compound synthesis, insert its one continuous characterization paragraph immediately after the synthesis paragraph.
4. For a General Procedure or compound series, keep the shared procedure first and follow it immediately with one separate, consistently formatted characterization paragraph per manuscript compound, in the same order as the series. Do not append all analytical data to the General Procedure paragraph.
5. Do not create a distant consolidated characterization section when the user asks for data beside the corresponding compounds. If characterization already exists elsewhere, move it to the correct location rather than duplicating it.
6. Before the first NMR block, use this fixed field sequence: `[physical form]; yield ...%; purity, ...%; ¹H NMR ...; ¹³C NMR ...; HRMS ...`. Use `[INSERT PHYSICAL FORM]` and `yield [INSERT YIELD]%` when those facts are not supported. Use `purity, >95%` only when supplied by the user or otherwise supported under the purity rule above.

### General Procedure plus a compound series

Write the common synthesis first under the supplied heading, for example:

`General Procedure B: N-Alkylation of 54-1.`

Follow it with the generalized experimental paragraph. Then give a separate consistently formatted characterization paragraph for every compound. Do not append several compounds' analytical data to the General Procedure paragraph, and do not imply that exceptions used the common conditions.

### Single compound

Use the supplied heading or:

`Synthesis of XX.`

Give the complete experimental paragraph first and the compound's characterization paragraph immediately after it.

## NMR normalization

Preserve every supported analytical element: nucleus, operating frequency, deuterated solvent, δ values, multiplicity, coupling constants, and integration. Normalize typography and punctuation without changing the data.

Use these patterns:

`¹H NMR (400 MHz, CDCl₃) δ 7.26 (d, J = 8.4 Hz, 2H), 6.91 (d, J = 8.4 Hz, 2H), 3.82 (s, 3H).`

`¹³C NMR (101 MHz, CDCl₃) δ 170.2, 145.6, 128.4, 55.3.`

- Italicize *J*. In Markdown use `*J*`; in rich text apply true italics.
- Use `MHz` for frequency, `Hz` for coupling constants, `δ` before the signal list, commas between signals or shifts, and semicolons between analytical techniques.
- Retain source multiplicities and qualifiers, including `s`, `d`, `t`, `q`, `dd`, `dt`, `td`, `m`, `br s`, ranges, overlapping signals, and assignments when reported. Do not reinterpret a multiplicity or supply an assignment.
- Preserve all reported coupling constants and their association with the correct signal. Use `J = 8.4 Hz` or `J = 8.4, 2.1 Hz` as supported.
- Preserve integrations exactly. Do not force the total integration to match a proposed structure.
- Retain the source's nucleus-specific data. Do not create ¹³C data from a structure or from ¹H data, and do not add DEPT or heteronuclear NMR labels unless reported.
- Apply true superscripts/subscripts in rich text. The Unicode forms above are preferred in directly pasteable plain text.

## HRMS normalization and validation

The acquisition polarity and the reported ion are evidence, not boilerplate. Read both from the report.

Use:

`HRMS (ESI): m/z [M + H]⁺ calcd for CₓHᵧN_zOₙ [value]; found [value].`

Change the ion notation to the supported species, including `[M − H]⁻`, `[M + Na]⁺`, or another explicitly reported ion. Never mechanically use `[M + H]⁺`.

For every HRMS entry:

1. Record positive/negative polarity separately from ion/adduct type. Positive polarity does not by itself prove `[M + H]⁺`, and negative polarity does not by itself prove `[M − H]⁻`.
2. Use the formula that the instrument report associates with the calculated ion. Distinguish a neutral molecular formula from an ion formula. Do not convert between them unless the source or a fully supported calculation makes the relationship unambiguous.
3. Check that polarity, ion notation, ion formula, and calculated m/z are mutually consistent. When an exact-mass calculation is available, use it as a check rather than as a substitute for the source record.
4. Transcribe calculated and measured values from their correct report fields. Do not swap theoretical/calculated and observed/measured values.
5. Use the ppm error for verification. If the report supplies it, preserve that value in `Data check`. If it does not, ppm may be calculated as `(found − calcd) / calcd × 10⁶`, clearly labeled as calculated and rounded no more precisely than the source m/z values support.
6. Standard JMC characterization text reports `calcd` and `found` only. Add ppm to the manuscript text only when the user requests it.
7. If any field conflicts, do not silently repair it. Format only the supported portion, place an appropriate `[INSERT ...]` marker if needed, and describe the conflict under `Data check`.

Validated formatting examples:

- `541-2. ... HRMS (ESI): m/z [M − H]⁻ calcd for C₄₁H₄₅FNO₄ 634.3338; found 634.3343.` The source is negative mode; reported error 0.7 ppm.
- `541-3. ... HRMS (ESI): m/z [M + H]⁺ calcd for C₃₇H₄₆NO₄ 568.3421; found 568.3439.` The source is positive mode; reported error 3.1 ppm.
- `542-7. ... HRMS (ESI): m/z [M + H]⁺ calcd for [SOURCE-SUPPORTED ION FORMULA] 546.3214; found 546.3210.` The source is positive mode; reported error −0.7 ppm. Do not invent the formula when it is not present in the current input.

## Output and data check

Return the directly pasteable manuscript text first under `JMC Characterization`. Then add a compact `Data check` when analytical files were supplied. For each compound, report:

- matched source file(s), only when useful for traceability;
- HRMS polarity and ion type;
- calcd/found m/z and reported or calculated ppm error;
- any formula/ion mismatch, conflicting identifier, unreadable value, or unsupported field.

Keep routine checks brief. A suitable line is:

`541-2 — negative mode, [M − H]⁻; calcd 634.3338, found 634.3343; reported error 0.7 ppm; values consistent.`

Do not let `Data check` wording leak into the manuscript paragraph. If the data are internally consistent, state that concisely; if they are not, identify the exact field and source of uncertainty.

## Combined-output compatibility

When experimental steps and analytical files are supplied together, return:

1. `SI Experimental Procedure` following the parent skill;
2. `Scheme Reagents and conditions` following the parent skill, when requested;
3. `JMC Characterization` following this module;
4. `Data check` following this module.

Use one compound mapping across all parts. Compound labels, starting materials, products, and exceptions must agree. Do not use analytical data to invent or alter an experimental operation, and do not use a proposed structure or procedure to overwrite an instrument-reported ion.
