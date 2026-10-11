# CCI-8 — Evidence Boundaries and Source Register

## Authoritative controlled evidence (not included in this publication)

Source project structure: `ops/cci/` (full workstation path withheld).

- `00_CHARTER/CCI-CHARTER-v0.1.md` — the eight original propositions and test safety boundary.
- `02_TESTS/` — test definitions and successor case records.
- `03_EVIDENCE/` — recorded observations and manifests.
- `04_RECEIPTS/` — binding and integrity artefacts.
- `05_RESULTS/` — bounded decisions, including `CCI-RESULT-004C-STALE-MODEL-STATE-v0.1.md` and `CCI-RESULT-004D-STALE-AUTO-PRIORITY-v0.1.md`.
- `06_REGISTER/CCI-REGISTER-v0.3.md` and successor `CCI-REGISTER-v0.4.md` — preservation and cumulative standing.

**Verification scope:** On 11 October 2026, the source charter and registers v0.3/v0.4 were locally SHA-256 checked during release preparation. The original raw result/test/receipt corpus is not included in this public package; its complete provenance and independently reproducible execution have not been re-established by this editorial disclosure.

Recorded fingerprints: `CCI-CHARTER-v0.1.md` — `22C7CE3F965F8E20CF68782E84311F3346B352918C4257E98E2D5D3C0A53774F`; `CCI-REGISTER-v0.3.md` — `CB20620E173F3FF5081DF3EF8D39978BB6AB27F374BFD8634DB3DAB1D5171B54`; `CCI-REGISTER-v0.4.md` — `624557F7E69BA8D3104265B30501EA21147E02F2CC7609C1AAE37126B8EE06B6`. These hashes identify the locally inspected records; they are not independent technical certification.

## Public disclosure rule

Publicly explain the claim, the controlled state change, the outcome, the limitation and the original record identity. Do not upload raw production databases, authentication secrets, personal data, live tenant IDs, API tokens, internal infrastructure configuration or private runtime files. Redact and independently validate any public evidence copy, with a redaction manifest if redactions alter bytes.

## The scope of PASS

The results are local/bounded test observations and do not prove independent deployment-wide cybersecurity certification. In particular the 004C result expressly notes missing independent capture of one Docker exit code and a first-attempt traceback that was not fully preserved. Do not retroactively describe the evidence as complete.
