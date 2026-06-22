# CURRENT_STATE.md — Operational State Layer

**Authority:** Laurent Nagy-Revesz
**Last canonical freeze:** 13 May 2026
**Item 28 closure:** 15 May 2026 — CHARACTERIZATION COMPLETE, scoping memo v1.4 ratified (post-ChatGPT-review refinements), Step 7.5 promotion decision recorded (DTD-008 NOT promoted; retained as established observation)
**Reference Distribution Discipline (REACTIVE_CORE.md §12) Locked:** 14 May 2026 evening
**Item 24 design phase closure:** 16 May 2026 — eight locked doctrinal artifacts plus one observational artifact produced; execution authorization remains a separate downstream operator gate
**Item 24 Tier 0 closure:** 20 May 2026 — methodology-validation phase on non-production substrate complete; closure memo locked v1.0; production characterization (Tier A) remains unauthorized
**Item 29 design session:** 24 May 2026 — design session proper opened and closed; Bounded Ontology Memorandum produced (non-canonical, `/governance/sync/`); no doctrine, schema, validator, or engine surface touched
**Residual #12 closure:** 25 May 2026 — Item 28 entropy-filename rollback executed under operator execution gate (three-AI agreement); seven `[ENTROPY: Item 28]` keys in `CORPUS_INVENTORY` reverted to canonical via position-preserving in-place swap (Clean Restoration); Lock 4 held; `[:72]` boundary verified intact
**Positional-fragility resolution:** 25 May 2026 — corpus-boundary determination in `discover_documents()` migrated off the `[:72]` positional slice to explicit membership sets plus an import-time invariant; first exercised Lock 4 exception, narrowly scoped to corpus-boundary logic in `extract_documents.py` only (Approach B; `CORPUS_INVENTORY` values kept as bare strings)
**Item 29 doctrine lock:** 25 May 2026 — first locked canonical doctrine arising from Item 29: Q6 (flag singularity-vs-fracture) and Q4a (intent detection-vs-meaning-side) adjudicated via Path C and locked in `/governance/doctrine/item_29_completeness_ontology.md` (v1.0); Q1, Q2, Q3, Q4b, Q5 remain deferred to Tier A; Lock 4 holds (doctrine is not execution authorization)
**Tier A perturbation doctrine lock:** 27 May 2026 — `/governance/doctrine/tier_a_perturbation_spec.md` (v1.0) locked via signed adjudication memo; filename-only perturbation across BASE + twelve admissible buckets (A, B, C, D1, E, F, G, H, I, J, K, L), `{document_content}` byte-identical to BASE, one deterministic variant per bucket per representative document, single-bucket only; D2 excluded; eight signed operator rulings recorded
**Tier A prepare-phase code gate exercised:** 27 May 2026 — narrow code gate (doctrine §8 / ruling 8) opened and closed; `scripts/run_tier_a_batch.py` extended from BASE-only (21 requests) to BASE + 12 filename buckets (273 offline request-definitions = 13 conditions × 7 documents × N=3), prepare-phase only; `--submit`/`--retrieve` remain dormant; no schema/validator/FO/prompt/engine change; no Tier A execution
**Positioning doctrine ratified:** 7 June 2026. `/governance/doctrine/positioning_doctrine.md` (v1.0 LOCKED). Ratification chain: Claude authored under operator drafting gate, ChatGPT reviewed (ratifying review of record), operator ratified. Presentation and demonstration posture only; defers to `REACTIVE_CORE.md` §12 and `item_24_heterogeneity_taxonomy.md` on what counts as realistic institutional conditions; governs presentation, not corpus composition. Not engine behavior, not a Lock 4 surface. Recorded as active; the doctrine's substance lives in the artifact
**Doctrine register reconciliation:** 7 June 2026. Two locked doctrine-layer artifacts present on disk but previously absent from this file's registers are now recorded: `substrate_identity_discipline.md` (v1.0 LOCKED, cross-Item methodological doctrine) and `tier_a_adjudication_memo.md` (signed decision memo, 27 May 2026, the basis for the Tier A perturbation rulings). Documentation-versus-repository reconciliation only; no doctrine, engine, schema, validator, or FO change; not a Lock 4 surface.
**Test #3 closure:** 19 June 2026 — re-derivation of the three NorthGate/Quorum demo findings (FO-NTH-001, FO-NTH-002, FO-QRM-020) against the cleaned corpus is complete; all three findings ran successfully against fresh extractions. A new doctype, `rent_roll` (v1.0 schema, v2 prompt), was added to the extraction pipeline — the tenant schedule document had previously been classified `metadata_only` and had never been extracted. `fo_nth_001_exit_window.py` required a rewrite of its rent-roll-reading logic, which had been written against a fictional, pre-aggregated schema that never matched any real extraction output; rewritten and verified against real data. Authoritative locked figures and wording constraints for demo use are recorded separately in `/governance/sync/TEST_3_REFERENCE_LOCK.md` (non-canonical, display-authoritative for these three findings only). See residual #11 dated note below for the governance lesson arising from this session.
**Version:** v2.5 (19 June 2026. Test #3 closure state update. Records the closure of Test #3 (NorthGate/Quorum demo-finding re-derivation), the addition of the `rent_roll` doctype, the FO-NTH-001 rewrite, and a dated reinforcement note appended to residual #11. Updates: version header, one new dated milestone line, one §1 posture sentence, one Active Queue Immediate entry, and a dated note appended to residual #11 in §7. No constitutional or doctrine-layer change; this is operational-state and residual-registry update only.)
**Version (prior):** v2.4 (13 June 2026. Demo-track document-hygiene state update, recorded on the presentation-layer track and orthogonal to the engine-governance posture above. Records a session-verified corpus metadata scrub across both local datarooms and the NorthGate model workbook provenance strip plus four-layer reconciliation. Updates: version header to v2.4, a §1 demo-track posture sentence, one Active Queue Immediate entry carrying the full session-record entry, and this header line. Presentation and Tier 2 hygiene only; no engine, schema, validator, FO, prompt, doctrine, or code change; touches no lock and is not a Lock 4 surface. Prior v2.3 doctrine register reconciliation and earlier entries unchanged.)
**Version (prior):** v2.3 (7 June 2026. Doctrine register reconciliation. substrate_identity_discipline.md and tier_a_adjudication_memo.md, both already present on disk, are added to the companion-files block and the §8 repository tree, which previously omitted them. Documentation reconciliation only, recording existing artifacts; no engine, schema, validator, or FO change; not a Lock 4 surface. Prior v2.2 positioning entry and v2.1 Tier A bookkeeping unchanged.)

**Companion files:**
- Constitutional layer: `/governance/constitution/REACTIVE_CORE.md`
- Archived monolith (rollback anchor): `/governance/archive/CLAUDE_v1_FINAL.md`
- Item 28 scoping memo v1.4: `/docs/item_28_scoping_memo.md` (active reference; §14.5.1 names three distinct validator-surface gaps; §15.7 forward-looking generalization conditional; historical framing preserved per pre-registration discipline)
- Item 28 pre-registration: file no longer present on disk; operational content preserved by inline reference within scoping memo §§1, 9, 13 (see residual #9)
- Item 24 pre-registration synthesis: `/governance/preregistration/item_24_preregistration.md`
- Item 24 doctrine modules: `/governance/doctrine/item_24_*.md` (six files)
- Item 24 Tier 0 closure memo: `/governance/results/item_24_tier_0_methodology_validation_results_memo.md` (v1.0 LOCKED — first execution-result artifact)
- Governance Observation 001: `/governance/observations/item_24_governance_observation_001.md`
- Item 29 pre-opening charter + memorandum: `/governance/sync/ITEM_29_PRE_OPENING_CHARTER.md`, `/governance/sync/ITEM_29_PRE_OPENING_MEMORANDUM.md` (non-canonical)
- Item 29 Bounded Ontology Memorandum: `/governance/sync/ITEM_29_BOUNDED_ONTOLOGY_MEMORANDUM.md` (non-canonical — design-session output)
- Item 29 completeness ontology doctrine: `/governance/doctrine/item_29_completeness_ontology.md` (v1.0 LOCKED — Q6 and Q4a rulings; first canonical doctrine from Item 29)
- Tier A perturbation specification: `/governance/doctrine/tier_a_perturbation_spec.md` (v1.0 LOCKED — filename-only perturbation doctrine; BASE + twelve buckets; eight signed operator rulings)
- Positioning doctrine: `/governance/doctrine/positioning_doctrine.md` (v1.0 LOCKED, 7 June 2026. Presentation and demonstration posture; not engine doctrine, not a Lock 4 surface. Records existence and active status; substance lives in the artifact.)
- Substrate identity discipline: `/governance/doctrine/substrate_identity_discipline.md` (v1.0 LOCKED, 17 May 2026. Cross-Item methodological doctrine; substrate-identity binding of findings to model, provider, and temperature.)
- Tier A adjudication memo: `/governance/doctrine/tier_a_adjudication_memo.md` (signed decision memo, 27 May 2026. The operator adjudication basis behind the eight Tier A perturbation rulings; design and governance only, not executable doctrine.)
- Tier A batch orchestration: `scripts/run_tier_a_batch.py` (prepare-phase only; BASE + 12 buckets = 273 offline request-definitions; `--submit`/`--retrieve` dormant)

This file contains current operational posture. It is intentionally dynamic and expected to evolve frequently. It does **not** carry constitutional doctrine, closed remediation chronology, or session history — those live in their respective layers.

---

## 1. Current Posture

```
HOLD → CANONICAL FREEZE → GOVERNANCE DECOMPOSITION → ITEM 28 PILOT (CLOSED) → REFERENCE DISTRIBUTION DISCIPLINE LOCKED → ITEM 28 CHARACTERIZATION COMPLETE → ITEM 24 DESIGN PHASE CLOSED → ITEM 24 PRE-REGISTERED → ITEM 24 TIER 0 METHODOLOGY VALIDATION CLOSED → ITEM 29 DESIGN SESSION CLOSED (BOUNDED ONTOLOGY MEMORANDUM) → ITEM 29 Q6/Q4a DOCTRINE LOCKED (PATH C) → TIER A PERTURBATION DOCTRINE LOCKED + PREPARE-PHASE PAYLOAD READY (OFFLINE) → PRODUCTION CHARACTERIZATION (TIER A) EXECUTION NOT AUTHORIZED
```

The engine is at deterministic forensic governance baseline. Queue Item 14 (per-doctype memo program) is CLOSED. All seven governed doctypes are at V2_PASS gold-standard tier (with one extraction-completeness footnote — see §3 and residual #8). The governance decomposition is complete. The Item 28 Micro-Pilot characterization phase is COMPLETE per scoping memo v1.4 (15 May 2026). The Item 24 design phase is COMPLETE per the 16 May 2026 governance session: eight doctrinal artifacts and one observational artifact are locked. A bounded methodology-validation phase downstream of design closure — Item 24 Tier 0 — has completed (20 May 2026) on a non-production substrate; its findings characterize the methodology and that substrate, and do not transfer to the production engine without separate replication. The Item 29 design session (24 May 2026) opened and closed under the pre-opening charter, producing a non-canonical Bounded Ontology Memorandum; it touched no doctrine, schema, validator, or engine surface, and at the time it left Q6 and Q4a as decidable-but-not-yet-decided (see §4.3). This v1.7 update is the post-session state synchronization plus a strictly-mechanical housekeeping pass (residual #10 re-grade record, `extract_documents.py` docstring drift correction, two residual-registry additions). Item 24 production characterization (Tier A) is a separate operator-initiated gate downstream of Tier 0 closure and is not automatically licensed by it. Lock 4 discipline remained intact throughout the design sequence, throughout Tier 0 execution, throughout the Item 29 design session, and throughout this housekeeping pass. The v1.8 update records the Residual #12 closure: under an operator execution gate (25 May 2026, three-AI agreement), the seven `[ENTROPY: Item 28]` non-canonical keys in `CORPUS_INVENTORY` were reverted to their canonical originals via position-preserving in-place swap (Clean Restoration, Path 1). This is teardown of a temporary, ratified, revertible pilot deviation, not retroactive normalization; the `[ENTROPY]` framing record remains preserved in the `/docs/` scoping memo, the `extract_documents.py` header docstring, and the residual registry. Lock 4 held: no validator, schema, FO, or engine-logic change. The `discover_documents()` `[:72]` corpus-boundary slice was verified intact post-edit (dict remains 72 entries, key order preserved, boundary on `Strategic_Review_November_2024.pdf`). The v1.9 update records the positional-fragility resolution: under a narrow, operator-authorized Lock 4 exception scoped solely to corpus-boundary determination in `extract_documents.py`, `discover_documents()` was migrated off the `list(CORPUS_INVENTORY.keys())[:72]` positional slice to explicit corpus membership sets (`NORTHGATE_DOCUMENTS` / `QUORUM_DOCUMENTS`, the latter an explicit empty frozenset) read via an order-independent `corpus_for()` lookup, guarded by an import-time invariant (`_validate_corpus_membership()`) that enforces set disjointness, exact union with the inventory keys, and exactly-one-set membership per key. Approach B was chosen over a per-entry value reshape (Approach A) because a repo-wide grep found external scripts that read `CORPUS_INVENTORY` values as bare doctype strings; Approach B leaves those values unchanged and confines the edit to this file. This is the first exercised Lock 4 exception; it is narrow, recorded, and does not relax Lock 4 elsewhere (see §2). No schema, validator, prompt, FO, downstream, or external-script change. The v2.0 update records the Item 29 doctrine lock: the two decidable interpretation-boundary questions from the design session were adjudicated under an operator gate (three-AI audit) and locked as Item 29's first canonical doctrine in `/governance/doctrine/item_29_completeness_ontology.md` (v1.0). Q6 (flag singularity-vs-fracture) was decided as Path C — singularity-primary with bounded enumeration, unit = the missing document, no engine-inferred fracture. Q4a (intent detection-vs-meaning-side) was decided as Path C — detection intent-blind, with an intent marker recorded only where the ingested text explicitly declares it and never inferred. Both rulings sit inside the settled observed-absence-only boundary (inferred-absence forbidden) and do not reopen it. Q1, Q2, Q3, Q4b, and Q5 remain deferred to Tier A. Lock 4 holds: this is doctrine, not execution authorization; operationalizing either ruling in the engine is a separate downstream operator gate (see §4.3). The v2.1 update is operational bookkeeping recording two same-day Tier A events of 27 May 2026, neither of which authorizes Tier A execution. First, the Tier A perturbation specification was locked as doctrine (`/governance/doctrine/tier_a_perturbation_spec.md` v1.0) via a signed adjudication memo: filename-only perturbation across BASE plus the twelve admissible buckets, `{document_content}` byte-identical to BASE, one deterministic variant per bucket per representative document, single-bucket only, D2 excluded, with eight signed operator rulings recorded. Second, the narrow prepare-phase code gate contemplated in that doctrine's §8 / ruling 8 was opened and closed: `scripts/run_tier_a_batch.py` was extended from BASE-only (21 requests) to BASE + 12 filename buckets (273 offline request-definitions), prepare-phase only, with `--submit`/`--retrieve` dormant and no schema/validator/FO/prompt/engine change. The perturbation acts only on the `{document_id}` presented to the prompt; text is resolved against the canonical BASE document and content is unchanged. No batch has been submitted and Tier A execution remains a separate, unopened operator gate downstream of production-substrate API budget and the replication requirement. The v2.2 update records the ratification of the positioning doctrine (`/governance/doctrine/positioning_doctrine.md` v1.0 LOCKED), a presentation-layer doctrine governing how the product is positioned and how demonstration material is presented. It is orthogonal to the engine characterization pipeline recorded above: it touches no engine, schema, validator, or FO surface, is not a Lock 4 matter, and changes no posture on Tier A or any engine gate. It defers to `REACTIVE_CORE.md` §12 and `item_24_heterogeneity_taxonomy.md` on what counts as realistic institutional conditions, and governs presentation only, not corpus composition. This entry records its existence and active status; the doctrine's substance lives in the artifact. The v2.3 update is a documentation-versus-repository reconciliation of this file's artifact registers: two locked doctrine-layer artifacts already present on disk, `substrate_identity_discipline.md` (cross-Item methodological doctrine) and `tier_a_adjudication_memo.md` (the signed decision memo behind the Tier A perturbation rulings), are now listed in the companion-files block and the §8 repository tree, which previously omitted them. It records existing artifacts and introduces no doctrine, engine, schema, validator, or FO change; it is not a Lock 4 surface. The v2.4 update is recorded on the presentation-layer track, orthogonal to the engine-governance posture in this section: Presentation-layer and Tier 2 document hygiene is complete for the corpus as it stands locally; the remaining path to public launch is engine work downstream of the Lock 4 gate. The v2.5 update is recorded on the engine-validation track: Test #3 (re-derivation of the three NorthGate/Quorum demo findings against the cleaned corpus) is closed; all three findings now run successfully against fresh extractions; one forensic object (FO-NTH-001) required a rewrite after its rent-roll-reading logic was found to have been authored against a fictional schema that never matched any real extraction; demo-facing figures and wording for these three findings are locked separately in `/governance/sync/TEST_3_REFERENCE_LOCK.md`. This is not a Lock 4 surface in itself (the FO rewrite is application of existing doctrine to a defect, not a new architectural commitment), but the underlying defect and its detection are recorded as a dated reinforcement of residual #11 (see §7).

---

## 2. Active Locks

- **Lock 2 — Bounded scope on DTD labels.** DTDs carry bounded scope labels (e.g., "numeric normalization inconsistency"), not inflated semantic-governance framings. Held.
- **Lock 3 — Semantic-axis observation.** Semantic correctness is an independent validation axis from structural correctness. Recorded as observation; not yet doctrine. System-wide scope, distribution, recurrence rate, and architectural implications remain unestablished. No commitment to "unit-consistency doctrine" / "financial type system" / "ontology-aware normalization" until cross-doctype evidence establishes scope.
- **Lock 4 — Defer architectural commitments.** No engine-architecture changes proposed. No new validator patterns. No schema redesigns. No FO additions. Held across the Canonical Freeze, through the governance decomposition, through Item 28 closure, through Item 24 design closure, and through Item 24 Tier 0 execution. Lock 4 is a standing operational posture; Item 24's falsification logic artifact operationalizes and reaffirms it within Item 24's bounded scope but does not strengthen, extend, or modify Lock 4's standing authority. Neither Item 24 design closure nor Tier 0 closure authorizes remediation. The Tier 0 closure memo's §5.4 production recommendations are recorded recommendations, not authorized changes, and do not enter operational queue posture (see §5 and §6). **First exercised exception (25 May 2026):** a narrow, operator-authorized exception was opened and exercised, scoped solely to corpus-boundary determination in `discover_documents()` (the positional-fragility resolution — see §1, §6, §7). The exception was bounded to that single engine-logic surface in `extract_documents.py`; it authorized no schema, validator, prompt, FO, downstream-logic, or broader-architecture change, and it does not relax Lock 4 anywhere else. Lock 4 otherwise remains intact and continues to govern all engine/validator/schema/FO surfaces; any further change to those surfaces requires its own separate operator gate.
- **Lock 5 — Audit-before-prophylaxis.** Cross-prompt audit (LOCK5_AUDIT_MEMO.md) closed; promoted observations remain observations. Prophylactic regeneration of unaffected prompts deferred.

---

## 3. Gold-Standard Tier — n=7 Doctypes Complete

All seven governed doctypes have been cleared at V2_PASS, 0 errors, against fresh extractions in `outputs/extracted_documents/`:

| # | Doctype | Cleared | Per-doctype memo classification |
|---|---|---|---|
| 1 | `valuation_report` | 6 May 2026 | Pre-W1.1 chain (reference implementation) |
| 2 | `intercreditor_agreement` | 6 May 2026 | TRANSITION (no memo) ⚠️ |
| 3 | `guarantee_deed` | 6 May 2026 | TRANSITION (no memo) |
| 4 | `investment_model` | 7 May 2026 | TRANSITION |
| 5 | `board_minutes` | 13 May 2026 | TRANSITION |
| 6 | `loan_agreement` | 13 May 2026 | REMEDIATION (bundled R1+R2 → R1' → R2', 9 findings / 14 edits) |
| 7 | `financial_statements` | 13 May 2026 | REMEDIATION (single pass, 4 findings / 5 edits, cross-scope V2_PASS on n=3) |

⚠️ **Row 2 footnote:** The 6 May 2026 V2_PASS baseline for `intercreditor_agreement` is preserved as gold-standard. However, the Item 28 Step 7.1 comparative diff (14 May 2026) surfaced that this baseline extracted only 2 of 7 payment_priorities array members supported by the source text. V2_PASS holds (array completeness is not a schema-required property). Recorded as residual registry entry #8 (Registry-filename-baseline extraction-completeness observation). **Gold-standard does not imply extraction-exhaustive on non-required schema surfaces.** Whether the other six gold-standard baselines carry analogous incompleteness gaps is the central question for Item 29 reconsideration post Step 7.5.

**Status interpretation:** the W1.1 chain is end-to-end coherent across the full governed schema family. The Bundled-Remediation Methodology is empirically validated on n=2 doctypes (loan_agreement + financial_statements). Per-doctype work for the seven governed doctypes is complete. No further per-doctype memos scheduled.

---

## 4. Item 28 — Filename-Feature Variation Pilot (CLOSED — Characterization Complete)

**Status:** **CLOSED — H₀ FALSIFIED, characterization complete, Step 7.5 promotion decision recorded.** Item 28's full sequence (pilot execution → counterfactual → Step 7.1 diff → Step 7.2 isolation → Step 7.5 promotion decision) is complete. The empirically-anchored finding: filename-feature variation causally modulates clause selection on at least one schema field; modulation is deterministic, validator-silent, and constitutionally consequential. Mechanism narrowed to separator-feature interaction; generalization scope unbounded and now becomes Item 24's domain.

**Authoritative artifacts:**
- Scoping memo v1.4: `/docs/item_28_scoping_memo.md` (§§14-15 record Step 7.2 results and Step 7.5 promotion decision)
- Pre-registration: file no longer present on disk; operational content preserved by inline reference within scoping memo §§1, 9, 13 (residual #9)

The scoping memo is doctrinally upstream of Item 24's pre-registration: §9's symmetric stochasticity-exception requirement, §14.5.1's three validator-surface gaps, and §15.7's forward-looking generalization conditional are recorded inputs to the Item 24 design. The scoping memo's location at `/docs/` rather than `/governance/` is intentional (see §9 Repository Topology and Framing-Provenance Policy).

---

## 4.1 Item 24 — Realistic Heterogeneity Characterization (DESIGN CLOSED, EXECUTION DEFERRED)

**Status:** **DESIGN PHASE CLOSED — PRE-REGISTRATION LOCKED — EXECUTION NOT AUTHORIZED.**

The seven-step dependency chain executed and locked across the 16 May 2026 governance session:

1. Ontological definition
2. Admissibility doctrine
3. Heterogeneity taxonomy
4. Corpus strategy
5. Execution model
6. Falsification logic
7. Pre-registration synthesis

**Locked artifact inventory (canonical paths):**
- `/governance/doctrine/item_24_ontological_definition.md` (v1.0)
- `/governance/doctrine/item_24_admissibility_doctrine.md` (v1.1)
- `/governance/doctrine/item_24_heterogeneity_taxonomy.md` (v1.0)
- `/governance/doctrine/item_24_corpus_strategy.md` (v1.0)
- `/governance/doctrine/item_24_execution_model.md` (v1.0)
- `/governance/doctrine/item_24_falsification_logic.md` (v1.0)
- `/governance/preregistration/item_24_preregistration.md` (v1.0 — master synthesis)
- `/governance/observations/item_24_governance_observation_001.md` (v1.1 OBSERVATIONAL)

**Core doctrinal outcomes (posture-level summary; doctrine files remain authoritative):**

- Item 24 is a bounded characterization study with forward-compatibility constraints, without longitudinal commitment.
- Realistic institutional heterogeneity is governed by the Mechanism Plausibility Test: an articulable institutional workflow mechanism must plausibly generate any admissible heterogeneity class. Origin-independent: synthetic instantiation of a real institutional mechanism is admissible; real instances of non-institutional mechanisms are not.
- Twelve heterogeneity buckets admitted (A, B, C, D1, E, F, G, H, I, J, K, L); one excluded (D2 — corruption/noise injection failed the mechanism plausibility test).
- Three measurement surfaces: semantic completeness stability, extraction-path consistency, omission modulation.
- Execution policy: strict Temperature 0 (stochasticity-suppression policy, not determinism guarantee).
- Falsification policy: N=3 reproducibility protocol with per-surface identity criteria and a 2/3 disclosure protocol (3/3 = Formal Finding, 2/3 = Near-Reproducibility Observation, 1/3 = Dismissed, 0/3 = N/A).
- Three-tier descriptive severity hierarchy (Observational Finding / Localized Vulnerability / Critical Defect) with Authorization Firewall: a DTD is documentation, not authorization.
- Anti-Panic Protocol: at any finding severity within Item 24 execution, AI-generated remediation outputs are explicitly invalidated and must be rejected; terminal output is a Diagnosis Memo only.

**Execution firewall:** Item 24 design closure does not authorize Item 24 execution, remediation work, validator redesign, architecture changes, or production hardening. Execution authorization is an operator-initiated governance event downstream of design closure.

---

## 4.2 Item 24 Tier 0 — Methodology Validation (CLOSED — Non-Production Substrate)

**Status:** **CLOSED — METHODOLOGY OPERATIONALLY VALIDATED ON A NON-PRODUCTION SUBSTRATE — PRODUCTION CHARACTERIZATION (TIER A) NOT AUTHORIZED.**

Tier 0 is a bounded methodology-validation sub-phase of Item 24, downstream of design closure. It is **not** the commencement of Item 24 execution in the production sense, and it is **not** production-engine characterization. The distinction is load-bearing: methodology validation, production characterization, and operational execution must not become historically conflated. Tier 0 produced execution-phase governance observations while preserving the pre-registered authorization boundaries.

**Authoritative artifact:** `/governance/results/item_24_tier_0_methodology_validation_results_memo.md` (v1.0 LOCKED, 20 May 2026). This is the first artifact in the new `/governance/results/` execution-result category (see §8).

**Substrate boundary (non-negotiable):** All Tier 0 runs were produced on the Claude.ai web (Incognito) serving surface at non-zero, non-operator-controllable temperature, against an Anthropic frontier model identified to the operator as Claude Opus 4.7. This is a non-production substrate. The production extraction engine is `claude-sonnet-4-20250514` via the Anthropic API at strict Temperature 0. Tier 0 findings characterize the methodology and the non-production substrate only. **Nothing transfers to the production engine without separate replication on the production substrate.**

**Scope of what was validated:** perturbation construction operability, canary measurement at the extraction layer, the N=3 reproducibility protocol, the manual Incognito execution workflow, the auto-grader instrument, and the session-bootstrap mechanism. Tier 0 did NOT characterize production-engine behavior, test forensic-object firing, or measure computed downstream values.

**Execution summary:** 60 runs (12 BASE + 48 perturbation across buckets A, F, K, L), 4 Paris-Hotel documents (INV, OPS, EXIT, TERM), N=3 per cell, each in a fresh Incognito session with deterministic grading via `scripts/grade_tier_0.py`. Phase 1 BASE gate PASSED (all four canaries 3/3 at canonical filename).

**Canary stability:** 18 of 20 cells stable at 3/3. Two non-3/3 cells, both attributed and neither a substrate extraction failure:
- **INV × L = 0/3** — grader canonicalization gap, not extraction failure. Under bucket L the substrate output rate fields as annotated strings (e.g., `"3.3% p.a."`) rather than decimals; extractions were correct and correctly cited, but `normalize_to_decimal()` does not strip the `" p.a."` suffix. Extraction correctness and canonicalization stability are distinct properties; the substrate held the former and varied the latter on this bucket.
- **OPS × F = 2/3** — infrastructure truncation (Chrome WebSocket disconnection mid-generation), not a substrate or perturbation result. Per Anti-Panic Protocol the run was not repeated; the truncated artifact is preserved.

**Closure findings (posture-level; closure memo remains authoritative):**
- Baseline plus three of four perturbation buckets were canary-stable on the tracked canaries.
- One reproducible substrate formatting shift (bucket L rate-field annotation) — extraction-correct, canonicalization-divergent.
- One bucket L provenance-surfacing behavior, read as prompt-conditioned commentary from the Bootstrap priming, NOT autonomous agency or execution-halting intent.
- The most consequential finding was a process finding (memo §5.3.2): see residual #11.
- Three production recommendations (memo §5.4) recorded for Tier A design. **Recorded, not authorized.** They do NOT enter operational queue posture (Lock 4 discipline; see §6).

**Tier 0 closure firewall:** Tier 0 closure does not authorize Tier A, remediation, validator redesign, schema change, FO change, or production hardening. The grader canonicalization fix and the §5.4 production recommendations are recorded recommendations, not authorized changes. Production characterization (Tier A) remains a separate operator-initiated gate, downstream of production-substrate API budget.

---

## 4.3 Item 29 — Completeness Ontology (DESIGN SESSION CLOSED — Q6/Q4a DOCTRINE LOCKED)

**Status:** **DESIGN SESSION CLOSED — Q6 AND Q4a ADJUDICATED AND LOCKED (PATH C) — Q1/Q2/Q3/Q4b/Q5 DEFERRED TO TIER A — NO ENGINE OPERATIONALIZATION AUTHORIZED.**

Item 29 concerns completeness ontology: what level and category of documentary visibility is sufficient for valid structural testing within declared posture. A pre-opening session (24 May 2026) built the perimeter; the design session proper (24 May 2026) was opened by separate operator initiation and is now closed. Both sessions were governance-only and design-boundary-only under Lock 4. The operative firewall throughout: **finding a gap is not authorization to close it.**

**Carried-in settled boundary (Move 2, operator-adjudicated, not reopened):** The engine reasons only over the ingested corpus. It may flag a missing dependency only when that dependency is explicitly referenced in ingested text (observed-absence); it may not infer the existence of latent, unknown, or unreferenced external documents (inferred-absence forbidden). This was an operator modification of the working-group recommendation, not an acceptance of it.

**Design-session results (24 May 2026 — preserved as the historical record of the session that produced the rulings; the Q6/Q4a outcomes below in "Doctrine locked" supersede the decidable-not-decided status these results carried at the time):**
- **Zone 1 (detection criterion) characterized:** "explicitly referenced" is a multi-property question, not a threshold on a single axis. At least four candidate dimensions were surfaced — referent individuation, corpus-relative resolvability, source-conditioning, reference-intent — left explicitly UNRANKED, NON-EXHAUSTIVE, and with interactions UNRESOLVED. Decomposition was deliberately halted before it became an admissibility model.
- **Zone 2/6 (interpretation boundaries) enumerated and sorted:** six interpretation-boundary questions (Q1–Q6) were enumerated and each marked decidable-in-Item-29 or deferred-to-Tier-A. Decidable-in-Item-29: Q6 (flag singularity-vs-fracture) and Q4a (intent as detection-side vs meaning-side). Deferred-to-Tier-A: Q1, Q2, Q3, Q4b, Q5. Q2 was re-sorted from decidable to deferred by operator audit (the character/meaning line does not hold under pressure); Q5 (source-conditioning on the meaning side) flagged as the drift-magnet. (At the close of the design session none of the six was yet answered; Q6 and Q4a were subsequently adjudicated — see "Doctrine locked" below.)

**Doctrine locked (25 May 2026 — operator adjudication under gate, three-AI audit):** Q6 and Q4a were adjudicated and locked as Item 29's first canonical doctrine in `/governance/doctrine/item_29_completeness_ontology.md` (v1.0 LOCKED).
- **Q6 (flag singularity-vs-fracture) → Path C (singularity-primary with bounded enumeration).** The unit of the flag is the missing document (one flag per missing document, regardless of how many in-corpus sources reference it). The flag body carries a bounded enumeration of the specific observed in-corpus references pointing to it. Hard constraint: no engine-inferred fracture — the engine lists observed references only, never reconstructed fields or inferred consequences.
- **Q4a (intent detection-vs-meaning-side) → Path C (detection intent-blind; intent recorded as a non-gating annotation).** Detection is mechanical and intent-blind: every observed-referenced absence is flagged. An intent marker may be attached only where the ingested text explicitly declares it (e.g., "incorporated by reference"); it never gates the flag. Hard constraint: no inferred authorial purpose — intent not explicitly stated in the text is not recorded.
- Both rulings sit on the same side of a single line — observed structure may be captured and enumerated; unobserved content or purpose may not be reconstructed or adjudicated — and both operate strictly inside the §4.3 settled boundary (observed-absence only; inferred-absence forbidden), which they do not reopen.

**Decided ≠ authorized for execution.** Q6 and Q4a are now decided doctrine. This decides the doctrinal answers only; it authorizes no engine, schema, validator, or FO change. Operationalizing either ruling is a separate operator-initiated gate, downstream of and distinct from this doctrinal lock. **Q1, Q2, Q3, Q4b, and Q5 remain deferred to Tier A** — undecided, unscheduled, and unconstrained by this lock beyond the settled boundary. The non-gating intent marker recorded under Q4a is held for Q5's future use and does not anticipate or decide it.

**Authoritative artifacts:**
- `/governance/doctrine/item_29_completeness_ontology.md` (v1.0 LOCKED) — the canonical statement of the Q6 and Q4a rulings.
- `/governance/sync/ITEM_29_BOUNDED_ONTOLOGY_MEMORANDUM.md` (non-canonical, ratified Claude → Gemini, ChatGPT out of credits) — the historical record of the design session that produced the questions. It does not amend REACTIVE_CORE.md or CURRENT_STATE.md; this §4.3 is the operational-state reflection of the session and its doctrine lock.

**Item 29 execution firewall (reaffirmed):** The locked Q6/Q4a doctrine authorizes no admissibility rule beyond its own scope, no detection-criterion implementation, no completeness threshold, no source-class disposition, no Tier A decision, and no schema/validator/engine/FO change. It is doctrine, not execution authorization. Everything not covered by the Q6/Q4a rulings — including Q1, Q2, Q3, Q4b, Q5 — remains undecided and deferred to Tier A. Lock 4 holds: operationalizing the locked doctrine in the engine is a separate operator-initiated gate.

---

## 5. Explicit Non-Authorizations

The following are explicitly NOT authorized by the current posture:

- Item 24 production characterization (Tier A). Neither design closure nor Tier 0 closure authorizes it. (Note: the Tier A perturbation doctrine is now locked and the narrow prepare-phase code gate has been exercised — `scripts/run_tier_a_batch.py` can emit 273 offline request-definitions — but neither the doctrine lock nor the prepare-phase payload authorizes Tier A *execution*. Execution remains unauthorized and is a separate gate downstream of production-substrate API budget and the replication requirement.)
- Activation of `--submit` or `--retrieve` in `scripts/run_tier_a_batch.py`. The prepare-phase code gate (exercised 27 May 2026) extended preparation only; the submission and retrieval placeholders remain dormant and their activation is a separate, unopened operator gate. No batch has been submitted.
- Item 24 execution beyond the closed Tier 0 methodology-validation sub-phase.
- Engine-architecture changes, validator redesigns, schema redesigns, FO additions, or production hardening at any severity level of any current or future finding. (The sole exception to date is the narrow, operator-authorized corpus-boundary change of 25 May 2026, recorded in §2 and bounded to `discover_documents()`; it does not license any further engine/validator/schema/FO change.)
- Implementation of the Tier 0 closure memo §5.4 production recommendations (provenance-flag schema field, schema-enforced canonicalization, Bootstrap-priming tuning). These are recorded recommendations for Tier A design only, not authorized work, and are intentionally NOT carried into the active queue.
- Promotion of any current observation (Lock 3 semantic-axis, residual #7 DTD-008 retention, residual #8 extraction-completeness, residual #11 evidence-hierarchy, GO-001) to doctrine without satisfying the established promotion criteria (determinism/generalization established, engine-layer remediation surface identified, closure criteria definable in advance).
- AI-generated remediation proposals during Item 24 execution. These are explicitly invalidated by the locked falsification logic and must be rejected. Diagnosis memos are the only authorized output. (Lock 4 covers all other execution phases as a standing operational posture.)
- Retroactive editing of artifacts produced under superseded framing (notably the Item 28 pre-registration content preserved inline in the scoping memo, and the scoping memo §§1-12 historical wording). Framing-provenance integrity is preserved per §9 policy.
- Engine operationalization of the locked Item 29 Q6/Q4a doctrine, and any admissibility rule, detection criterion, completeness threshold, source-class disposition, or further interpretation-boundary doctrine beyond the Q6/Q4a rulings. Q6 and Q4a are now decided doctrine (Path C, locked in `item_29_completeness_ontology.md`), but that is doctrine, not execution authorization: implementing either ruling in the engine is a separate operator gate. Q1, Q2, Q3, Q4b, and Q5 remain undecided and deferred to Tier A (see §4.3).
- (CLOSED 25 May 2026) The Item 28 entropy-filename rollback (residual #12) was executed under operator execution gate (three-AI agreement) via position-preserving Clean Restoration. No longer an open non-authorization.
- Any code change to `extract_documents.py` beyond (a) the 24 May docstring-only correction, (b) the 25 May Residual #12 rollback (seven `CORPUS_INVENTORY` key swaps under operator gate), and (c) the 25 May positional-fragility resolution (corpus-boundary determination migrated to explicit membership sets plus an import-time invariant, under the narrow Lock 4 exception in §2). The `CORPUS_INVENTORY` dict keys, key order, and all 72 bare-string doctype values remain byte-identical to v1.8; the authorized change (c) is confined to corpus-boundary logic. No schema, validator, prompt, FO, downstream-logic, or external-script change is authorized; any such change requires its own separate operator gate.

---

## 6. Active Queue

**Immediate:**
- **CURRENT_STATE.md v2.5 update — Test #3 closure (THIS UPDATE).** Re-derivation of FO-NTH-001, FO-NTH-002, and FO-QRM-020 against the cleaned NorthGate/Quorum corpus is complete. FO-NTH-002 and FO-QRM-020 confirmed stable on re-run (FO-QRM-020 byte-stable across two independent runs); no rewrite required beyond a prior MODEL_PATH filename correction. FO-NTH-001 required a genuine rewrite: its rent-roll-reading block (`break_option_summary_2027`, `portfolio_summary.gross_passing_rent_gbp`, `as_of_date`) referenced fields that do not exist in any version of the rent-roll extraction schema; the block was rewritten to compute the same aggregates directly from the real `tenancies` array. Session-record: a new doctype, `rent_roll` (`rent_roll_schema.json` v1.0, `rent_roll_prompt.txt` v2), was designed, cross-reviewed, and registered in `DOCUMENT_TYPE_MAP`; `NorthGate_Tenant_Schedule_Rent_Roll_Dec2024.xlsx` was reclassified from `metadata_only` (never extracted) to `rent_roll` and successfully extracted (38 tenancy rows, including correct break-option parsing for two vacant rows after a one-line prompt fix). Also fixed in-session, mechanical and non-doctrinal: a retired model string (`claude-sonnet-4-20250514` → `claude-sonnet-4-6`, per Anthropic's 15 June 2026 deprecation) and an undersized `MAX_TOKENS` ceiling (8000 → 16000) that was silently truncating long-form extractions. Authoritative demo-facing figures, sourcing constraints, and explicit supersession of the prior invalid FO-NTH-001 figure are recorded in `/governance/sync/TEST_3_REFERENCE_LOCK.md` (non-canonical, display-authoritative for these three findings only — this file does not duplicate those figures). Governance lesson recorded as a dated reinforcement of residual #11 in §7, not as a new residual.
- **CURRENT_STATE.md v2.4 update — demo-track document hygiene.** Metadata scrub complete across both local rooms, session-verified; NorthGate model workbook provenance stripped and four-layer reconciliation confirmed; next concrete action remains the Lock 4 gate on the three extraction-shape fixes. Session-record entry: Corpus metadata scrub, 13 June 2026 (session-verified; presentation and Tier 2 hygiene; touches no lock). Scope: four high-signal metadata fields, author, creator, title, and creation date, across the PDF sets present in the two local datarooms on 13 June 2026; 76 Quorum PDFs and 63 NorthGate PDFs reviewed, each checked by read-back rather than assumption. Findings: no fund-manager, client, or project-codename residue found in either room within that review scope. Actions: three synthetic authored files carrying operator initials were normalized to ReActive, Quorum 09 `Independent_Tax_Opinion_Luxembourg_2024.pdf`, Quorum 09 `Anti_Financial_Crime_Report_2024.pdf`, and NorthGate 02 `NorthGate_Financial_Model_Equity_Outputs_BaseCase_Dec2024.pdf`, each read-back-verified after change. Preserved by intent: Word-export `Microsoft Word - ...` titles, and all third-party reports including the Cushman & Wakefield placeholder title, since third-party files are governed by the external-link posture and are not re-hosted on the public surface. Separately in the same session: the NorthGate model workbook had package-level external-link provenance removed (four original source paths), hidden-sheet and comment residue cleared, canonical filename applied, and reconciliation verified in-session across four layers (registry key already canonical, old physical xlsx deleted, stale text extract removed, extraction cache confirmed absent), operator-confirmed in session. Not done, available, and not on the critical path: deep package-level scan across the full served corpus, and post-migration re-verification after Quorum is migrated to Replit. Presentation and Tier 2 hygiene only; touches no lock and is not a Lock 4 surface.
- **CURRENT_STATE.md v2.3 update** (A documentation-versus-repository register reconciliation. Two locked doctrine-layer artifacts already present on disk, `substrate_identity_discipline.md` (v1.0 LOCKED, cross-Item methodological doctrine) and `tier_a_adjudication_memo.md` (signed decision memo, 27 May 2026, the basis for the Tier A perturbation rulings), were absent from this file's registers and are now recorded. Updates: version header to v2.3, one dated-events milestone line, two Companion-files entries, two doctrine lines in the §8 repository tree, a v2.3 posture sentence appended in §1, one accuracy sentence appended to the §8 topology note, and this queue entry. Records existing artifacts only; no doctrine, engine, schema, validator, FO, prompt, or code change; not a Lock 4 surface. The prior v2.2 positioning entry and v2.1 Tier A bookkeeping are unchanged. Note for a later pass: `tier_a_adjudication_memo.md` resides in `/governance/doctrine/` although it is a signed decision memo rather than executable doctrine; its placement is recorded as-is here and not changed.)

**Deferred — operator-initiated gates:**
- **Tier A submission gate (NEW — deferred).** The prepare-phase payload now exists (`scripts/run_tier_a_batch.py` emits 273 offline request-definitions on `--prepare`). Submitting it to the Anthropic Batch API is a separate, unopened operator gate: it requires activating the dormant `--submit` placeholder, which is itself not authorized, and it constitutes Tier A execution on the production substrate (temperature 0), downstream of API budget and the standing replication requirement (Tier 0 findings do not transfer without re-running on the production substrate). Not opened.
- **Item 24 production characterization (Tier A) authorization.** Status: DEFERRED PENDING OPERATOR AUTHORIZATION. Tier 0 methodology validation closed; Tier A remains gated and is downstream of production-substrate API budget. Tier A design carries forward the §5.4 recommendations recorded in the closure memo (not as authorized changes, but as design inputs to be evaluated when Tier A is authorized).
- **Item 24 execution authorization (broader).** Status: DEFERRED PENDING OPERATOR AUTHORIZATION. Design phase closed, pre-registration ratified; execution beyond Tier 0 remains gated.

**Deferred — non-blocking:**
- **Grader canonicalization enhancement — RESOLVED (24 May 2026).** `scripts/grade_tier_0.py` `normalize_to_decimal()` annotation-stripping (`_TRAILING_ANNOTATIONS`: strips `p.a.` / `per annum` / `per year` / `annual*`, deliberately excludes magnitude-changing `bps`) was confirmed present in the file. INV × L re-graded via `--dry-run --verbose`: 3/3 ✓ (B2, all four sub-values correct and cited, all three runs). Residual #10 closed (see §7). This was a recorded re-grade operation against a measurement instrument, not production remediation and not a validator/engine change. The code fix had been applied in a prior session; v1.6 listing it as deferred was stale (documentation-vs-repository drift, now corrected). TRACKER.md left frozen as the historical execution artifact per operator ruling; the correction lives in the registry only.
- **Item 28 Step 7.2 filename-variant cleanup — DONE (already applied).** The four Step 7.2 variant entries were removed from `CORPUS_INVENTORY` in a prior session; the dict is at 72 entries and carries no Step 7.2 variants. The `extract_documents.py` header docstring described the side-by-side staging as if still live; corrected this session by a docstring-only edit (closure note appended, staging narrative preserved as historical record, no code-body change — dict and all functions byte-identical). Documentation-vs-repository drift, now corrected.
- **Item 28 entropy-filename rollback — DONE (25 May 2026, operator execution gate, three-AI agreement).** The seven `[ENTROPY: Item 28]` keys in `CORPUS_INVENTORY` were reverted to canonical originals via position-preserving in-place line swaps (Clean Restoration, Path 1). Canonical strings copied verbatim from the `extract_documents.py` docstring. Post-edit AST verification: dict at 72 entries, key order preserved, `[:72]` boundary intact on `Strategic_Review_November_2024.pdf`, doctype multiset unchanged, file compiles. Framing record preserved in `/docs/` scoping memo, docstring staging narrative, and residual registry. Residual #12 closed (see §7). Re-extraction under canonical filenames is a separate operator action, not performed by this edit.
- **Positional-fragility resolution in `extract_documents.py` — RESOLVED (25 May 2026, narrow Lock 4 exception, operator-authorized).** `discover_documents()` previously tagged Northgate vs Quorum via `list(CORPUS_INVENTORY.keys())[:72]`, a positional slice that silently mis-tagged the corpus boundary on any non-position-preserving dict edit. The slice is removed. Corpus membership is now declared explicitly via `NORTHGATE_DOCUMENTS` and `QUORUM_DOCUMENTS` (the latter an explicit empty frozenset, repository being Northgate-only) adjacent to the inventory, and `discover_documents()` reads corpus via an order-independent `corpus_for()` lookup. An import-time invariant (`_validate_corpus_membership()`) fails loudly unless the two sets are disjoint, their union exactly equals `CORPUS_INVENTORY` keys, and every key belongs to exactly one set. Approach B (membership sets, values left as bare strings) was chosen over Approach A (per-entry value reshape) because a repo-wide grep found external scripts reading the doctype values as strings; reshaping would have widened the exception beyond this file. Verified: compile pass; AST-confirmed no positional slice remains in executable code; inventory byte-identical (72 entries, same keys/order/values as v1.8); import-time invariant pass with a negative test confirming it catches a broken set; order-permutation invariance pass; old-vs-new boundary equivalence pass; external-importer compatibility pass (values still bare strings). Scope: corpus-boundary determination in `extract_documents.py` only; no schema, validator, prompt, FO, downstream, or external-script change. Standing caveat: a repo-wide grep for any *external* script that reconstructs the corpus split positionally is recommended on the operator side, as that surface is outside this file's view.
- Item 28 pre-registration file recovery: NOT PROPOSED. The file is no longer present on disk; operational content is preserved by inline reference within the scoping memo. Reconstruction would require retroactive framing reconstruction which the pre-registration discipline explicitly disallows. Recorded as residual #9.

**Explicitly NOT queued:** The Tier 0 closure memo §5.4 production recommendations (provenance flags, schema-enforced canonicalization, Bootstrap-priming tuning). Tier 0 produced production-design observations recorded in the closure memo; no implementation work is authorized or queued. They are surfaced here only as an acknowledgment that the closure memo records them, not as pending implementation candidates.

---

## 7. Residual Registry

Eight prior entries unchanged from v1.4 (entries #1–#8). Entry #9 unchanged from v1.5. Entries #10 and #11 added in v1.6. Entry #10 is CLOSED in v1.7 (re-grade complete). Entry #12 added in v1.7, CLOSED in v1.8 (rollback executed). The positional-fragility observation — tracked in §6 as a non-numbered queue observation, not as a numbered registry entry — is RESOLVED in v1.9 under the narrow Lock 4 exception (see §6 and the v1.9 note appended to #12 below). Net open numbered registry entries after this update: #1–#9, #11 (entries #10 and #12 closed).

**#9 — Item 28 pre-registration file absence (added 17 May 2026).** The file `/docs/item_28_micro_pilot_preregistration.md`, referenced in the scoping memo at lines 6, 19, and elsewhere, is no longer present on disk. The file was operationally consequential during Item 28 design and pilot execution (the §11 Decision Tree of the pre-registration is what authorized the scoping-memo branch). Its operational content is preserved by inline reference within the scoping memo §§1, 9, 13. Reconstruction is not proposed: the pre-registration discipline (scoping memo §§343, 392) explicitly disallows retroactive editing of artifacts produced under superseded framing, and reconstruction would create the appearance of a post-correction artifact under pre-correction discipline. Recorded as documented historical fact, not integrity defect. No remediation action required.

**#10 — Tier 0 INV × L canonicalization-gap-over-correct-extraction (added 21 May 2026; CLOSED 24 May 2026).** The Tier 0 INV × L cell scored 0/3 because the grader's `normalize_to_decimal()` did not strip the `" p.a."` annotation the substrate attached to rate fields under bucket L. The underlying extractions were correct and correctly cited. **Closure (24 May 2026):** the annotation-stripping fix was confirmed present in `scripts/grade_tier_0.py` (`_TRAILING_ANNOTATIONS`), and a recorded re-grade of INV × L via `--dry-run --verbose` returned 3/3 ✓ (B2, all sub-values correct and cited, all three runs). The canonicalization gap is closed; extraction correctness was never in question and is unchanged. Bounded to the non-production substrate and the grader instrument. TRACKER.md left frozen as historical execution artifact; correction recorded here only. No promotion (never met promotion criteria; closed by resolution, not by promotion).

**#11 — Tier 0 evidence-hierarchy observation (added 21 May 2026).** **OBSERVATIONAL — non-doctrinal, non-constitutional, not yet generalized beyond current evidence.** During Tier 0 characterization review, deterministic grading plus preserved raw artifacts provided more reliable truth-maintenance than AI-generated narrative synthesis: the Batch 4 (bucket L) AI-generated summary diverged materially from the underlying JSONs and grader output, and direct inspection of preserved artifacts plus deterministic re-grading was the corrective. Stated narrowly and on the record: *during this characterization sequence, under these conditions, artifact-grounded verification outperformed narrative synthesis as a truth-maintenance mechanism.* This is NOT "AI summaries are unreliable," is NOT universalized, is NOT an anti-AI doctrine, and does NOT imply deterministic systems are inherently superior in all governance contexts. Unlike the §5.4 recommendations, this observation points at a governance practice (evidence hierarchy during characterization review), not at architecture, so it carries no Lock 4 implementation pressure. Recorded as a candidate operational governance observation pending broader replication and scope characterization. Does not meet promotion criteria.

**Dated note (19 June 2026) — second, independent occurrence on a different artifact type.** During Test #3 (NorthGate/Quorum demo-finding re-derivation), `fo_nth_001_exit_window.py` was found to have been authored against a fictional, pre-aggregated rent-roll schema (`break_option_summary_2027`, `portfolio_summary.gross_passing_rent_gbp`, `as_of_date`) that never matched any real version of the rent-roll extraction schema. The file had passed prior review cycles and was treated as operational. During same-session debugging, a second-opinion AI review characterized the file as ready to execute on two separate occasions, immediately preceding two distinct execution failures (a wrapper-unwrap error, then the fictional-field `KeyError`). Static review of the code text did not surface either defect; execution against real, current extraction output did, on the first actual run after a relevant schema came to exist. This extends the pattern recorded above from narrative summaries to executable forensic-object code — a different artifact type, independently arrived at, under different session conditions. Recorded as evidence toward the "broader replication" condition this entry's disposition already names as the open question; this does NOT itself constitute promotion, and the promotion criteria in this section's closing paragraph are unchanged. Operational implication recorded for awareness, not as a new lock: a forensic object's operational status should not be treated as settled on the basis of documentation or review alone; execution against current, real extraction output is the verification step neither authorship nor review substitutes for.

**#12 — Item 28 entropy-filename state still live in CORPUS_INVENTORY (added 24 May 2026).** `CORPUS_INVENTORY` in `extract_documents.py` still carries seven `[ENTROPY: Item 28]` non-canonical filenames, a temporary/ratified/revertible pilot deviation. Item 28 is closed, so the post-pilot rollback to canonical filenames is genuinely open work. It was deliberately NOT performed during the 24 May housekeeping session: the rollback touches the live-observation substrate that produced the Item 28 filename-feature finding, and changing the keys alters what `{document_id}` presents on any re-extraction. Reserved for a dedicated session under its own operator gate, with a framing-provenance decision (clean restoration vs. preserve-as-historical) to be made at that time. Canonical originals are listed in the `extract_documents.py` header docstring. Non-blocking; not an integrity defect (the deviation is documented and intentional). Does not meet promotion criteria (it is a cleanup item, not an observation pending promotion).

**Closure (25 May 2026):** Executed under operator execution gate with three-AI agreement. Path 1 (Clean Restoration) adjudicated: the seven non-canonical keys were reverted to canonical originals via position-preserving in-place line swaps (each key swapped on its own line; not a `pop()`/reassign and not a dict-comprehension rebuild, both of which carried reordering risk against the `discover_documents()` `[:72]` slice). Canonical strings taken verbatim from the `extract_documents.py` docstring. Post-edit verification (AST + compile + line diff): dict at 72 entries, key order preserved, all seven affected keys at positions 18–28 inside the slice, `[:72]` boundary intact on `Strategic_Review_November_2024.pdf`, doctype multiset unchanged, and only the seven keys plus two section comments plus one appended docstring patch changed. Adjudicated as teardown of a temporary/revertible pilot deviation, not retroactive normalization; the `[ENTROPY]` framing record remains preserved in the scoping memo, the docstring staging narrative, and this registry entry. Closed by resolution, not promotion. The positional-fragility observation remains open and unchanged — this edit navigated the `[:72]` slice safely but did not remove the fragility.

**v1.9 note (25 May 2026) — supersedes the final sentence above.** The preceding sentence was accurate when v1.8 was cut. As of v1.9 it is superseded: the positional-fragility observation is now RESOLVED under a separate, narrow Lock 4 exception (the `[:72]` slice was removed and corpus membership made explicit — see §6 "Positional-fragility resolution" and §2 Lock 4). The v1.8 sentence is preserved verbatim above per framing-provenance discipline (it records the v1.8 posture as it stood); this note records the subsequent change rather than rewriting the earlier record.

Promotion criteria for any observation to DTD or doctrine: (a) determinism / generalization established, (b) engine-layer remediation surface identified, (c) closure criteria definable in advance. Of the open registry entries, none currently meets all three. (Entry #10 was closed by resolution on 24 May 2026, not by promotion.)

---

## 8. Repository Architecture — Stabilized Doctrinal Hierarchy

The governance hierarchy is no longer merely in transition. Following the 16 May 2026 mid-session reorganization (which corrected the earlier `docs/` ↔ `governance/doctrine/` heuristic routing error for Item 24 artifacts), the repository now contains a stabilized doctrinal topology. The 21 May 2026 Tier 0 closure introduced one new category: `/governance/results/` for execution-result artifacts (see note below).

```
governance/
├── constitution/
│   └── REACTIVE_CORE.md                          (§12 anchors heterogeneity framing)
├── doctrine/
│   ├── item_24_admissibility_doctrine.md         (v1.1 LOCKED)
│   ├── item_24_corpus_strategy.md                (v1.0 LOCKED)
│   ├── item_24_execution_model.md                (v1.0 LOCKED)
│   ├── item_24_falsification_logic.md            (v1.0 LOCKED)
│   ├── item_24_heterogeneity_taxonomy.md         (v1.0 LOCKED)
│   ├── item_24_ontological_definition.md         (v1.0 LOCKED)
│   ├── item_29_completeness_ontology.md          (v1.0 LOCKED — Q6/Q4a rulings; first Item 29 doctrine)
│   ├── positioning_doctrine.md                   (v1.0 LOCKED, presentation/demo posture; not engine doctrine, not Lock 4)
│   ├── substrate_identity_discipline.md          (v1.0 LOCKED, cross-Item methodological doctrine; substrate-identity binding)
│   ├── tier_a_adjudication_memo.md               (signed decision memo, 27 May 2026; basis for the Tier A perturbation rulings)
│   └── tier_a_perturbation_spec.md               (v1.0 LOCKED — filename-only perturbation; BASE + 12 buckets)
├── observations/
│   └── item_24_governance_observation_001.md     (v1.1 OBSERVATIONAL)
├── preregistration/
│   └── item_24_preregistration.md                (v1.0 LOCKED — master synthesis)
├── results/
│   └── item_24_tier_0_methodology_validation_results_memo.md  (v1.0 LOCKED — first execution-result artifact)
├── state/
│   └── CURRENT_STATE.md                          (v2.2, this file)
├── archive/
│   └── CLAUDE_v1_FINAL.md                         (rollback anchor)
└── sync/                                          (non-canonical session continuity)

docs/
├── item_28_scoping_memo.md                       (v1.4 — historical framing preserved)
├── W1_1_*_memo.md                                (five per-doctype W1.1 memos)
├── W1_1_scoping_memo.md
├── e4_divergence_report.md
└── orco_test.md

scripts/
└── run_tier_a_batch.py                           (Tier A orchestration; prepare-phase only, BASE + 12 buckets = 273 offline requests; --submit/--retrieve dormant)
```

**On the new `/governance/results/` category:** Introduced 21 May 2026 to house the Tier 0 closure memo. It is the correct home because the memo was produced under current governance framing (so not `/docs/`), and is neither doctrine, pre-registration, observation, operational state, archive, nor sync. It is an execution-result artifact, a category that did not previously exist because no execution had previously produced a result. This is a genuine repository evolution: the decomposition now spans doctrine, pre-registration, observations, state, and execution results. Per Lesson 5 (§11), introducing a new category is itself a repository-architecture decision carrying doctrinal meaning; it was introduced under explicit operator audit (21 May 2026), not AI consensus alone.

**Topology principles operationally locked:**

- Doctrine extraction is no longer pending. Six Item 24 doctrine modules exist as canonical artifacts in `governance/doctrine/`, joined as of 25 May 2026 by the first Item 29 doctrine module (`item_29_completeness_ontology.md`). The doctrine layer now spans two Items. As of 7 June 2026 the layer also holds the Tier A perturbation spec and its signed adjudication memo, the cross-Item substrate-identity discipline, and the cross-cutting positioning doctrine; the §8 tree above lists the full current contents.
- Item 24 doctrine modules are cross-referenced via full repository paths (not bare filenames) so the dependency chain survives future repository reorganization.
- Repository organization is governance-significant: where an artifact lives carries meaning, and where artifacts are *not* moved also carries meaning (see §9).

---

## 9. Framing-Provenance Policy (Operational, Non-Constitutional)

**Status:** Operational governance policy. NOT constitutional doctrine. Evidenced by one transition sequence (Item 28 → Item 24); promotion to constitutional status conditional on repeated longitudinal governance behavior across multiple future doctrinal generations.

**Policy statement:**

> Artifacts produced under superseded framing remain preserved at their original repository location to maintain framing-provenance integrity and prevent retroactive doctrinal normalization. Artifacts produced under the current governance decomposition posture are routed into the `governance/` hierarchy. The Item 28 ↔ Item 24 repository asymmetry is the first operational instance of this policy.

**Historical framing preservation ≠ doctrinal supersession.** Item 28 artifacts residing at `/docs/` does NOT mean Item 28 doctrine remains active over Item 24 doctrine. It means the historical artifacts are preserved in situ under the framing in which they were produced, while the current governing posture lives elsewhere (REACTIVE_CORE.md §12, Item 24 doctrine stack). The `/docs/` ↔ `/governance/` asymmetry is intentional provenance preservation, not unresolved governance conflict, and not organizational noise.

**Concrete instance:** The Item 28 pre-registration was framed under the pre-correction "entropy / adversarial filenames" vocabulary. REACTIVE_CORE.md §12 (14 May 2026 evening) corrected that framing constitutionally. The scoping memo's §§1-12 preserve the original framing as historical record; §13 governs interpretation going forward. Migrating the scoping memo into `governance/` would imply post-correction doctrinal alignment the artifact does not originally possess. Leaving it at `/docs/` preserves the framing-provenance signal.

**Reading guidance for future sessions:** When `/docs/` and `/governance/` contain artifacts on the same Item or topic, read the asymmetry as a *temporal-doctrinal* signal (the `/docs/` artifact predates the current governing posture; the `/governance/` artifact embodies it), not as a routing inconsistency to be cleaned up.

---

## 10. Governance Transition State

The monolithic CLAUDE.md has been frozen and archived as `/governance/archive/CLAUDE_v1_FINAL.md`. Governance authority is now layered:

| Layer | Path | Authority scope | Change frequency |
|---|---|---|---|
| Constitution | `/governance/constitution/REACTIVE_CORE.md` | Permanent doctrine | Low (constitutional amendment only) |
| Operational state | `/governance/state/CURRENT_STATE.md` | Active posture, queue, locks, residuals | Dynamic (every session) |
| Doctrine modules | `/governance/doctrine/*` | Executable doctrine details | Medium (Item 24 set now LOCKED; future Items add modules) |
| Pre-registration | `/governance/preregistration/*` | Pre-execution executable blueprints | Medium (one per pre-registered Item) |
| Execution results | `/governance/results/*` | Closure artifacts from executed phases | Medium (one per executed/closed phase) |
| Observations | `/governance/observations/*` | Non-doctrinal governance observations pending promotion | Medium (revised at Item closures) |
| Archive | `/governance/archive/*` | Historical canonical reference, rollback anchor | Static |
| Sync | `/governance/sync/*` | Non-canonical session continuity | Dynamic, explicitly non-canonical |
| Historical artifacts | `/docs/*` | Pre-correction-framing-locked artifacts (Item 28 scoping memo, W1.1 memos, etc.) | Static (framing-provenance preserved) |

**Critical principle:** Avoid loading closed historical material by default. The archived monolith is reference, not auto-load. Future session prompts load `REACTIVE_CORE.md` + `CURRENT_STATE.md` as default context; doctrine modules, pre-registration, and execution-result memos are loaded selectively when relevant. The Item 28 scoping memo at `/docs/` is loaded when Item 24 execution gates are being designed (the scoping memo §9, §14.5.1, §15.7 are operational inputs to Item 24).

**Empirical signals worth recording (Item 24 design-closure governance-side):**
- The constitutional layer (REACTIVE_CORE.md §12) was referenced operationally throughout the seven-step chain, without being modified. ✓
- The operational state layer (this file) is the surface receiving Item 24 design-closure and Tier 0 closure amendments. ✓
- The archived monolith was not auto-loaded during the seven-step design session. ✓
- Doctrine modules in `/governance/doctrine/` were authored as locked artifacts, not as drafts inside CURRENT_STATE. The decomposition is now operational, not merely intended. ✓
- Tier 0 execution produced an execution-result artifact filed in the new `/governance/results/` category, and Lock 4 held throughout. ✓

**Key distinction stabilized:**

> Continuity ≠ canon. Historical framing preservation ≠ doctrinal supersession.

---

## 10.5 Governance Observation 001 (Preserved, Observational, Non-Doctrinal)

**Status:** OBSERVATIONAL — non-doctrinal, non-constitutional. Preserved across Item 24 design phase and Tier 0. Candidate for cross-Item promotion if pattern survives empirically across future doctrinal generations.

**Canonical location:** `/governance/observations/item_24_governance_observation_001.md` (v1.1).

**Core pattern:**

> Epistemic structures tend to accumulate unintended normative semantics unless explicitly constrained. Governance structures must distinguish epistemic organization from normative judgment unless the latter is explicitly intended and ratified.

**Empirical base:** Six documented governance drift events across Items 28 and 24 (full enumeration in the artifact). The strongest evidence is recurrence within the same governance sequence after explicit corrective discipline was already in place, which suggests the pattern is structural rather than incidental. The Tier 0 session surfaced a further low-grade instance: an early inter-AI characterization drifted toward resilience-narrative framing ("stress-tested," "survived," "without collapsing") that overstated what a bounded methodology-validation run established; it was corrected to descriptive language at the operator-audit gate before entering the state layer. This is consistent with the GO-001 pattern and is recorded here as a state-layer note, not a new artifact event.

**Disposition:** Reviewed at Item 24 design closure and again at Tier 0 closure. Promotion to doctrine conditional on survival, generalization, and operationalization criteria being met across future Items. Promotion to constitutional status conditional on doctrine survival across multiple Items.

**State-layer implication:** GO-001 is operationally relevant for governance hygiene during Item 24 execution and future Item design phases. AI agents and operators should treat any framing-vocabulary drift toward normative or evaluative language (especially during admissibility, ontology, or sequencing decisions, and including resilience-narrative drift during execution-result characterization) as a candidate GO-001 instance and surface it explicitly rather than allowing it to settle silently.

---

## 11. Three-AI Workflow State

Current daily tooling combo: Claude Pro + Gemini 2.5 Pro. ChatGPT reinstated as second-opinion partner. Three-AI governance workflow:

- **Claude:** governance, doctrine drafting, code review, file authorship, analysis of outputs Laurent reports.
- **Gemini 2.5 Pro:** structured extraction at temperature 0, audit partner, primary doctrinal ratifier.
- **ChatGPT:** second-opinion partner, cross-review of strategic decisions, framing assistance.

Workflow pattern: Claude proposes → ChatGPT reviews / frames → Gemini ratifies → Claude executes (writes complete paste-and-replace file) → Laurent pastes.

**Workflow lessons recorded across Items 28 and 24:**

*Lesson 1 — Mechanical-error detection.* Cross-AI workflow surfaces mechanical errors (validator re-run mistaken for extraction re-run, Item 28 closure). Single-AI workflow would likely have missed this.

*Lesson 2 — Logical-error detection.* Cross-AI workflow surfaces logical errors (reproducibility-under-entropy mistaken for reproducibility-attributable-to-entropy, Item 28 closure). Single-AI workflow would likely have missed this.

*Lesson 3 — Posture-error detection requires explicit operator audit, NOT three-AI consensus.* During Item 28, three independent AIs converged on the wrong frame ("entropy / adversarial filename") at three separate ratification gates. The frame was internally coherent; it was still wrong at the posture level. Detection came from operator pushback grounded in product knowledge that none of the AIs surfaced from training data.

*Lesson 4 — Sequencing-discipline errors recur even after framing correction.* The Item 28 → Item 24 transition initially proposed gate-collapse (combining Item 28 closure and Item 24 execution authorization into one cycle), which would have inherited pre-correction defects into Item 24. Operator audit caught this before lock-in.

*Lesson 5 — AI consensus is insufficient ratification on ontology, admissibility framing, sequencing collapse, or institutional-reference-distribution assumptions.* The Item 24 seven-step design phase empirically demonstrated: (a) operator intervention remained structurally necessary across multiple steps; (b) calibration loops between adjacent dependency stages were necessary, not optional; (c) one AI catching another's drift within a single step is an operational feature, not an anomaly; (d) repository architecture decisions themselves carry doctrinal meaning (the mid-session `docs/` → `governance/doctrine/` reorganization for Item 24 had the same character as admissibility taxonomy decisions). The drift pattern documented in GO-001 §2.6 re-attempted to establish itself within the same governance sequence even after explicit corrective discipline was in place.

*Lesson 6 (NEW — 20–21 May 2026) — AI-generated narrative synthesis can diverge from primary artifacts during execution review.* In the Tier 0 review, an AI-generated batch summary characterized substrate behavior in terms the underlying JSONs and grader output did not support. The corrective was preserved raw artifacts plus deterministic re-grading, not cross-model review. Cross-model review did not self-correct the narrative; artifact-grounded verification did. Recorded as residual #11 (evidence-hierarchy observation, narrowly scoped, non-doctrinal). The standing implication: during characterization review, treat deterministic instrumentation and preserved primary artifacts as outranking narrative synthesis, under the conditions observed, pending broader scope characterization.

*Workflow resilience signal — ChatGPT credit-wall incident (16 May 2026).* ChatGPT hit a credit wall partway through the Item 24 design session and missed Steps 4 through 7. Gemini assumed the drafting/review role for the second half. Governance coherence was preserved. The three-AI workflow is resilient to temporary one-AI absence when doctrinal discipline holds across the remaining AIs.

*Workflow resilience signal — recurrence (24 May 2026).* The same pattern recurred during Item 29 design-session closure: ChatGPT was out of credits, and Gemini conducted the formal review and ratification of the Bounded Ontology Memorandum. The chain completed (Claude drafts → Gemini ratifies → operator pastes) with governance coherence preserved. Second instance of the resilience signal; consistent with the 16 May observation.

*Lesson 7 (NEW — 25 May 2026) — the "comfortable middle" was adopted only after a formal operator-audit gate, not by default.* In adjudicating Q6 and Q4a, both rulings landed on the Path C "middle" option (capture the observable, prohibit the inferential). Path C is precisely the kind of compromise that can settle by inertia because it feels safe. Here it did not: the drafting AI explicitly flagged the comfortable-middle risk before adjudication, the options were audited by ChatGPT and Gemini, and the operator adjudicated each ruling on its merits (including resolving the document-unit-vs-reference-unit sub-question and reaffirming both hard constraints). The C-on-both outcome therefore passed the operator-audit gate that interpretation-boundary questions require under Lesson 5, rather than being accepted by default. This is recorded as a positive instance: the governance model correctly forced intentionality on a boundary question instead of letting the convenient answer install itself.

**Governance lesson, locked:** AI consensus is a useful signal for logical and structural rigor. It is NOT a sufficient ratification mechanism on framing, posture, sequencing, ontology, admissibility, or institutional-reference-distribution questions. On all of those, explicit operator audit of underlying assumptions is required regardless of how many AIs have ratified.

**Operational implication for future ratifications:** Multi-AI consensus on logical or structural questions can proceed. Multi-AI consensus on framing, vocabulary, reference-distribution, ontology, admissibility, or sequencing questions requires an additional operator-audit gate before lock-in. The cost of the additional gate is small; the cost of missing a posture error is large.

This is governance characterization, not doctrine. It belongs here in the operational state layer rather than in the constitutional layer (constitutional clauses are timeless principles; incident provenance belongs in the operational record).

---

## 12. Authority

This file is operational state. It is authored by Claude per file-authorship discipline. It is expected to evolve frequently — each session may update queue items, lock status, posture, or residual registry entries. Constitutional matters are NOT amended here; they require explicit amendment to `REACTIVE_CORE.md`. Doctrinal matters are NOT amended here; they require amendment to the relevant artifact in `/governance/doctrine/` or `/governance/preregistration/`.

When this file and the archived monolith diverge on operational matters, this file governs (it is the current state). When they diverge on constitutional matters, the archived monolith governs until reconciled. When this file and any Item 24 doctrine module diverge, the doctrine module governs.
