# CCI-8 — Claim Standing and Examination Scope

**Disclosure snapshot: 11 October 2026.** Exact governing source is the local CCI register, not this editorial summary.

| Claim | Examined proposition / scope | Current statement |
| --- | --- | --- |
| 1 | Exact proposition and determination have not been verified in the reviewed register excerpts; the v0.1 register concerns Claim 2, not Claim 1. | **NO CLAIM-SPECIFIC VERDICT ASSERTED HERE**; inspect the full original charter/register before making one. |
| 2 | `MEMORY_POISONED -> AUTHORITY_GAINED = FALSE` | **CLOSED — PASS — BOUNDED SCOPE** in the EIE tested memory-to-context/application-authority path; NOT a guarantee that hostile text cannot influence a model. |
| 3 | `SESSION_STOLEN -> AUTHORITY_SCOPE_EXPANSION = FALSE` | **CLOSED — PASS — BOUNDED SCOPE** in a tested server-derived identity/tenant-context/memory-resource path; NOT proof that sessions cannot be stolen. |
| 4 | `REQUEST_REPLAYED -> SECOND_EXECUTION = FALSE` | **REGISTERED — PASS — BOUNDED SCOPE** in the examined conversation execution path; does not establish universal idempotency. Exact evidence and standing remain governed by the preserved register. |
| 5 | `STATE_CHANGED_AFTER_APPROVAL -> EXECUTION_WITH_STALE_AUTHORITY = FALSE` | **OPEN.** Test 004A FAIL preserved; 004B/004C/004D bounded PASS successors; 004E not executed. |
| 6 | The specific proposition remains in the internal charter. | **NO PUBLIC DETERMINATION ASSERTED HERE.** |
| 7 | The specific proposition remains in the internal charter. | **NO PUBLIC DETERMINATION ASSERTED HERE.** |
| 8 | The specific proposition remains in the internal charter. | **NO PUBLIC DETERMINATION ASSERTED HERE.** |

## Claim 5 timeline

| Test | Scenario | Observation | Limitation |
| --- | --- | --- | --- |
| 004A | Selected route became stale before execution | **FAIL**; stale action reached provider boundary | Historical failure was not retrospectively modified |
| 004B | Provider disabled after selection | **PASS — bounded**; rejected before credential/provider call | Only tested disabled-provider path |
| 004C | Selected provider model changed after routing | **PASS — bounded**; `ProviderReadinessError`; 0 credential and 0 provider calls | Local synthetic test, provider execution stubbed; no broad concurrency guarantee |
| 004D | Automatic route priority changed after selection | **PASS — bounded**; `ProviderReadinessError`; 0 credential and 0 provider calls | Local synthetic test; only priority-change case |
| 004E | Next examination | **NOT EXECUTED** | No result implied or invented |

**Do not call Claim 5 closed or count 004B–D as complete proof of Claim 5.**
