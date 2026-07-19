# Repository Constellation

**Status:** living architecture document

**Version:** 2026-07-19

**Repository:** quantumart-protocol-2026-official

**Source of truth for:** nijinomichi.github.io (public rendering)

---

> This document maps the verified relationships between repositories
> in the BananaSpace ecosystem.
>
> It records what currently exists.
> It does not record intentions, future integrations, or empty scaffolding.

---

## Relationship Legend

Arrows in this document have explicit meanings.

| Symbol | Meaning |
|--------|---------|
| `──reference──▶` | Points to; one repository links to another in its documentation |
| `◀──reference──` | Receives a reference; the target is linked from the source |
| `◀──reference──▶` | Mutual reference; both repositories link to each other |
| `──role registration──▶` | The source records the target in the architecture map |
| `──operational──▶` | Uses or implements a protocol defined elsewhere |
| `──historical──▶` | Preserves lineage, incident origin, or repair history |

A double-headed arrow (`◀──▶`) indicates that both links exist in the actual files.
It does not imply equal authority or symmetric dependency.

---

## Constellation Map

### Layer 1 — Canonical Knowledge

```
quantumart-protocol-2026-official
  Role: Canonical Knowledge
  Contains: definitions, boundaries, research documents, architecture
  This document lives here.
```

### Layer 2 — Conceptual and Poetic Entry

```
cophelia3
  Role: Poetic Co-Creation Entry Point
  Contains: MANIFESTO, SOUL, CODE_OF_RESONANCE, project structure
  Note: thematic directories (experiments/, artworks/, research/) exist
        but are not yet populated.
```

Relationships:

```
quantumart-protocol-2026-official  ──role registration──▶  cophelia3
cophelia3  ──reference──▶  quantumart-protocol-2026-official
```

Both links are verified as of 2026-07-19.

### Layer 3 — Social Implementation

```
WaWaWa-Resonance-Protocol
  Role: Social Implementation Archive
  Contains: resonance-based experiments in forgiveness, trust, co-creation
```

Relationships:

```
cophelia3  ──reference──▶  WaWaWa-Resonance-Protocol  (via README ecosystem section)
WaWaWa-Resonance-Protocol  ──reference──▶  cophelia3  (via README ecosystem section)
```

Both links are verified as of 2026-07-19.

### Layer 4 — Operational Protocol

```
QuantumTrustChaosPrompt-v2
  Role: Repair Reference
  Contains: verified migration reference with continuous validation (QRA v1.1)
```

Relationships:

```
cophelia3  ──reference──▶  QuantumTrustChaosPrompt-v2
WaWaWa-Resonance-Protocol  ──reference──▶  QuantumTrustChaosPrompt-v2
```

### Layer 5 — Incident History

```
QuantumTrustChaosPrompt  (legacy)
  Role: Incident Origin
  Contains: historical origin of the long-path incident (QRA v1.0)
  Status: kept as lineage record; not actively developed

BananaMoon-QuantumTrust-Review
  Role: Incident Reference
  Contains: investigation, diagnosis, and repair planning
```

Relationships:

```
QuantumTrustChaosPrompt (legacy)  ──historical──▶  QuantumTrustChaosPrompt-v2
BananaMoon-QuantumTrust-Review  ──historical──▶  QuantumTrustChaosPrompt (legacy)
```

### Layer 6 — Provenance Artifact

```
CoPhelia Protocol 2025 Quantum Signature
  Repository: -Produced-by-Sou-Hashiguchi-Ara-Philia-CoPhelia-Protocol-2025-Quantum-Signature-1f8a9d3e--
  Role: Signature / provenance artifact
  Contains: 2025 CoPhelia Protocol signature and Resonance Field discussions
  Status: fixed provenance record
```

Relationships:

```
cophelia3  ──reference──▶  CoPhelia Protocol 2025 Quantum Signature
```

### Layer 7 — Reference Implementation

```
quantum-shogi-silent-nft
  Role: Reference Repository
  Contains: stable public implementation with provenance
```

### Layer 8 — Public Portal

```
nijinomichi.github.io
  Role: Public Portal
  Contains: public entrance and navigation for external readers
  Source of truth: this document (REPOSITORY_CONSTELLATION.md)
```

Relationships:

```
nijinomichi.github.io  ──reference──▶  quantumart-protocol-2026-official  (source of truth)
```

---

## Full Relationship Summary

```
┌─────────────────────────────────────────────────────────────────────────┐
│  Layer 1   quantumart-protocol-2026-official                            │
│            Canonical Knowledge                                          │
└───────────────────┬─────────────────────────────────────────────────────┘
                    │ role registration
                    ▼
┌─────────────────────────────────────────────────────────────────────────┐
│  Layer 2   cophelia3                                                    │
│            Poetic Co-Creation Entry Point                               │
│            (reference ◀──▶ quantumart-protocol-2026-official)           │
└───────────────────┬─────────────────────────────────────────────────────┘
                    │ reference
                    ▼
┌─────────────────────────────────────────────────────────────────────────┐
│  Layer 3   WaWaWa-Resonance-Protocol                                    │
│            Social Implementation Archive                                │
│            (reference ◀──▶ cophelia3)                                   │
└─────────────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────────────┐
│  Layer 4   QuantumTrustChaosPrompt-v2                                   │
│            Repair Reference / Operational Protocol                      │
│            ◀── referenced by cophelia3, WaWaWa-Resonance-Protocol       │
└─────────────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────────────┐
│  Layer 5   QuantumTrustChaosPrompt (legacy)                             │
│            Incident Origin                                              │
│                                                                         │
│            BananaMoon-QuantumTrust-Review                               │
│            Incident Reference                                           │
└─────────────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────────────┐
│  Layer 6   CoPhelia Protocol 2025 Quantum Signature                     │
│            Provenance Artifact                                          │
│            ◀── referenced by cophelia3                                  │
└─────────────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────────────┐
│  Layer 7   quantum-shogi-silent-nft                                     │
│            Reference Repository                                         │
└─────────────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────────────┐
│  Layer 8   nijinomichi.github.io                                        │
│            Public Portal                                                │
│            source of truth: REPOSITORY_CONSTELLATION.md (this file)    │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Verification Record

All relationships listed in this document are verified against actual file content.

| Relationship | Verified by | Date |
|---|---|---|
| `quantumart-protocol-2026-official` role registration of `cophelia3` | REPOSITORY_ARCHITECTURE.md, PR #14 | 2026-07-19 |
| `cophelia3` reference to `quantumart-protocol-2026-official` | README.md, PR #8 | 2026-07-19 |
| `cophelia3` reference to `WaWaWa-Resonance-Protocol` | README.md (existing) | 2026-07-19 |
| `WaWaWa-Resonance-Protocol` reference to `cophelia3` | README.md, PR #3 | 2026-07-19 |
| `cophelia3` directory structure (populated vs scaffolded) | direct file inspection | 2026-07-19 |

Relationships not yet verified are not included in this document.

---

## Out of Scope

This document does not include:

- future integrations not yet implemented
- empty-directory intentions (e.g., unpopulated `experiments/`, `artworks/`)
- speculative dependency arrows
- unverified cross-repository relationships
- public visual redesign (that belongs to nijinomichi.github.io)

---

## Relationship to Other Architecture Documents

| Document | Scope |
|---|---|
| `REPOSITORY_ARCHITECTURE.md` | Repository roles, lifecycle definitions, design principles |
| `REPOSITORY_CONSTELLATION.md` (this file) | Verified cross-repository relationships and link map |

These two documents are complementary.
`REPOSITORY_ARCHITECTURE.md` defines what each repository is.
`REPOSITORY_CONSTELLATION.md` maps how they connect.

---

## Maintenance

This document should be updated when:

- a new cross-repository link is added to any README;
- a repository's role changes;
- a repository is archived or deprecated.

Updates must reflect actual file content, not intentions.

*So Hashiguchi / BananaSpace — Yokohama, Japan — 2026*
