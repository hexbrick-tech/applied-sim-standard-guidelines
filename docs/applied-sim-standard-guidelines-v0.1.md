# Applied SIM Standard Guidelines v0.1

**Status:** Draft  
**Version:** 0.1

## 1. Purpose

The Applied SIM Standard Guidelines (ASG) define the semantic interface between SIM Foundation and Applied SIM practices.

ASG does not prescribe a single analysis procedure, domain model, implementation, tool, or AI system. It specifies constraints that preserve Foundation semantics when they are applied in a concrete practice.

### Responsibility

ASG defines conformance constraints for Applied SIM practices. Its responsibility is to preserve the semantic distinctions and constraints established by SIM Foundation while allowing Applied practices to define domain-specific procedures, artifacts, roles, workflows, and implementations.

ASG does not establish a canonical reasoning procedure, redefine Foundation concepts for operational convenience, or require an Applied practice to resolve semantic states beyond what its inquiry requires. Applied procedures may introduce stronger operational controls where useful, but those controls remain distinguishable from semantics inherited from Foundation.

## 2. Normative language

The terms **MUST**, **MUST NOT**, **SHOULD**, **SHOULD NOT**, and **MAY** express normative requirements.

A practice claiming conformance MUST identify the ASG version to which it conforms.

## 3. Foundation semantics

Applied practices MUST preserve the semantics inherited from SIM Foundation rather than redefine them for implementation convenience.

This draft focuses on the application of Observation, Interpretation, Evaluation, Semantic Boundary, boundary stability, and resistance to narrative completion.

Traceability from each normative requirement to SIM Foundation is intentionally subject to a subsequent Foundation consistency review.

## 4. Observation Integrity

### ASG-O1 — Evidence-bounded observation
An Observation **MUST NOT** assert semantic content that is not supported by what was actually observed.

### ASG-O2 — Observation preservation
Ambiguity in an Observation **MUST NOT** be resolved merely to make a downstream model complete.

### ASG-O3 — Observed is not defined
The existence of an observed expression, action, role, or object **MUST NOT** by itself be treated as proof that a stable Semantic Boundary has been established for a corresponding Concept.

### ASG-O4 — Inference separation
A conclusion inferred from Observation **MUST** be represented as Interpretation rather than silently incorporated into Observation.

## 5. Interpretation Discipline

### ASG-I1 — Traceability
An Interpretation **MUST** remain traceable to the Observation or Observations from which it was derived.

### ASG-I2 — No backward contamination
An Interpretation **MUST NOT** be treated as if it had been directly observed.

### ASG-I3 — Contestability
An Applied practice **SHOULD** preserve the ability to challenge an Interpretation with an alternative explanation when the available Observations permit one.

## 6. Evaluation Discipline

### ASG-E1 — Evaluation context
An Evaluation **MUST** identify or preserve the context required to understand the judgment, including the relevant purpose, criteria, or perspective where applicable.

### ASG-E2 — No intrinsic projection
An Evaluation **MUST NOT** be projected backward as an intrinsic property of an Observation or Interpretation.

## 7. Unknown and Undefined

### ASG-U1 — Unknown
An Applied practice **MUST** preserve Unknown as the state in which information required to determine meaning is not known. It **MUST NOT** narrow Unknown to a particular kind of missing fact, value, attribute, relation, Concept, or Semantic Boundary.

### ASG-U2 — Undefined
An Applied practice **MUST** preserve Undefined as the state in which something is observed but cannot currently be placed within an established semantic structure. It **MUST NOT** redefine Undefined as requiring any particular diagnosis, including failure to establish a stable Semantic Boundary for a Candidate Concept.

### ASG-U3 — Separation
An Applied practice **MUST NOT** use Undefined as a generic category for missing information.

### ASG-U4 — Observation retention
Marking a Candidate Concept as Undefined **MUST NOT** erase or invalidate the underlying Observation.

## 8. Boundary Validation

### ASG-B1 — Boundary authority
An Applied practice **MUST NOT** treat a provisional, unstable, or merely assumed Semantic Boundary as established semantic authority. Downstream use **MAY** proceed when the inquiry permits it, provided the boundary's status remains observable.

### ASG-B2 — Placement before Undefined
An Applied practice **SHOULD NOT** treat an observed element as Undefined without considering whether the available Observation already permits it to be placed within an established semantic structure. This consideration **MUST NOT** require a particular diagnostic or counter-hypothesis procedure.

### ASG-B3 — Missing detail is not boundary failure
A missing property, relationship, exception rule, or detailed behavior **MUST NOT** by itself be treated as evidence that a Semantic Boundary is absent or unstable.

## 9. Semantic Probes

### ASG-P1 — Observation-seeking probes
A Semantic Probe **SHOULD** seek additional observable facts rather than ask a human to choose among structures already assumed by the analysis.

### ASG-P2 — Narrative restraint
A Semantic Probe **MUST NOT** introduce an unobserved model as though that model were already established.

### ASG-P3 — Boundary probes
When a Candidate Concept lacks a stable boundary, the practice **SHOULD** probe observable behavior that can reveal where the Concept begins, ends, differs from adjacent Concepts, or becomes complete.

### ASG-P4 — Expansion probes
A practice **MAY** probe relationships, reuse, constraints, actors, or surrounding context after or alongside boundary investigation, provided those probes do not silently establish the boundary they are intended to investigate.

## 10. Feedback

### ASG-F1 — Feedback is a normal path
Failure to establish a Semantic Boundary **MUST** be permitted to return the analysis to further Observation. Such feedback is a normal analytical path, not an exceptional failure.

### ASG-F2 — Missing-observation identification
When practical, feedback from Undefined **SHOULD** identify what Observation is missing and what Probe could obtain it.

### ASG-F3 — Reassessment
A Candidate Concept **SHOULD** be reassessed after new Observation is obtained rather than retaining Undefined by default.

## 11. Narrative Non-Completion

### ASG-N1 — No plausibility completion
Missing semantic content **MUST NOT** be filled solely because a completion is plausible, conventional, or consistent with general domain knowledge.

### ASG-N2 — Explicit inference
When general knowledge or reasoning is intentionally used, its result **MUST** remain distinguishable from Observation.

### ASG-N3 — AI assistance
An AI-assisted Applied practice **MUST NOT** treat an AI system's ability to generate a plausible completion as evidence that the completion was observed.

## 12. Conformance and Traceability

### ASG-C1 — Version declaration
A conforming Applied practice **MUST** identify the ASG version it targets.

### ASG-C2 — Requirement mapping
A conforming practice **SHOULD** be able to show how its process, artifacts, or controls satisfy applicable ASG requirements.

### ASG-C3 — Foundation provenance
ASG normative requirements **SHOULD** be traceable to supporting semantics or invariants in SIM Foundation.

Where a requirement cannot be supported by Foundation, it **MUST** be identified for Foundation consistency review rather than silently treated as Foundation semantics.

## 13. Reference reasoning pattern

The following pattern is illustrative, not a mandatory workflow:

```
Observation
    |
    v
Candidate Concept
    |
    v
Boundary investigation
    |
    +-- sufficiently stable --> downstream use
    |
    +-- insufficient --------> Undefined
                                  |
                                  v
                         identify missing Observation
                                  |
                                  v
                            Semantic Probe
                                  |
                                  v
                              Observation
                                  |
                                  +----> reassess boundary
```

Unknown follows a different path: the Concept is sufficiently established, while a required fact or property remains unknown.

## 14. v0.1 review targets

Before promotion beyond Draft, this version should be reviewed in two directions:

1. **Downstream conformance:** align Applied SIM for Business Analysis with these requirements.
2. **Upstream consistency:** map each normative requirement to SIM Foundation and identify Supported, Partial, or Foundation Gap cases.

The motivating validation criterion for v0.1 is that failures such as interpretation leaking into Observation, generic use of Undefined, premature boundary assertion, and narrative-producing Semantic Probes are either prevented or made observable by a conforming Applied practice.
