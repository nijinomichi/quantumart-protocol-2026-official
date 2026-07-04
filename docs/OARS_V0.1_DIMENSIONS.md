# OARS v0.1 Dimension Profile

## Status

This document defines the initial reporting profile for **OARS v0.1-draft**.

OARS does not define beauty itself. It defines a reproducible coordinate system for describing, comparing, and discussing aesthetic processes. The distinction between required and optional dimensions concerns **reporting obligations**, not claims that every dimension must produce a non-zero score.

For a required dimension, an experiment must either:

1. report a value and method,
2. report qualitative evidence when quantification is not justified, or
3. declare `not_applicable` with a reason.

A missing value without explanation is not valid OARS v0.1 reporting.

## Required Core Dimensions

The following six dimensions are required for every OARS v0.1 research record.

### 1. R — Reproducibility

Whether another person can reconstruct the transformation or analysis from the published data, code, environment, parameters, and versioned dependencies.

Minimum record:

- source reference,
- procedure or executable method,
- environment and dependency versions,
- parameters and seeds where relevant,
- output hash or equivalent identity record.

### 2. T — Transparency

Whether the project discloses its assumptions, limitations, human and AI roles, uncertainty, licensing, and changes made during production.

Transparency is not the same as publishing all private material. Ethical non-disclosure must be explained without exposing protected information.

### 3. F — Failure Emergence

How divergence between intention and outcome is identified, recorded, interpreted, and allowed to influence later work.

A high value is not automatically desirable. OARS records how failure functions in the process rather than rewarding failure for its own sake.

### 4. H — Human Co-creation

How human judgment, authorship, intervention, consent, and responsibility participate in the process.

When no AI or collaborative system is involved, the record may describe the human decision structure or declare the collaborative component `not_applicable`.

### 5. B — Creative Branch Count

How many meaningful creative alternatives were created, merged, rejected, archived, or remain active.

Recommended representation:

\[
B=(B_{merged},B_{rejected},B_{active},B_{archived})
\]

Branch count measures process divergence, not aesthetic quality. Artificially generating branches to inflate the count is invalid.

### 6. O — Observation Diversity

How varied the declared observations, observer positions, interpretations, or participant groups are.

When observer groups are ethically and methodologically justified, diversity may be represented using Shannon entropy:

\[
O=-\sum_i p_i\log p_i
\]

The grouping method must be declared before analysis. Sensitive personal attributes must not be used without a legitimate ethical basis and informed consent.

## Optional Contextual Dimensions

The following six dimensions are optional and should be activated only when their use is justified by the experiment.

### 7. Q — Quantum-inspired Uncertainty Representation

Records how uncertainty, indeterminacy, phase, probability, or related concepts are represented.

Every use must be labelled as one of:

- physical,
- computational,
- metaphorical.

`Q` is not a universal measure of quantumness and must not be presented as a new physical observable.

### 8. φ — Compositional Harmony

Records declared compositional relations, including golden-ratio structures when actually used.

Golden-ratio use is neither mandatory nor presumed superior. Other compositional systems may be documented under the same coordinate when the method is declared.

### 9. E — Prompt Entropy

Records diversity or uncertainty within a declared prompt unit such as tokens, semantic categories, instructions, or generated branches.

For a declared distribution \(p_i\):

\[
E=-\sum_i p_i\log p_i
\]

The tokenizer, model, category scheme, and sampling procedure must be published. Experiments without prompts should report this dimension as `not_applicable` or omit it as an optional coordinate.

### 10. S — Failure Sharing Rate

Records the proportion of ethically publishable failures intentionally shared with collaborators or observers:

\[
S=\frac{N_{shared\ failures}}{N_{recorded\ failures}}
\]

A higher sharing rate is not automatically better. Privacy, safety, dignity, consent, and confidentiality can justify non-disclosure.

### 11. τ — Trust Recovery Time

Records elapsed time between a predeclared trust rupture and a predeclared recovery condition:

\[
\tau=t_{recovered}-t_{rupture}
\]

If recovery does not occur during the study window, the observation must be reported as right-censored rather than converted into a false success or failure value.

### 12. AR — Aesthetic Resonance

A context-dependent derived score or qualitative synthesis:

\[
AR=g(\mathbf{A};\mathbf{w},\mathcal{C})
\]

The function \(g\), weights \(\mathbf{w}\), and evaluation context \(\mathcal{C}\) must be declared before analysis. AR must never be presented as a universal measurement of beauty.

## OARS v0.1 State Profile

The full coordinate space remains:

\[
\mathbf{A}=(R,T,F,Q,\phi,H,E,B,O,S,\tau,AR)
\]

For v0.1 reporting, it is partitioned as:

\[
\mathbf{A}_{core}=(R,T,F,H,B,O)
\]

\[
\mathbf{A}_{optional}=(Q,\phi,E,S,\tau,AR)
\]

This partition may be revised in later versions through an RFC and documented migration path.

## Non-goals

OARS v0.1 does not:

- calculate a true value of beauty,
- rank people or cultures,
- infer trustworthiness from personal traits,
- turn artistic metaphors into physical claims,
- require disclosure that violates consent, safety, or privacy,
- reward metric inflation.

## Review Requirement

Before integration into `main`, reviewers should confirm:

- the six required dimensions are applicable across the intended research scope,
- `not_applicable` handling is explicit,
- optional metrics cannot be mistaken for universal requirements,
- physical, computational, empirical, and metaphorical claims remain distinguishable,
- privacy, consent, uncertainty, and right-censoring are handled correctly.
