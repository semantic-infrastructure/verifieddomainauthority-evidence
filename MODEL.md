# Reference Model — Verified Domain Authority

**Model name:** Domain-Based Proof of Authority (DBPA)  
**Domain:** verifieddomainauthority.com  
**Repository:** verifieddomainauthority-evidence  
**Version:** v1.0  
**Last updated:** 2026-01-19

---

## Model intent

The DBPA model defines a **structural framework** for demonstrating
verifiable authority at the **domain level**.

It specifies how ownership, editorial control, publication integrity,
and revocation can be **proven through inspectable evidence**.

The model is non-evaluative and non-ranking.
It does not judge content quality or truthfulness.

---

## Model structure

### Layer 1 — Domain Control

**Domain control** establishes that an entity legitimately controls a domain.

Evidence types may include:
- Domain registration records
- DNS configuration and continuity
- TLS certificates and certificate transparency records

Constraints:
- Control must be attributable to a responsible entity
- Control signals must be inspectable
- Control does not imply endorsement or expertise

---

### Layer 2 — Editorial Authority

**Editorial authority** documents who is authorized to publish,
modify, and retract content under the domain.

Evidence types may include:
- Editorial policies
- Role assignments and delegation records
- Signed publication statements

Constraints:
- Authority must be explicitly assigned
- Individual authorship is subordinate to domain authority
- Changes to authority must be versioned

---

### Layer 3 — Publication Integrity

**Publication integrity** ensures that published artifacts
are protected against undocumented modification.

Evidence types may include:
- Timestamps and hashes
- Signed documents
- Append-only logs and changelogs

Constraints:
- All modifications must be recorded
- Silent changes are prohibited
- Integrity evidence must be time-bound

---

### Layer 4 — Revocation and Correction

**Revocation and correction** define how authority or publications
can be withdrawn or amended.

Evidence types may include:
- Revocation notices
- Correction records
- Supersession mappings

Constraints:
- Revocations must be explicit and reference prior artifacts
- Historical records are retained
- Revocation does not erase prior publication

---

## Relationships

The DBPA model enforces the following relationships:

- **Domain Control → Editorial Authority**  
  Only a controlling entity can assign editorial authority.

- **Editorial Authority → Publication Integrity**  
  Authorized publishers are accountable for integrity of artifacts.

- **Publication Integrity → Revocation and Correction**  
  Corrections and revocations operate on integrity-protected artifacts.

No reverse inference is permitted.

---

## Alignment with sources

The DBPA model is grounded in:
- DNS and domain control standards (RFC 1034, RFC 1035)
- Public key infrastructure and certificate transparency (RFC 5280, RFC 6962)
- Timestamping and integrity protocols (RFC 3161)
- Provenance and verifiable artifact models (W3C PROV, Verifiable Credentials)

Specific anchors are documented in `SOURCES.md`.

---

## Constraints

- No trust, reputation, or popularity scoring is defined
- No certification or compliance approval is implied
- No search or ranking signals are referenced
- The model documents structure only

---

## Change discipline

- Any modification to this model requires:
  - an explicit update to this file, and
  - a corresponding entry in `CHANGELOG.md`.

Deprecated model elements are documented and not removed silently.

---

## Disclaimer

This model defines a proof structure only.  
It does not provide legal advice, certification, or enforcement guarantees.
