# Elias CCI-8 — Cybersecurity Claims and Bounded Examination

**Elias Systems Ltd | Public examination-status disclosure | 11 October 2026**

CCI-8 is an eight-claim cybersecurity examination programme focused on how authority, tenant context, memory, request replay and execution eligibility behave under specified adverse conditions. This is a **record of bounded examinations**, not a claim of universal security or a production certification.

## Position as of 11 October 2026

| Item | Recorded public-facing position |
| --- | --- |
| Claim 1 | Exact standing not confirmed in the reviewed source records; no PASS or closure claimed here. |
| Claims 2–3 | CLOSED — PASS — BOUNDED SCOPE in their respective recorded paths. |
| Claim 4 | REGISTERED — PASS — BOUNDED SCOPE in the examined conversation execution path. |
| Claim 5 | **OPEN** — state changed after approval; stale authority must not cause execution. |
| Historical Test 004A | **FAIL** — preserved observed stale automatic-routing condition; stale execution reached the provider boundary before remediation. |
| Test 004B | **PASS — BOUNDED SCOPE** — disabled-provider successor scenario blocked before credential or provider call. |
| Test 004C | **PASS — BOUNDED SCOPE** — changed selected model after routing; stale execution rejected, zero credential/provider calls in the test. |
| Test 004D | **PASS — BOUNDED SCOPE** — changed automatic routing priority; stale candidate rejected, zero credential/provider calls in the test. |
| Test 004E | **PREPARATION ONLY — NOT EXECUTED** as of this disclosure. |
| Claims 6–8 | No disposition asserted in this release; further examination required. |

The Claim 5 tests examined particular automatic provider-routing decisions and committed state changes. They did **not** directly examine a literal approved `MemoryProposal` object or prove universal concurrency, fallback, or deployment-wide protection.

## Why the failure stays visible

004A remains FAIL even though later tests reported bounded passes. Changed code or later results do not rewrite the first observation. Evidence lineage and changed-condition authority are central to this publication.

## What this does NOT prove

No universal prevention of memory poisoning, session theft, prompt manipulation, replay across all endpoints, cross-tenant compromise, stale authority across all paths, or complete control-plane security is established. The programme is not an independent production penetration test or certification.

## How to inspect

Start with [the scoped claim-status table](CLAIM-STATUS.md), then [the evidence boundaries](EVIDENCE-BOUNDARIES.md). The underlying source records reside in the local CCI charter, tests, evidence, receipts, results and successor registers, which must be screened before any public inclusion. This README intentionally does **not** embed private app code or internal test data.

## Relationship to other Elias work

The LOVE Formula supplies an ethical foundation; EIE offers an application context for some of these tests; neither relationship independently certifies this security programme. [EASA](https://github.com/Eliassystems/Elias-Agentic-Security-Assurance) is a **different** examination and its results must not be attributed to CCI-8.

---

© 2026 Elias Systems Ltd. All rights reserved. Public availability of these documents does not grant a licence to protected formulas, proprietary software, trademarks or private implementation assets.
