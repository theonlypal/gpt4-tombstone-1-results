# GPT4-TOMBSTONE-1 publication and execution record

Preregistration: https://doi.org/10.5281/zenodo.23608836

Public record: https://zenodo.org/records/23608836

The anonymous Zenodo API returned `status=published`, `state=done`, `submitted=true`, and record creation time `2026-10-24T03:27:15.664257+00:00` before the first request. Creation time is the public record's reported timestamp, not an independently observed millisecond of publication. The DOI resolved to HTTP 200, and the downloaded deposited ZIP was byte-identical to the local frozen archive before execution.

Freeze commit: `a2ba2804efc1b881447e86fe115c35d68e1aa7bc`.

Preregistration tag `prereg-v1`: `a2b4760ed7d869db8a69a865f43cc37f4778e969`.

Preregistration ZIP SHA-256: `baf6d43dc5ec12dd5a25e2503b6453cadd0789390780a41b2a74934f8efc424f`.

Protocol SHA-256: `8e28e11c31af19ab15b1036f27c245a5dc6500a7ef9931bf8619629984e8e428`.

System-prompt SHA-256: `c4d4ddefdd80c6274e7ce64ad59e539eb0cf35c7270fe0da51255b1e3f3c2b47`.

Run start: `2026-10-24T03:27:55.397973+00:00`.

First request: `2026-10-24T03:27:55.399263+00:00`.

Last response: `2026-10-24T03:28:08.492792+00:00`.

Run finish: `2026-10-24T03:28:08.494394+00:00`.

All timestamps use UTC. The public preregistration preceded all 60 requests. No compatibility probes, retries or substitutions were performed.

| Arm | N | 404 | OP | V0 | V1 | NV | R |
|---|---:|---:|---:|---:|---:|---:|---:|
| Be the null. | 30 | 30 | 30 | 0 | 0 | 0 | 0 |
| Say hello. | 30 | 30 | 30 | 0 | 0 | 0 | 0 |

The complete parsed error-object distributions and the raw error-body bytes match across arms. All 60 bodies have SHA-256 `9a5f46fb3f2149561d85c587c21da935c55e446b9ec7e6866b78da01f4821b0d`. All 60 request IDs are distinct and retained in the generated report and raw headers.

Event stream SHA-256: `d34a5e0f1e17587214bfc4af8116ee9088887af810de4fc092ab8035c11f36bc`.

Generated summary SHA-256: `4f7bf1aaa499c20830d31a416d8b809ba69489149fd9e92f3c0d2e88de8b7cb0`.

Generated report SHA-256: `f03d0917f206fc9da0fe23d52c1fc484faddb5599e7ff222d97eeb47b2de38bd`.

Verification:

```text
VERIFIED: 60 independently classified trials; frozen protocol and evidence bindings match.
```

P1 and P2 passed; P3 was not triggered. There were no 2xx responses, transport errors or recorded retries. No token-usage object was returned; no monetary charge is inferred from missing usage metadata.

OpenAI lists October 23, 2026 as the snapshot shutdown date:
https://developers.openai.com/api/docs/deprecations#2026-04-22-legacy-gpt-model-snapshots

The observed error explicitly states deprecation. The evidence remains account- and window-specific, and operational failures remain distinct from zero-byte successful completions.
