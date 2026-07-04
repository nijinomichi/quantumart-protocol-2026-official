# OARS — Open Aesthetic Research System

## Position

**OARS (Open Aesthetic Research System)** is a proposed open coordinate system for researching aesthetic processes in scientific visualization, computational art, and human–AI co-creation.

OARS does **not** define beauty itself and does not claim that trust, forgiveness, beauty, or failure are physical quantum observables. It provides a reproducible structure for describing, comparing, and discussing aesthetic processes without collapsing them into one universal score.

CoPhelia³ and RadicanTrust™ operate **on top of OARS** as distinct protocol modules:

- **OARS** defines the shared research coordinates, measurement rules, provenance requirements, and claims boundaries.
- **CoPhelia³** defines a failure-sharing and co-creation protocol.
- **RadicanTrust™** defines a trust, provenance, transparency, and revision protocol.

This separation prevents one concept from becoming a container for every concern. The system becomes stronger by making the interfaces between components explicit.

## Core Research Question

> How can scientific data, aesthetic transformation, failure, trust, and public interpretation remain distinguishable, reproducible, and mutually generative within one shared research system?

## System Architecture

### Layer 0 — Scientific Source

Records the original dataset, license, acquisition time, uncertainty, instrument, and stable source URL.

### Layer 1 — Transformation

Records preprocessing, mathematical mappings, software versions, parameters, random seeds, and output hashes.

### Layer 2 — Aesthetic Interpretation

Records artistic decisions that are not scientific claims: color systems, composition, rhythm, metaphor, poetic annotation, and curatorial framing.

### Layer 3 — Participation and Trust

Records consent, accessibility, observer feedback, disagreement, revision history, failure sharing, and the distinction between anonymous participation and attributed authorship.

### Layer 4 — Protocol Modules

Hosts protocols that operate over the shared OARS coordinates.

- CoPhelia³ uses failure, dialogue, branching, and co-creation records.
- RadicanTrust™ uses provenance, transparency, recovery, and revision records.
- Future modules may be added without redefining the OARS coordinate system.

## Operational Terms

- **OARS**: the common research system and coordinate space.
- **CoPhelia³**: an artistic and social protocol for sharing failed attempts and converting them into dialogue and new branches.
- **RadicanTrust™**: a protocol for building and evaluating trust through provenance, transparency, recovery, revision, and reproducibility.
- **Quantum aesthetics**: artistic inquiry informed by quantum science, its instruments, concepts, limits, and public meanings. The term does not imply a new physical theory.
- **Failure**: a divergence between intention and outcome that may remain meaningful even when no correctable mistake occurred.

## Minimal Research Record

Every public experiment should publish:

1. source dataset and license,
2. exact data subset,
3. transformation parameters,
4. code or executable method,
5. software environment,
6. output checksum,
7. human and AI roles,
8. known uncertainties and limitations,
9. accessibility notes,
10. consent and participation conditions,
11. revision and dispute channel,
12. failed attempts and abandoned branches when ethically publishable.

## OARS Aesthetic State Vector

OARS represents an aesthetic process as a vector rather than a single beauty score:

\[
\mathbf{A}
=
(R,T,F,Q,\phi,H,E,B,O,S,\tau,AR)
\]

where:

- \(R\): reproducibility,
- \(T\): transparency,
- \(F\): failure emergence,
- \(Q\): quantum-inspired uncertainty representation,
- \(\phi\): compositional harmony, including declared golden-ratio relations when used,
- \(H\): human co-creation quality,
- \(E\): prompt entropy,
- \(B\): creative branch count,
- \(O\): observation diversity,
- \(S\): failure sharing rate,
- \(\tau\): trust recovery time,
- \(AR\): aesthetic resonance.

The vector is descriptive, not metaphysical. It does not reveal a true or universal quantity of beauty.

## Metric Boundaries

### Failure Sharing Rate

\[
S
=
\frac{N_{shared\ failures}}
{N_{recorded\ failures}}
\]

This measures the proportion of recorded failures that are intentionally shared with collaborators or observers. A higher value is not automatically better; privacy, consent, safety, and context can justify non-disclosure.

### Trust Recovery Time

\[
\tau
=
t_{recovered}-t_{rupture}
\]

This measures the elapsed time between a declared trust rupture and recovery according to a predeclared operational criterion. If recovery never occurs within the study window, the result is right-censored rather than forced into a numeric success.

### Observation Diversity

For declared observer groups with proportions \(p_i\):

\[
O
=
-\sum_i p_i\log p_i
\]

This is a Shannon-entropy measure of observer-distribution diversity. The grouping scheme must be declared in advance and must not use sensitive categories without a legitimate ethical basis and consent.

### Creative Branch Count

\[
B
=
|\mathcal{B}_{created}|
\]

Branches should also be reported by state:

\[
B=(B_{merged},B_{rejected},B_{active},B_{archived})
\]

The count measures divergence in the creative process, not quality. Artificially generating branches to inflate the metric is invalid.

### Prompt Entropy

Prompt entropy must be tied to an explicit unit of analysis. For a declared distribution \(p_i\) over prompt tokens, semantic categories, instructions, or generated branches:

\[
E
=
-\sum_i p_i\log p_i
\]

No single implementation is canonical. The tokenizer, category scheme, model, and sampling procedure must be published.

### Aesthetic Resonance

\[
AR
=
g(\mathbf{A};\mathbf{w},\mathcal{C})
\]

Aesthetic Resonance is a context-dependent derived score. The function \(g\), weights \(\mathbf{w}\), and evaluation context \(\mathcal{C}\) must be declared before analysis. OARS does not permit AR to be presented as a universal measurement of beauty.

## Evaluation Without a Universal Beauty Score

The primary output of OARS is the complete vector \(\mathbf{A}\), together with methods, uncertainty, and qualitative interpretation.

A weighted aggregate may be used for a specific exhibition, experiment, or study only when:

1. the purpose is stated,
2. the weights are published,
3. uncertainty is reported,
4. qualitative disagreement remains visible,
5. the aggregate is not described as beauty itself.

## Claims Boundary

OARS distinguishes four claim types:

1. **Physical claim** — supported by scientific data and an established method.
2. **Computational claim** — supported by code, parameters, and reproducible output.
3. **Empirical human-study claim** — supported by declared participants, consent, protocol, and analysis.
4. **Artistic or philosophical interpretation** — presented as interpretation rather than measurement.

The use of terms such as superposition, entanglement, phase, resonance, or uncertainty must be marked as physical, computational, or metaphorical in each experiment.

## Next and Next Plan

### Phase 1 — Canonicalization

- Publish OARS definitions and claims boundaries.
- Separate the OARS system from CoPhelia³ and RadicanTrust™ protocol modules.
- Create machine-readable metric and provenance schemas.
- Establish one canonical owner for each definition, dataset, metric, and renderer.

### Phase 2 — Reference Experiments

- Gravitational-wave visualization from open detector data.
- Quantum microscopy visualization with perceptually uniform color mapping.
- Prompt-order experiment demonstrating non-commutative sequencing as a computational analogy, not a physical claim.
- Failure Phase Diagram using observer responses, branch records, and revision logs.
- Trust-recovery pilot with a predeclared recovery criterion.

### Phase 3 — Public Reproducibility

- Release scripts, environments, hashes, and sample outputs.
- Run independent reproduction attempts.
- Archive failed reproductions rather than deleting them.
- Publish disagreement notes alongside successful outputs.
- Report missing data and censored trust-recovery cases.

### Phase 4 — Research Community Connection

Prepare distinct contribution packages for:

- **Digital humanities and aesthetics**: failure, anti-optimization, authorship, interpretation.
- **HCI / CHI**: human–AI co-creation, trust calibration, consent, accessibility, and observer studies.
- **Visualization / VIS**: provenance-aware scientific visualization and uncertainty communication.
- **SIGGRAPH / computational art**: reproducible transformation pipelines and generative visual systems.
- **AI research / NeurIPS workshops**: prompt ordering, model variability, prompt entropy, and plural evaluation criteria.
- **Open science communities**: reproducible artifacts, data citation, versioned methods, and negative results.
- **Quantum outreach networks**: accurate public communication of quantum science through art.

### Phase 5 — Community Protocol

- Open a request-for-comments process.
- Accept multilingual issues and anonymous feedback routes.
- Define contributor roles and conflict-of-interest declarations.
- Publish annual OARS revisions with migration notes.
- Invite external researchers to challenge the coordinate definitions and metric assumptions.

## Proposed Research Outputs

1. OARS system specification
2. Claims-boundary standard
3. Machine-readable metric schema
4. Dataset provenance schema
5. CoPhelia³ protocol specification
6. RadicanTrust™ protocol specification
7. Reference implementation
8. Failure and revision archive
9. Observer-study protocol
10. Accessibility, ethics, and consent checklist
11. Citation file and versioned releases
12. Research paper and exhibition package

## Immediate 30-Day Plan

- Week 1: freeze OARS vocabulary, metric definitions, and provenance schema.
- Week 2: publish one reproducible visualization notebook and one artistic transformation record.
- Week 3: conduct a small observer study with explicit consent and qualitative disagreement capture.
- Week 4: release OARS v0.1 research package and open the first RFC.

## Invitation

OARS is not complete by design.

Researchers, artists, engineers, educators, and critics are invited not merely to endorse it, but to test where it fails. A system for studying trust and aesthetics becomes credible only when its weaknesses remain visible, versioned, and open to revision.
