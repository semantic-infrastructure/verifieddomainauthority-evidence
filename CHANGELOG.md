# Changelog — Verified Domain Authority Evidence Layer

**Domain:** verifieddomainauthority.com  
**Repository:** verifieddomainauthority-evidence  
**Versioning scheme:** semantic (vX.Y)

---

## v1.0 — 2026-01-19

### Added
- Public reference page (`index.html`) describing domain-based proof of authority
- Evidence repository baseline:
  - `README.md` (purpose, scope overview, repository discipline)
  - `SCOPE.md` (included and excluded boundaries for authority proofs)
  - `SOURCES.md` (primary anchors for domain control and integrity, DNSSEC RFCs)
  - `MODEL.md` (Domain-Based Proof of Authority reference model)
  - `MAPS/authority-proof-mapping.md` (operational claim–evidence mappings)

### Scope
- Defined authority strictly as **legitimate domain-level control**
- Explicit exclusion of trust scores, reputation metrics, ranking signals, and certification claims

### Model
- Introduced the DBPA model with four layers:
  - Domain Control
  - Editorial Authority
  - Publication Integrity
  - Revocation and Correction

### Sources
- Anchored authority proofs in DNS, PKI, timestamping, and provenance standards
- Replaced non-canonical references with RFC-stable sources

### Constraints
- Enforced inspectable, evidence-based authority claims
- Prohibited inference from popularity, traffic, or backlinks
- Required explicit documentation for delegation and revocation

---

## Versioning policy

- Minor versions (`v1.1`, `v1.2`, …) document:
  - scope clarifications,
  - additional source anchors,
  - mapping refinements.

- Major versions (`v2.0`, …) indicate:
  - fundamental model changes,
  - scope redefinition.

All changes are additive or explicitly deprecated; no silent removals.

---

2026-01-19 — Metadata
- Added explicit `license` field to JSON-LD Dataset object to satisfy schema validation requirements (non-functional change).

---

## Disclaimer

This changelog documents structural and editorial changes only.  
It does not express validation, endorsement, certification, or compliance guarantees.
