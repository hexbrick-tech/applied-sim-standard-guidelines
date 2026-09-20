# ASG v0.1 — SIM Foundation Traceability Mapping

**Status:** Initial review
**ASG target:** v0.1 Draft
**Foundation authority:** English SIM canon

## Classification

- **Supported** — directly supported by Foundation semantics or an explicit Foundation constraint.
- **Partial** — Foundation supports the direction, but ASG narrows, strengthens, or adds a condition.
- **Gap** — a potentially foundational invariant not currently established explicitly in the reviewed canon.
- **Applied-specific** — a legitimate standard/application concern rather than inherited Foundation semantics.

This mapping does not modify ASG v0.1. It observes the current draft as written.

## Requirement mapping

| Requirement | Status | Foundation provenance | Review note |
| --- | --- | --- | --- |
| ASG-O1 Evidence-bounded observation | **Supported** | Vol.1 §2, §9; Vol.2 §4, §8; Vol.3 §4, §16; Vol.4 §3, §8, §22 | Strongly supported by source/subject/observer-added meaning distinctions. |
| ASG-O2 Observation preservation | **Supported** | Vol.1 §7; Vol.2 §7, §9; Vol.3 §13, §18; Vol.4 §7, §18 | Foundation rejects invented completeness and premature convergence. |
| ASG-O3 Observed is not defined | **Supported** | Vol.3 §7, §11, §14, §16; Vol.4 §14 | Observation of an element or implementation does not establish its semantic boundary or authority. |
| ASG-O4 Inference separation | **Supported** | Vol.1 §9; Vol.2 §4; Vol.3 §16, §22; Vol.4 §3, §8, §22 | Directly supported as prevention of unmarked interpretation / Semantic Leakage. |
| ASG-I1 Traceability | **Partial** | Vol.1 §9; Vol.2 §4; Vol.4 §3, §8 | Foundation requires interpretation to remain distinguishable from observation/source. Explicit one-or-more Observation traceability is stronger. |
| ASG-I2 No backward contamination | **Supported** | Vol.1 §9; Vol.2 §4; Vol.3 §16; Vol.4 §3, §22 | Interpretation-to-observation is explicitly identified as Semantic Leakage. |
| ASG-I3 Contestability | **Supported** | Vol.1 §9, §14; Vol.2 §8; Vol.3 §7; Vol.4 §7–§9 | Foundation preserves alternatives and treats plausible interpretation as non-authoritative. |
| ASG-E1 Evaluation context | **Partial** | Vol.1 §4, §5, §10, §14; Vol.2 §3; Vol.3 §21; Vol.4 §13 | Foundation says evaluation introduces criteria implying perspective, purpose, authority, or values. Requiring explicit context structure is stronger. |
| ASG-E2 No intrinsic projection | **Supported** | Vol.1 §4, §10; Vol.3 §21; Vol.4 §13, §22 | Evaluation must not silently rewrite observation or become intrinsic to the subject. |
| ASG-U1 Unknown | **Partial** | Vol.1 §7; Vol.3 §13; Glossary: Unknown; Vol.4 §4–§5 | Canon defines Unknown more generally as information required to determine meaning being unknown. ASG narrows it by requiring Concept/Boundary establishment. |
| ASG-U2 Undefined | **Partial** | Vol.3 §14; Glossary: Undefined; Vol.4 §5 | Canon defines Undefined as an observed element that cannot currently be placed within established semantic structure. ASG narrows it to Candidate Concept boundary failure. |
| ASG-U3 Separation | **Supported** | Vol.3 §13–§14; Glossary Meaning Handling Boundary; Vol.4 §5 | Canon explicitly distinguishes uncertainty and meaning-handling states. |
| ASG-U4 Observation retention | **Supported** | Vol.3 §14; Glossary: Undefined; Vol.4 §5 | Undefined presupposes that something has been observed; it does not invalidate Observation. |
| ASG-B1 Boundary before attribution | **Partial** | Vol.3 §7, §11, §16; Vol.4 §14 | Canon rejects hypothesis-to-definition and implementation-to-authority. Categorical prohibition on all downstream attributes is stronger. |
| ASG-B2 Counter-hypothesis | **Gap** | Related: Vol.2 §8; Vol.3 §7, §9–§10; Vol.4 §15, §20–§21 | Hypotheses/probes must be challengeable, but canon does not explicitly require Undefined itself to be challenged by “Concept already established.” |
| ASG-B3 Missing property is not missing boundary | **Partial** | Vol.3 §11, §13–§14; Glossary: Unknown / Undefined | Consistent with canon, but explicit property-vs-boundary rule is an Applied interpretation. |
| ASG-P1 Observation-seeking probes | **Supported** | Vol.3 §6, §9; Vol.4 §6, §15 | Probe increases observability rather than confirming a preselected answer. |
| ASG-P2 Narrative restraint | **Supported** | Vol.2 §8–§9; Vol.3 §9, §16; Vol.4 §8, §15 | Strongly supported by anti-leading and anti-narrative-completion guidance. |
| ASG-P3 Boundary probes | **Supported** | Vol.3 §6–§9; Vol.4 §15 | Direct application of questions/probes that vary conditions to expose a boundary. “Boundary Probe” itself is Applied terminology. |
| ASG-P4 Expansion probes | **Applied-specific** | Compatible with Vol.3 §6, §9, §24 | Useful Applied classification; Foundation does not define this probe type or ordering constraint. |
| ASG-F1 Feedback is a normal path | **Supported** | Prologue §5; Vol.3 §3, §10; Glossary: Recurrent Observation; Vol.4 §16, §21 | Re-entry and re-observation are normal SIM reasoning. |
| ASG-F2 Missing-observation identification | **Supported** | Vol.3 §6, §13–§14; Vol.4 §4, §6 | Unknown/Undefined can direct further observation and question generation. |
| ASG-F3 Reassessment | **Supported** | Vol.3 §3, §10; Vol.4 §16, §21 | Re-observation after new evidence/context is canonical behavior. |
| ASG-N1 No plausibility completion | **Supported** | Vol.1 §8–§9; Vol.2 §8–§9; Vol.4 §4, §8–§9 | Plausibility cannot manufacture meaning or authority. |
| ASG-N2 Explicit inference | **Supported** | Vol.1 §9; Vol.2 §4; Vol.3 §16; Vol.4 §3, §17, §22 | Observer-added inference remains distinguishable from Observation. |
| ASG-N3 AI assistance | **Supported** | Vol.4 §1, §4, §8–§9, §22 | Explicit application of Vol.4 AI reasoning constraints. |
| ASG-C1 Version declaration | **Applied-specific** | Related: Prologue §7–§9 | Versioned conformance is standards governance, not a Foundation invariant. |
| ASG-C2 Requirement mapping | **Applied-specific** | Related: Prologue §7, §9; Vol.3 §23–§24 | Legitimate ASG governance; not mandated by Foundation. |
| ASG-C3 Foundation provenance | **Applied-specific** | Prologue §7–§9; Vol.3 §23–§24 | Formal requirement-level provenance is ASG interface/governance responsibility. |

## Summary

| Classification | Requirements |
| --- | --- |
| **Supported (18)** | O1, O2, O3, O4, I2, I3, E2, U3, U4, P1, P2, P3, F1, F2, F3, N1, N2, N3 |
| **Partial (6)** | I1, E1, U1, U2, B1, B3 |
| **Gap (1)** | B2 |
| **Applied-specific (4)** | P4, C1, C2, C3 |

## Primary review findings

### 1. Foundation coverage is strong

Most ASG v0.1 requirements are direct normative applications of existing Foundation semantics. Vol.4 already contains strong constraints against Unknown completion, premature convergence, Narrative Attraction, implementation authority, leading probes, Evaluation Leakage, and Artificial Completeness.

### 2. Unknown / Undefined need correction in ASG

The current ASG wording narrows canonical definitions:

- **Unknown** canonically concerns unavailable information required to determine meaning.
- **Undefined** canonically concerns something observed that cannot currently be placed within established semantic structure.

The Concept-boundary formulation discovered during Business Analysis is useful, but should not replace those definitions.

### 3. O/I/E should remain Foundation distinctions, not an ASG-created pipeline

Foundation strongly establishes:

    Observation ≠ Interpretation ≠ Evaluation

It does not require every Applied SIM practice to implement O/I/E as a fixed three-stage workflow. ASG should constrain Semantic Leakage among these reasoning products without canonizing a procedural pipeline.

### 4. Counter-hypothesis is the strongest Foundation Gap candidate

ASG-B2 adds a reflexive check on the act of declaring Undefined:

    Candidate Undefined
            ↓
    Observe the classification itself
            ↓
    Could the Concept already be sufficiently established?
            ↓
    Attempt to falsify Undefined

This is highly consistent with Reflexive Observation, challengeable Boundary Hypotheses, and non-confirmatory Semantic Probes, but is not currently explicit in the reviewed Foundation text.

### 5. Probe taxonomy belongs naturally in Applied/ASG space

“Boundary Probe” is a useful name for canonical probe behavior. “Expansion Probe” is a useful Applied classification. Neither needs to become a new Foundation concept unless later observations show that the distinction is domain-independent and semantically necessary.

## Next review action

Before changing ASG v0.1:

1. review each **Partial** item and decide whether to loosen ASG wording or intentionally retain it as an Applied standard constraint;
2. test **ASG-B2** against Vol.1–Vol.4 as a possible Foundation refinement;
3. revise U1/U2 so they import canonical Unknown/Undefined semantics instead of redefining them;
4. preserve Applied-specific governance and probe taxonomy without presenting them as Foundation definitions.
