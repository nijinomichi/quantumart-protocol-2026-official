# Repository Architecture

**Status:** living architecture document

**Version:** 2026-07-19

**Repository:** quantumart-protocol-2026-official

---

> This document describes the architectural roles of the public repositories
> within the BananaSpace ecosystem.
>
> It records responsibilities rather than implementation details.

---

# Purpose

The ecosystem has grown into multiple repositories with different purposes.

This document preserves the architectural relationships between those repositories
so that future contributors can understand the system without reconstructing its
history from commit logs.

This document is observational.

It is not a protocol specification.

It is not a scientific claim.

It is an architectural map.

---

# Design Principles

The architecture follows several long-term principles.

- Preserve provenance.
- Separate canonical knowledge from implementation.
- Separate incidents from production.
- Prefer non-destructive evolution.
- Record repository responsibilities explicitly.
- Keep public entry points stable.
- Preserve historical evidence whenever practical.

---

# Repository Roles

| Role | Repository | Primary Responsibility |
|------|------------|------------------------|
| Canonical Knowledge | quantumart-protocol-2026-official | Definitions, boundaries, research documents, architecture |
| Incident Origin | QuantumTrustChaosPrompt (legacy) | Historical origin of the long-path incident |
| Repair Reference | QuantumTrustChaosPrompt-v2 | Verified migration reference with continuous validation |
| Incident Reference | BananaMoon-QuantumTrust-Review | Investigation, diagnosis, and repair planning |
| Reference Repository | quantum-shogi-silent-nft | Stable public implementation with provenance |
| Public Portal | nijinomichi.github.io | Public entrance and navigation |

---

# Architectural Constellation

```
                    Canonical Knowledge
                            │
                            ▼
      quantumart-protocol-2026-official
                            │
     ┌──────────────┬──────────────┬──────────────┐
     │              │              │              │
     ▼              ▼              ▼              ▼
Incident       Repair        Reference       Public
Origin         Reference     Repository      Portal
     │              │              │              │
     ▼              ▼              ▼              ▼
QuantumTrust   QuantumTrust   quantum-       nijinomichi
ChaosPrompt    ChaosPrompt    shogi-         .github.io
(legacy)       -v2            silent-nft
                      │
                      ▼
             BananaMoon-QuantumTrust-Review
```

The repositories are complementary.

Each repository has a single primary responsibility.

Responsibilities should remain explicit.

---

# Repository Lifecycle

Documents do not become canonical merely by being published.
They move through observation, experiment, review, and reference
before canonical status is assigned.

| Stage | Meaning | Typical Artifact |
|-------|---------|------------------|
| Idea | An unverified question or concept | proposal, note |
| Experiment | Prototyping and observation | experimental record |
| Review | Human, technical, and boundary verification | PR, review log |
| Reference | Verified material ready for reuse | reference document |
| Canonical | The current authoritative source | protocol, definitions |
| Public | The guided entry point for external readers | README, portal, release |

Promotion to Canonical requires that the document has been observed,
experimented upon, reviewed, and established as a reusable reference.
Public visibility is a consequence of canonical status, not its cause.

---

# Evolution Rules

When a new repository is created, its primary architectural role should be
identified before implementation begins.

Possible roles include:

- Canonical Knowledge
- Reference Repository
- Experimental Laboratory
- Repair Reference
- Public Portal
- Archive
- Dataset
- Tooling

A repository should normally have one primary role.

---

# Boundary

This document describes repository architecture.

It does not certify scientific validity.

It does not replace repository-specific documentation.

It does not supersede LICENSE files.

It does not redefine provenance records.

---

# Maintenance

This document may evolve as the ecosystem grows.

Changes should preserve historical continuity whenever possible.

Major architectural revisions should reference the corresponding review
discussion or issue.
