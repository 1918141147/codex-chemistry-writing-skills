---
name: jmc-manuscript-workflow
description: Draft or revise Journal of Medicinal Chemistry manuscripts for natural-product semisynthesis, analogue optimization, SAR, and pharmacology. Use when the user supplies project files or asks for a JMC-style medicinal chemistry manuscript, section, or Word revision. Always complete the required study-theme, group-publication, and pharmacology-data confirmation gate before drafting.
---

# JMC Manuscript Workflow

Produce an evidence-grounded JMC manuscript whose chemistry, biological story, figures, experimental procedures, citations, and Word formatting agree with the user's latest accepted materials.

## Mandatory intake gate

Before drafting or substantively revising manuscript prose, read [references/intake-gate.md](references/intake-gate.md) and obtain the three required confirmations:

1. the study theme: compound class/scaffold, modification campaign, biological activity, disease/model context, and intended endpoint;
2. the exact group publications and claims allowed for the “our group has long pursued…” background paragraph;
3. when pharmacology data are absent or incomplete, whether to write chemistry only or wait for a minimal pharmacology package from the user.

This gate applies even when the answers appear inferable from supplied files. State the inference and ask the user to confirm or correct it. File review and source inventory may proceed while waiting, but manuscript drafting must not.

## Source authority

- Treat the user's latest accepted manuscript and explicit current-turn instructions as the editing authority.
- Treat experimental records, NMR/HRMS files, assay outputs, and designated pharmacology reports as data authorities within their scopes.
- Treat PPT notes, Chinese comments, and annotations as author guidance or hypotheses, not verified scientific results.
- Treat example JMC papers as models for prose architecture, transitions, claim restraint, and caption logic; never copy their facts or language into the new study. Do not reproduce a published article's typeset page geometry in a submission manuscript. Follow the current JMC author template or guidelines for submission structure and page formatting.
- When sources conflict, stop at the conflict, report it precisely, and ask which source governs. Do not silently reconcile chemistry, compound numbering, yields, assay results, or mechanisms.

## Workflow after confirmation

1. Inventory and classify all supplied files using the source map in [references/intake-gate.md](references/intake-gate.md).
2. Establish the current manuscript baseline, requested edit scope, and next short version name. Preserve all content outside scope.
3. Build the section-level argument using [references/manuscript-architecture.md](references/manuscript-architecture.md).
4. Draft chemistry, SAR, pharmacology, and experimental text under [references/chemistry-pharmacology-rules.md](references/chemistry-pharmacology-rules.md).
5. Apply the JMC and Word conventions in [references/format-and-qa.md](references/format-and-qa.md).
6. Run a claim-evidence check, chemistry consistency check, citation check, and document-format check before delivery.

## Writing boundaries

- Do not invent assay values, yields, masses, compound identities, stereochemistry, target engagement, causal mechanisms, or in vivo efficacy.
- Use `lead compound` rather than `probe` unless the work actually establishes and uses a chemical probe.
- Keep Results and Discussion chemistry concise and design-led; place reproducible operations and quantities in the Experimental Section or Supporting Information.
- Base pharmacology claims only on supplied data. Separate observation, association, and mechanism; use cautious language when target engagement or causality is not demonstrated.
- Verify current JMC author requirements and publication status of cited papers when current accuracy matters; do not hard-code mutable word limits or article-status information.
- For Word edits, use minimal local changes, retain images and unrelated text, and create a new version rather than overwriting the accepted baseline.

## Deliverables

Return the requested manuscript or revised section in the user's existing format. For DOCX work, preserve paragraph hierarchy, figures, captions, compound styling, and reference formatting. When DOCX rendering tools are available, rendering and visual inspection are mandatory before delivery. If the renderer is unavailable, complete structural integrity checks and clearly disclose that visual QA could not be performed.
