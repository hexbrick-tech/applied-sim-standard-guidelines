# ASG v0.1 — Responsibility Review

**Status:** Completed review  
**Target:** ASG v0.1 Draft  
**Review basis:** ASG Responsibility + existing Foundation traceability mapping

## Review question

This review asks a different question from Foundation traceability:

> Even when a requirement is compatible with or derivable from SIM Foundation, does it belong in ASG as a conformance constraint?

The working classifications are:

- **Preserve** — fits ASG responsibility as a conformance constraint preserving Foundation semantics.
- **Reframe** — the underlying concern belongs in ASG, but the current wording narrows Foundation semantics, over-prescribes a procedure, or is stronger than necessary.
- **Applied-specific** — useful operational guidance, but better treated as an Applied method choice unless ASG explicitly intends to standardize that control.
- **Governance** — belongs in ASG because it governs conformance itself rather than inheriting semantic content from Foundation.

This review records decisions made before changing normative requirement text. The original classifications are preserved below as review provenance; see **Resolution** for their disposition in the current ASG draft.

## Requirement review

| Requirement | Responsibility review | Reason |
| --- | --- | --- |
| O1 Evidence-bounded observation | **Preserve** | Directly prevents observer-added meaning from becoming Observation. |
| O2 Observation preservation | **Preserve** | Prevents semantic completion for downstream convenience. |
| O3 Observed is not defined | **Preserve** | Preserves the distinction between observed existence and established meaning. |
| O4 Inference separation | **Preserve** | Prevents unmarked Interpretation from becoming Observation. |
| I1 Traceability | **Reframe** | Provenance is useful, but mandatory derivation from specific Observations is stronger than Foundation's minimum invariant of distinguishability. |
| I2 No backward contamination | **Preserve** | Direct Semantic Leakage constraint. |
| I3 Contestability | **Preserve** | Preserves alternative explanations where Observation permits them without imposing a fixed procedure. |
| E1 Evaluation context | **Reframe** | Evaluation basis must remain observable, but requiring a particular explicit context structure may over-prescribe representation. |
| E2 No intrinsic projection | **Preserve** | Prevents Evaluation from silently becoming an intrinsic property of Observation or Interpretation. |
| U1 Unknown | **Reframe** | Current wording narrows canonical Unknown by requiring an established Concept or Semantic Boundary. |
| U2 Undefined | **Reframe** | Current wording incorrectly equates Undefined with insufficient Candidate Concept boundary. |
| U3 Separation | **Preserve** | Prevents Undefined from collapsing into generic missing information. |
| U4 Observation retention | **Preserve** | Preserves the Observation underlying an Undefined state. |
| B1 Boundary before attribution | **Reframe** | The categorical prohibition on downstream attribution is stronger than Foundation; ASG should constrain silent semantic authority rather than require universal sequencing. |
| B2 Counter-hypothesis | **Reframe** | Core discipline is derivable from Foundation, but the named counter-hypothesis procedure and “other Concepts” framing are ASG-specific and narrower than canonical Undefined. |
| B3 Missing property is not missing boundary | **Reframe** | Useful safeguard, but should preserve canonical Unknown/Undefined distinctions without making Concept-boundary diagnosis the governing model. |
| P1 Observation-seeking probes | **Preserve** | Constrains probes toward observability rather than confirmation. |
| P2 Narrative restraint | **Preserve** | Prevents probes from silently manufacturing semantic structure. |
| P3 Boundary probes | **Applied-specific** | Valid operational specialization of Semantic Probe, but ASG need not require this named diagnostic procedure. |
| P4 Expansion probes | **Applied-specific** | Applied probe taxonomy and ordering choice, not a Foundation semantic constraint. |
| F1 Feedback is a normal path | **Reframe** | Re-observation is canonical, but tying feedback specifically to failure to establish a Semantic Boundary narrows the general recurrent-observation principle. |
| F2 Missing-observation identification | **Reframe** | Further Observation is supported, but requiring Undefined to be diagnosed into a missing Observation/Probe is stronger than Foundation. |
| F3 Reassessment | **Preserve** | Prevents a prior semantic state from becoming permanent merely by inertia after new Observation. |
| N1 No plausibility completion | **Preserve** | Directly preserves non-completion and semantic authority. |
| N2 Explicit inference | **Preserve** | Keeps observer-added reasoning distinguishable from Observation. |
| N3 AI assistance | **Preserve** | AI capability must not become evidence or semantic authority. |
| C1 Version declaration | **Governance** | Necessary for versioned ASG conformance; not claimed as Foundation semantics. |
| C2 Requirement mapping | **Governance** | Makes conformance inspectable without prescribing the Applied implementation. |
| C3 Foundation provenance | **Governance** | Protects the Foundation/ASG boundary by making inherited vs ASG-added constraints observable. |

## Summary

| Classification | Requirements |
| --- | --- |
| **Preserve (15)** | O1, O2, O3, O4, I2, I3, E2, U3, U4, P1, P2, F3, N1, N2, N3 |
| **Reframe (9)** | I1, E1, U1, U2, B1, B2, B3, F1, F2 |
| **Applied-specific (2)** | P3, P4 |
| **Governance (3)** | C1, C2, C3 |

## Cross-cutting findings

### Undefined is a state, not a diagnosis

ASG must not redefine canonical Undefined as failure to establish a Candidate Concept boundary. Boundary insufficiency may explain an Undefined state in a particular inquiry, but it is not the canonical definition and need not be diagnosed before Undefined can remain observable.

### Distinction preservation does not imply a pipeline

Foundation establishes distinctions such as:

    Observation ≠ Interpretation ≠ Evaluation

ASG should preserve those distinctions when they matter, but should not turn them into a mandatory sequence or canonical reasoning pipeline.

### Sufficiency does not require semantic completion

An Applied practice may proceed while Unknown, Undefined, Ambiguous, or Conflicting states remain, provided those states and the basis of subsequent Interpretation or Evaluation remain observable. ASG should not require resolution merely to enable downstream work.

### Applied controls may be stronger without becoming Foundation semantics

ASG may intentionally standardize stronger operational controls, but it should do so explicitly. A useful Applied procedure must not silently become a Foundation definition or invariant.

## Resolution

The review actions have been completed in the current ASG v0.1 draft.

- **Reframe resolved:** I1, E1, U1, U2, B1, B2, B3, F1, and F2 were revised to preserve Foundation semantics without requiring a canonical reasoning sequence, a narrowed definition of Unknown or Undefined, or a mandatory diagnostic procedure.
- **Applied-specific resolved:** P3 and P4 were removed from the normative ASG requirements. Their probe taxonomy remains suitable for Applied methods where useful, but is not standardized by ASG.
- **Reference workflow removed:** the former reference reasoning pattern was removed because it encoded the earlier boundary-centric workflow and conflicted with the revised U/B/F requirements.
- **Governance retained:** C1, C2, and C3 remain ASG governance requirements and are not presented as Foundation-native semantics.

The classifications above remain unchanged because they record the state and reasoning that motivated these revisions rather than the status of the revised requirements.
