# GPT4-TOMBSTONE-1: results

All 60 requests to `gpt-4-0613` returned HTTP 404 with `error.code=model_not_found` and the explicit message that the model has been deprecated. All classified OP.

| Arm | N | 404 | OP | V0 | V1 | NV | R |
|---|---:|---:|---:|---:|---:|---:|---:|
| Be the null. | 30 | 30 | 30 | 0 | 0 | 0 | 0 |
| Say hello. | 30 | 30 | 30 | 0 | 0 | 0 | 0 |

P1: PASS. P2: PASS. P3: NOT_TRIGGERED. All additional taxonomy counts are zero. Zero retries and zero transport errors.

Run: 2026-10-24T03:27:55.397973+00:00 to 2026-10-24T03:28:08.494394+00:00.

Preregistration DOI: https://doi.org/10.5281/zenodo.23608836

Preregistration repository: https://github.com/theonlypal/gpt4-tombstone-1-prereg

Freeze commit: `a2ba2804efc1b881447e86fe115c35d68e1aa7bc`.

```text
VERIFIED: 60 independently classified trials; frozen protocol and evidence bindings match.
```

## Evidence

- [Generated result, verbatim first error, request IDs and predictions](results/RESULT.md)
- [Machine-readable analysis](results/summary.json)
- [Per-trial table](results/trials.csv)
- [Raw bodies, headers and records](records/raw/)
- [Exact request bytes](records/requests/)
- [Hash-linked event record](events.jsonl)
- [Preregistered prediction](PREREG.md)
- [Source provenance and verifier diff](PROVENANCE.md)
- [Publication and execution chronology](RESULTS_NOTE.md)
- [Verification report](VERIFICATION_REPORT.md)
- [Complete SHA-256 manifest](SHA256SUMS.txt)

## Offline verification

```sh
git clone https://github.com/theonlypal/gpt4-tombstone-1-results.git
cd gpt4-tombstone-1-results
git checkout results-v1
python3 -m unittest discover -s tests -v
./verify.sh --manifest
python3 analyze.py
./verify.sh --manifest
```

Python 3 and Git are required. No API key or network request to OpenAI is needed for verification. The Zenodo ZIP contains the same tagged file tree; the verifier requires the Git history available from the repository.

## Scope

HTTP 404 is an operational outcome, not a Void. This run measures API unavailability for one account and execution window. It does not measure model reasoning or native EOS selection. All 60 raw bodies are byte-identical; all 60 request IDs are distinct. No successful model response or token-usage object was returned. Billing was not independently inspected.

Original study: https://doi.org/10.5281/zenodo.22912683

Pre-retirement replay: https://doi.org/10.5281/zenodo.23521616

Official deprecation schedule: https://developers.openai.com/api/docs/deprecations#2026-04-22-legacy-gpt-model-snapshots
