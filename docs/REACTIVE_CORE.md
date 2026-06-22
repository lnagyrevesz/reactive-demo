# REACTIVE_CORE.md — Constitutional Layer

**Authority:** Laurent Nagy-Revesz
**Status:** Permanent constitutional doctrine. Low-frequency change.
**Companion files:**
- Operational state: `/governance/state/CURRENT_STATE.md`
- Archived monolith (rollback anchor, historical reference): `/governance/archive/CLAUDE_v1_FINAL.md`
- Doctrine modules (future): `/governance/doctrine/*` (Q-π, Q-χ, Bible v3.1, absence taxonomy, FO template, W1.1 governance overlay)

This file contains the constitutional substrate of ReActive — the doctrine that does not change session-to-session and that governs every layer of the engine. Operational state, queue items, doctrinal modules with executable detail, DTD register entries, session history, and audit trail material live in their respective layers. They are not duplicated here.

---

## 1. What ReActive Is

ReActive is a deterministic forensic intelligence platform for institutional real estate due diligence. It ingests raw dataroom documents, extracts structured facts, reconstructs declared structures, tests internal coherence, and surfaces quantified deltas between reconstructed and reported values — identifying where claims across documents cannot simultaneously be true.

**ReActive quantifies differences between reconstructed and reported states under explicit assumptions. It does not recommend actions or interpret outcomes.**

The platform's analytical method derives from Project Stone (BRIF / Eurohypo, 2009), which identified a ~€200M NAV delta on Orco Property Group ahead of the company's structural failure. ReActive is engineered to make that method systematically reproducible.

---

## 2. Method DNA — Project Stone

Stone is not a feature, a module, or a marketing story. It is the **method spine** of ReActive. Every capability ReActive builds is assessed against the question: *"Would this have helped identify the €200M Orco delta in 2009?"* Capabilities that fail this test are deprioritised.

### The Stone method — five forensic layers

1. **Independent reconstruction** of portfolio structure from primary documents (per-asset valuations, broker reports, public disclosures), without relying on management summaries as the source of truth
2. **Reasoned scenario application** — per-asset, per-segment, per-geography haircuts with explicit anchored rationale
3. **Bottoms-up reconciliation** to a restated NAV, with full derivation trail
4. **Quantified delta** versus reported NAV, expressed as numbers with documentary basis
5. **Evidence-linked output** — descriptive and quantified, never advisory or prescriptive

### ReActive's Stone integration — V1 vs V2

- V1 absorbs **layers 1, 4, and 5**. V1 produces **Structural Deltas**: differences between independently aggregated values from the corpus and reported summary values. These are *coherence deltas*.
- V2 absorbs **layers 2 and 3**. V2 will produce **Scenario Deltas (Stone-class)**: differences between reported values and scenario-adjusted reconstructions.

The pipeline is identical for both. V2 only replaces "sum of reported per-asset values" with "sum of scenario-adjusted per-asset values." The architecture reserves the slot from V1 onward.

### Doctrinal commitments (locked)

**a) ReActive QUANTIFIES; it does not advise.** Outputs are numbers with documentary derivation. They are not recommendations. ReActive quantifies differences between reconstructed and reported states under explicit assumptions. It does not recommend actions or interpret outcomes.

**b) Reconstruction is INDEPENDENT of reported figures.** The system rebuilds structure from primary documents, then compares to reported values. It does not start from reported values and audit them.

**c) Every transformation is TRACEABLE.** Each value in an output must answer: *"What documentary basis and what assumption produced this?"*

**d) Deltas are quantified and contextualised; they are not translated into recommendations.** Interpretation is permitted (explanation, framing, market context). Prescription is not (recommendations, ratings, scoring of materiality, fault, or remediation).

### Anchoring sentence

*V1 does not reproduce Stone — but every V1 output must look like it comes from the same mind that produced Stone.*

### The Orco Test (release gate)

Before any V1 release candidate ships, it must pass the Orco Test — five binary questions with auditable answers, locked in `/docs/orco_test.md`. Failure on any criterion blocks release. The Orco Test is not a vibe check. It is a hard gate.

---

## 3. The Three Constitutional Principles

These principles were ratified 13 May 2026 by ChatGPT + Gemini converged ratification, elevated to constitutional status during the financial_statements REMEDIATION closure. They govern extraction-layer behavior absolutely and override any local prompt rule, schema annotation, or heuristic that conflicts with them.

### Principle 1 — The engine preserves documentary incoherence as evidence-bearing state unless explicitly authorized to normalize.

When a value appears differently in different sections of the same document, both stated values MUST be preserved at their respective extraction paths. They must NOT be reconciled, normalised, or collapsed to a single value by the extractor. Section-priority resolution rules of any kind are forbidden inside extraction prompts. Downstream forensic objects are the authorized layer for analyzing such divergences; extraction must preserve the divergence intact for that analysis to be possible.

**Operational consequence:** ReActive sells the work (rigorous deliverable) because the method preserves divergence (forensic orientation). Silent reconciliation would collapse that posture into ordinary extraction.

### Principle 2 — Canonical path ≠ exclusive truth.

When two schema paths carry the same conceptual fact, the canonical path is the recommended consumer choice for downstream forensic objects — but the secondary path is **preserved as evidence-bearing, not deprecated**. Both extractions remain in the JSON; neither is silenced. Downstream FOs may legitimately reference either path or both.

**Corollary:** Schema architectural redundancy (two paths for one conceptual fact) is not a defect to be collapsed; it is observation-bearing structure to be preserved.

**Empirical anchor:** NorthGate FY2024 extraction shows `distributions_to_parent = -2,723,343` at `$.balance_sheet` vs `+2,723,343` at `$.related_party_transactions` — same absolute value, divergent sign, both extracted with section-specific source attribution.

### Principle 3 — No silent reconciliation.

Reconciliation of section-divergent values is a forensic-objects responsibility, not an extractor's. Any prompt rule that selects between two stated values is reconciliation; any prompt rule that preserves both is forensic. The extractor MUST emit both values when both are stated; the FOs may then analyze, compare, contradict, or collapse them per their analytical logic — visibly, with full provenance.

**Contrapositive (load-bearing):** If a prompt rule produces a single value from two stated values, the extractor is operating in reconciliation mode, which is forbidden.

Principle 3 is the negative-space counterpart to Principle 1; together they form an inviolable pair governing extraction-layer behavior.

---

## 4. Engine Architecture (Constitutional Shape)

```
RAW VDR → INGESTION → EXTRACTION → STRUCTURE RECONSTRUCTION → FO TESTING → DELTA COMPUTATION → FINDINGS
```

- **Ingestion:** Document classification, deduplication, format conversion.
- **Extraction:** LLM-assisted, schema-constrained. **AI BOUNDARY — only layer using LLM.**
- **Structure Reconstruction:** Entity Graph, Debt Layer, Temporal Layer, Income Layer. Deterministic.
- **FO Testing:** Pure Python, no AI. Deterministic.
- **Delta Computation:** Structural Deltas (V1) → Scenario Deltas (V2). Deterministic.
- **Findings:** JSON with full evidence chains. Deterministic replay via `extraction_manifest.json`.

**Core rule (constitutional):** Same corpus in → same findings out → every time.

**AI boundary (constitutional):** LLM-assisted behavior is confined to the extraction layer. All downstream layers — reconstruction, FO testing, delta computation, findings emission — are deterministic and AI-free. Probabilistic / confidence-based routing, multi-archetype extraction per document, and ingestion-platform probabilistic logic are explicitly NOT V1 capabilities. V1 routing remains deterministic registry-based via `CORPUS_INVENTORY` per Q-π.15. Reconsideration is permitted only on empirical evidence from adversarial dataroom testing.

---

## 5. Provenance Invariant

Every extracted fact MUST carry provenance.

**Canonical pair (Q-α, locked under Bible v3.1):** Every extracted scalar is a `{value, source}` pair. Composite blocks contain such pairs; composite blocks are never themselves wrapped.

**Canonical key name for provenance attribution is `source`.** Aliases (notably `provenance`) are forbidden and treated as wrapper-key violations.

**Provenance placement (Q-π.18):** Provenance MAY be attached at the node level or **inherited from an ancestor structure** when the schema defines the node as non-provenance-bearing. A node that does not carry its own `source` is not provenance-less; it is **parent-anchored**. This is not a relaxation of the invariant — it is an extension of how provenance attaches to the data tree.

**Three legitimate placements of one invariant:**
- Atomic block — block-level `source` covers all bare-primitive children
- BARE_DICT — ancestor's `source` covers the entire sub-structure
- Q-χ.C value-not-found — local sentinel source attached; provenance preserved at document level, evidence explicitly absent

Provenance is never silently dropped, synthesized, or back-filled. Synthetic provenance construction by any downstream consumer is forbidden.

---

## 6. Absence Semantics

ReActive represents absence at three structurally distinct surfaces. Each surface has exactly **one** canonical absence shape. The three shapes are not interchangeable; mixing them produces representation defects.

**The taxonomy is complete with respect to current schema patterns.** Every absent-fact representation in the engine maps to exactly one of the three. Future schema patterns surfacing a fourth absence shape require explicit doctrinal extension; ad-hoc fourth-shape emissions are doctrine-forbidden.

### Pattern 1 — Q-χ.C: Wrapped scalar absence

**Surface:** WRAP-classified paths emitting `{value, source}` pairs at extraction.

**Canonical shape:**

```json
{
  "value": null,
  "source": {
    "document": "<real source filename>",
    "page": null,
    "section": null,
    "reference": "NOT FOUND"
  }
}
```

**Semantic interpretation:** Search-and-fail. The extractor performed a directed search for this specific scalar fact in the named document and did not find it. Provenance is preserved (`document` remains real); only the fact-existence claim is the sentinel.

**Detection key (downstream consumers):** `value is None AND source["reference"] == "NOT FOUND"`. The `document` field carries real data and MUST NOT be tested as part of sentinel detection.

**Universal application:** Q-χ.C applies to ALL wrapped fields, including fields where the schema permits `oneOf: [sourced_* | null]`. Raw `null` at a wrapped-field position is forbidden — the canonical sentinel is the only legal absence representation. The schema's `oneOf` permissiveness is for downstream validator tolerance; the canonical extraction shape is always the Q-χ.C sentinel.

**Mixed-state prohibition:** If either `page` or `section` is non-null while `reference == "NOT FOUND"`, the pair represents a contradictory mixed state and MUST be rejected. The extractor cannot simultaneously claim to know which page contains the fact AND that the fact is not found.

### Pattern 2 — Q-δ: Block-level absence

**Surface:** ATOMIC_BLOCK paths whose schema declares them as conditionally absent via a structural `exists` flag.

**Canonical shape:**

```json
"<block_name>": { "exists": false, "source": null }
```

For blocks without a sibling source convention:

```json
"<block_name>": { "exists": false }
```

**Semantic interpretation:** The entire block is structurally absent in the document. Absence has no citable source; the bare sub-fields have no meaningful value to carry when the mechanism does not exist. The structural flag (`exists: false`) is the only positive evidence required.

**Allowed keys under absence:** When the block is absent, allowed keys are exactly `{flag_key, "source"}` (or `{flag_key}` alone, per the variant above). Any other keys — hallucinated sub-fields, leftover bare null fields — are representation defects.

### Pattern 3 — Rule 19.1: Nullable-array absence

**Surface:** Optional array fields schema-typed as `["array", "null"]`.

**Canonical shape:** The field is **OMITTED entirely from the output JSON**. No `null`, no `[]`, no sentinel — the key is simply absent from its parent object.

**Semantic interpretation:** Absence by omission. The corresponding facts are not present in the document, and no in-band representation is needed — the field's absence from the output is itself the canonical signal.

**Why omission, not null, not empty array:**
- Raw `null` at the array position fails strict list-or-fail validation.
- Empty array `[]` is shape-valid but semantically misleading (implies the extractor found and processed an empty list, vs. found nothing to extract).
- Omission is unambiguous: the dispatcher walks the parent traversal node, never encounters the unmapped key, and emits no error.

**Doctrinal symmetry:** Rule 19.1 is the array-level analogue of Q-δ block-level absence. Both use omission / structural-flag rather than null-emission to represent the absence of a structural surface. Q-χ.C is structurally distinct because it applies to wrapped-scalar surfaces where local provenance must be preserved even in absence.

### Three-shape comparison

| Pattern | Surface | Canonical shape | Absence signal carrier |
|---|---|---|---|
| **Q-χ.C** | WRAP scalar (`{value, source}`) | `{value: null, source: {document: real, page: null, section: null, reference: "NOT FOUND"}}` | `source.reference == "NOT FOUND"` |
| **Q-δ** | ATOMIC_BLOCK with structural flag | `{exists: false, source: null}` or `{exists: false}` | `exists: false` |
| **Rule 19.1** | Optional array (`["array", "null"]`) | (field omitted entirely) | Absence of key in parent |

### Boundary discipline (constitutional)

- **Mixing patterns is forbidden.** A wrapped field cannot use Q-δ shape (`exists: false`). A block cannot use Q-χ.C `NOT FOUND` sentinel. An array cannot use `null`-emission. Each surface has exactly one legal absence representation.
- **New schema patterns require doctrinal extension.** If a future schema surfaces a fourth absence shape (e.g., nullable-map, nullable-tuple), the case requires explicit ratification before any extraction prompt emits the new shape.
- **Q-δ and Q-χ.C never coexist on the same field.** Q-δ applies when the BLOCK is absent (structural flag false). Q-χ.C applies when the BLOCK is present but a specific WRAPPED scalar field within it could not be located.
- **BARE_DICT null is NOT Q-χ.C.** BARE_DICT children with null values represent projection-layer absence (provenance inherited via upward traversal), not search-and-fail. Q-χ.C detection logic MUST NOT be applied to BARE_DICT children. Reported by FOs as `evidence_unavailable_at_projection_layer`, distinct from `evidence_unavailable`.

### Doctrine module pointer

Validator accept conditions (the 6-part Q-χ.C strict conjunction, the Q-π.14 triple-gate enforcement for Q-δ, the Q-π.14.A garbage-keys check), full downstream consumer detection contracts, and the relationship to Q-π.7 / Q-π.18 / BARE_DICT live in the doctrine module. Until that module is extracted from the archived monolith, the authoritative reference is `/governance/archive/CLAUDE_v1_FINAL.md` (sections ABSENCE TAXONOMY, Q-χ RULES, Q-π RULES Q-π.14, Q-π.18).

---

## 7. Schema Archetypes (Constitutional Frame)

ReActive supports exactly **two** schema archetypes. Every classification module MUST declare its archetype via an `ARCHETYPE` constant restricted to a two-element controlled enum:

- `ARCHETYPE = "envelope"` — administrative documents (contracts, minutes, agreements, statements)
- `ARCHETYPE = "analytical"` — analytical documents (valuation reports, financial models)

No other values permitted. No free-text variants. No subtypes. The constant is future-executable metadata read by the validator and downstream tooling.

A classification module without an `ARCHETYPE` constant, or with an `ARCHETYPE` value outside the two-element enum, is a deployment defect surfacing at validator load time.

The cross-archetype shared invariant is the `{value, source}` provenance pair (Section 5 above). Archetype declaration governs administrative-vs-analytical shape conventions; it does not relax the provenance invariant.

---

## 8. Forensic Object Discipline

### Three canonical FO types

1. **Contradiction** — A ≠ B → impossible coexistence. Status: `contradiction_detected`.
2. **Structural Tension** — A and B coexist, dependency unresolved. Status: `structural_tension_detected`.
3. **Structural Dependency** — Declared independence, structural linkage present. Status: `structural_dependency_detected`.

### Required FO output architecture

Every FO output carries three structural elements:

- **evidence_chain** — facts only, sourced, referenced, no interpretation
- **structural_test** — logical alignment of facts, descriptive not assertive
- **conclusion** — coexistence or incompatibility statement plus uncertainty boundary

### Forbidden in FO outputs

The following language is forbidden in FO outputs: *material*, *suggests*, *implies*, *can lead to*, *can propagate*, *inconsistent with reality*.

**No severity scoring. No HIGH/MEDIUM/CRITICAL.**

### FO reading contract (binding on all FOs, current and future)

- **Q-χ.C facts:** any FO that depends on a Q-χ.C-flagged fact reports `evidence_unavailable` and exits the relevant test branch without firing `contradiction_detected` or `structural_tension_detected`. The field is excluded from all computation, comparison, aggregation, and contradiction detection.
- **BARE_DICT null:** reported as `evidence_unavailable_at_projection_layer`. Q-χ.C detection logic MUST NOT be applied to BARE_DICT children.
- **Missing required input:** FO aborts the test and emits `input_unavailable`. No default values, no zero-substitution, no skip-and-continue.
- **Conflicting valid inputs:** FO emits `contradiction_detected` with both citations in the evidence chain.
- **No interpolation, no inference, no synthetic provenance, no null-to-zero casting.**

The four unavailability classes (`evidence_unavailable`, `evidence_unavailable_at_projection_layer`, `input_unavailable`, `evidence_chain_broken`) MUST NOT be collapsed into a single "no data" code at the FO output level.

---

## 9. Language Doctrine

### Prohibited in any engine output

*red flag*, *warning sign*, *risk indicator*, *suggests fraud*, *valuation concern*, *material risk*, *recommendation*, *prediction*, *forecast*, *probability of loss*, *default*, *breach*, *crisis*, *material* (qualitative-judgment sense), *suggests*, *implies*, *should*, *must*, *advise*, *high risk*, *concerning*, *significant* (qualitative-judgment sense).

### Required terms

*inconsistency*, *structural contradiction*, *finding*, *structural tension*, *gate not satisfied*, *coherence gap*, *structural dependency*, *delta*, *reconstructed value*, *structural delta*, *scenario delta*.

---

## 10. Document Layer Separation

Engine code, config files, and test outputs may reference FO codes, Bible sections, and internal terminology freely.

**BUT:** If this engine ever generates or modifies documents intended for a dataroom, those documents must **NEVER** contain: *FO-*, *Bible*, *canonical*, *ReActive*, *CLAUDE.md*, *forensic object*, *evidence_chain*, *structural_test*, *run_scan*, *extraction_config*, *findings.json*, *run_summary*, *run_manifest*, *structural_tension_detected*, *contradiction_detected*, *structural_dependency_detected*, *Stone*, *Orco Test*, *Q-π*, *Q-α*, *Q-β*, *Q-γ*, *Q-δ*.

Dataroom documents must read as if written by the persons named on them, with zero awareness that any forensic engine exists.

---

## 11. Real Dataroom Robustness — Two Doctrines (Locked 6 May 2026)

ReActive's V1 architecture is validated against synthetic, intentionally-clean corpora. Real institutional datarooms do not arrive that way. To prevent ontology overfitting, two doctrines are constitutional:

### Doctrine A — Classification is non-blocking.

All documents are ingestible by the engine. Classification only determines extraction depth and precision, not eligibility. A document that fails to match a specific doctype routes to a generic fallback, not to skip. Taxonomy uncertainty is a routing decision, not a blocking error.

**Important nuance:** fallback extraction is a coverage mechanism, not a parity mechanism. FO findings carry implicit provenance about routing path; a finding sourced from a fallback-routed document is structurally weaker than a finding sourced from a specific-doctype document, and the FO output should expose this rather than hide it behind a uniform "finding" abstraction.

### Doctrine B — Corpus organization is advisory, not authoritative.

Filenames, folders, metadata, and declared dataroom organization carry useful signal but are NOT treated as ground truth. The engine does not infer doctype from filename alone, does not trust folder placement as canonical, does not assume metadata accuracy. This protects against the engine inheriting false assumptions from dataroom organization choices made for narrative purposes rather than structural correctness.

### Explicitly deferred (NOT committed in V1)

Probabilistic / confidence-based routing, multi-archetype extraction per document, full ingestion-platform rebuild, Stage 0/1/2/3 pipeline. These are listed by name to prevent scope drift. V1 routing remains deterministic. Probabilistic routing has architectural cost — it breaks reproducibility at the routing layer and weakens the forensic audit trail that ReActive's fund-manager liability posture depends on — and is not adopted without empirical evidence that deterministic routing fails on real datarooms.

### Strategic framing

ReActive is a **contradiction detection engine built on document structure, not a document classification system**. The priority is to extract usable structure from everything, improve precision via classification where possible, and never block ingestion on taxonomy purity.

---

## 12. Reference Distribution Discipline (Locked 14 May 2026)

The Northgate and Quorum corpora are controlled development corpora created to support methodological stabilization of ReActive's forensic extraction and contradiction-detection architecture.

Their relative cleanliness compared to real institutional datarooms is a development-stage constraint and MUST NOT be interpreted as the engine's target operating distribution.

ReActive's reference distribution is the realistic institutional dataroom environment, including (non-exhaustively):

- heterogeneous filename conventions
- OCR degradation
- partial scans
- multilingual fragments (including non-Latin scripts)
- inconsistent labeling
- duplicated uploads
- hybrid formats
- broker shorthand
- code-name structures
- incomplete provenance
- and other forms of documentary incoherence common in institutional real estate operations

Accordingly:

- No filename convention is treated as structurally canonical.
- No realistic dataroom filename pattern is treated as adversarial by default.
- Robustness claims MUST be evaluated against heterogeneous real-world documentary conditions rather than against the cleanliness of development corpora.

Development corpora exist to stabilize methodology, not to define ontology.

### Anti-symmetric corollary

This clause does NOT establish a preference for irregular or degraded filenames. Institutional datarooms contain pristine law-firm exports and banker-curated PDFs alongside scanner debris and broker shorthand. The reference distribution is *heterogeneity itself* — the simultaneous presence of all these forms — not any subset of them. Any framing that privileges either clean or irregular inputs as more "realistic" than the other is a category error.

### Relationship to existing constitutional ground

This clause makes explicit a posture that was already implicit in §1 (forensic identity — ReActive's value increases with documentary incoherence), §2 (Project Stone DNA — the Orco method operated on heterogeneous, partial, internally inconsistent material), and §11 (Real Dataroom Robustness — corpus organization is advisory, not authoritative). The clause was added because operational framings of pilot work could drift against these existing principles in ways that operational locks alone cannot prevent. It belongs in the constitutional layer because the drift it prevents is a class of drift, not a single instance.

---

## 13. Working Protocols (Operator / Assistant Model)

Laurent is the **execution operator and product owner**, not an engineer. The interaction model is non-negotiable.

### User role — what is in scope

- Run scripts and commands on Replit
- Paste provided files or code blocks into the workspace
- Report outputs back to the AI assistant
- Validate results at the business / methodological level

### User role — what is OUT of scope

- Debugging code
- Inspecting or reasoning about implementation details
- Modifying code beyond direct paste-and-replace operations
- Making technical design decisions at the file or function level

### Assistant obligations — file handling

- The assistant produces **complete, ready-to-paste files**. Laurent pastes-and-replaces.
- Never instruct Laurent to "edit line X", "insert this section", "add this to your file", or any partial-edit operation. If a file changes for any reason, regenerate the entire file.
- This applies to governance files, code, configs, prompts, schemas, and any other persistent artifact.
- **File authorship is reserved to Claude.** Gemini and ChatGPT are audit partners, design ratifiers, and second-opinion reviewers — not file authors. If Gemini or ChatGPT volunteers to "author" or "write" a file, the offer must be declined. Correct workflow: another AI ratifies design → Claude drafts the file as paste-and-replace → another AI reviews the drafted file → Laurent pastes.

### Assistant obligations — verification

When verification of system state is required, the assistant MUST:

- Provide an exact command for Laurent to run, framed as "paste this into your Replit shell"
- Interpret the result based on the output Laurent pastes back

The assistant MUST NEVER:

- Ask Laurent to "open file X and check line Y"
- Ask Laurent to "look at" or "verify" implementation details
- Ask Laurent to read, analyze, or reason about code
- Delegate engineering reasoning tasks to Laurent in any form

### Communication

- No commentary on Laurent's life, time of day, work patterns, or schedule.
- Push back substantively on disagreements when warranted. Accept correction when wrong.
- Do not make Laurent repeat himself. If a rule lands once, it stays landed.

### Authority

These protocols cannot be relaxed by any AI. Any future Claude session that violates them is failing the project, not optimizing it.

---

## 14. Execution Boundary (Locked 27 April 2026)

No AI assistant has access to:
- The Replit environment
- The master archive on Laurent's MacBook Air
- Any running engine, script, or pipeline

All execution is performed by Laurent. AI outputs claiming to report execution results are synthesis or hallucination and must be treated as such until Laurent pastes real output into the conversation.

### AI roles

- **Claude Pro:** governance, doctrine, code review, analysis of outputs Laurent reports.
- **Gemini 2.5 Pro:** structured extraction at temperature 0, audit partner, analysis of outputs Laurent reports.
- **ChatGPT:** second-opinion partner for cross-review of strategic decisions.

### Contamination triggers

Any AI message containing phrases like *"I ran..."*, *"I executed..."*, *"the pipeline produced..."*, *"the batch completed..."*, *"the run returned..."*, *"results show..."* — without Laurent having pasted real output into the conversation — is a contamination event and must be quarantined.

### Authority

This boundary cannot be relaxed by any AI. Only Laurent can ratify execution outputs.

---

## 15. Design Decisions Taxonomy (Disciplinary Frame)

All design-related entries in ReActive's governance fall into exactly four categories. The category label is part of the entry, locked at ratification, to prevent doctrine drift:

- **Doctrine** — binding principle governing engine behavior. Ratified, locked, only changeable by explicit constitutional amendment.
- **Observation** — empirical finding awaiting characterization. Not binding. May or may not promote to doctrine; may or may not promote to DTD.
- **DTD (Deferred Technical Debt)** — deterministic, structurally characterizable defect with engine-layer remediation surface. Promotion criteria: determinism (≥3 reproductions), engine-layer remediation surface identified, closure criteria definable in advance.
- **Governance Characterization** — recorded description of process or role dynamics (e.g., three-AI workflow). Not doctrine, not defect, not observation pending promotion.

### DTD Discipline Rule

DTDs are reserved for **deterministic, structurally characterizable defects** that can be reproduced and remediated at the engine layer. Stochastic noise from the upstream LLM at temperature 0 — including run-to-run variance, transient parse failures, and content-correlated but non-byte-stable failures — does NOT meet the bar for DTD opening. Such phenomena are recorded as observations.

The deterministic/non-deterministic distinction is the gating criterion, not the structural/semantic distinction.

---

## 16. Doctrine Modules — Pointer

The following doctrine modules govern executable behavior and are referenced here by name. Their full text lives in the archived monolith (`/governance/archive/CLAUDE_v1_FINAL.md`) and will be extracted into `/governance/doctrine/*` during future modularization. Until then, the archived monolith is the authoritative source for each:

- **Q-π rules** — runtime path normalization, strict mode, archetype declaration, block-absence triple-gate, schema archetypes, parent-anchored provenance (Q-π.1 through Q-π.18)
- **Q-χ rules** — value-not-found semantics, single-value not-found sentinel (Q-χ.C)
- **Bible v3.1 doctrine** — Option A invariant, Q-α through Q-δ wrapping rulings, structural flag handling
- **Absence taxonomy** — three-part canonical representation (Q-χ.C wrapped scalar, Q-δ block, Rule 19.1 nullable array) with full canonical shapes, validator accept conditions, and downstream consumer detection contracts
- **W1.1 Governance Overlay** — E.4-B residual analysis grid, FO interpretation doctrine
- **FO template v1.3** — gold-standard FO architecture
- **Q-π.17 archetype declaration table** — locked archetype assignment per the seven governed doctypes

These modules are doctrine. They are stable. They are not duplicated here. Modularization into `/governance/doctrine/*` proceeds gradually, after this two-file decomposition is verified stable.

---

## 17. Authority

This file is the constitutional layer of ReActive's governance. It is authored by Claude per the file-authorship discipline. It is ratified by Laurent. ChatGPT and Gemini are audit partners.

Amendments to this file require explicit constitutional-amendment ratification — they are not made through routine session work. Operational adjustments, queue changes, lock status changes, and DTD register updates all happen in `CURRENT_STATE.md` or in the doctrine layer, not here.

The archived monolith (`/governance/archive/CLAUDE_v1_FINAL.md`) is the canonical historical source. Where this file and the archived monolith diverge on constitutional matters, the archived monolith governs until reconciled by explicit amendment.
