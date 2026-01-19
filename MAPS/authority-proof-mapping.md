# Authority Proof Mapping — Verified Domain Authority

**Domain:** verifieddomainauthority.com  
**Repository:** verifieddomainauthority-evidence  
**Reference model:** Domain-Based Proof of Authority (DBPA)  
**Version:** v1.0  
**Last updated:** 2026-01-19

---

## Purpose

This mapping operationalizes the DBPA model by defining **which evidence types
are permitted to substantiate which authority claims** at the domain level.

It serves as a consistency guardrail across scope, model, and sources.
No evaluation or sufficiency judgement is expressed.

---

## Authority claims (in scope)

- **Domain ownership claim**
- **Domain control claim**
- **Editorial authority claim**
- **Publication integrity claim**
- **Revocation or correction claim**

Claims outside this list are out of scope.

---

## Evidence categories (in scope)

- Domain registration records
- DNS configuration continuity
- TLS certificates and certificate transparency records
- Editorial policy documents
- Signed publication statements
- Timestamps, hashes, and signatures
- Append-only logs and changelogs
- Revocation or correction notices

---

## Claim–evidence mapping

| Authority claim                 | Permitted evidence types                                                                 | Notes |
|--------------------------------|------------------------------------------------------------------------------------------|-------|
| Domain ownership claim          | Registration record, DNS continuity                                                      | Registrant must be identifiable |
| Domain control claim            | DNS configuration, TLS certificate, CT record                                             | Control is technical, not reputational |
| Editorial authority claim       | Editorial policy, role assignment, signed statement                                       | Delegation must be explicit |
| Publication integrity claim    | Hash, timestamp, signature, changelog                                                     | Silent modification prohibited |
| Revocation / correction claim  | Revocation notice, correction record, supersession mapping                                | Prior artifact remains referenceable |

---

## Boundary constraints

- Authority claims **must be supported by inspectable evidence**.
- Evidence **does not imply** endorsement or content correctness.
- Domain-level authority **supersedes individual authorship claims**.
- Claims **must not** be inferred from popularity, traffic, or backlinks.

---

## Explicit exclusions

The following mappings are explicitly excluded:

- Authority inferred from search ranking
- Reputation or trust scores
- Social or network-based endorsement
- Implicit or unverifiable delegation

---

## Consistency rule

Any introduction of a new:
- authority claim, or
- evidence category

requires synchronized updates to:
- this file,
- `SCOPE.md`, and
- `CHANGELOG.md`.

---

## Disclaimer

This document defines allowed authority proof mappings only.  
It does not validate claims, certify domains, or confer endorsement.
