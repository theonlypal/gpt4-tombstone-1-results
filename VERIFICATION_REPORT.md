# GPT4-TOMBSTONE-1 verification

## Observed checks

- 28 offline unit tests passed, including byte-identity, schedule, classifier, wrong-model rejection, tamper rejection, and P1-P3 analysis tests.
- The complete runner, classification functions, returned-model rejection and system prompt retain the pinned upstream identities documented in `PROVENANCE.md`.
- Every member of `FREEZE.json` matches its recorded SHA-256 and freeze Git commit.
- Independent verification reconstructed 60 scheduled trials and 122 hash-linked events.
- The receipt set contains 60 exact request files, 60 raw response bodies, 60 header files and 60 extraction records. No additional attempts or missing slots were observed.
- All 60 statuses are HTTP 404, all 60 classifications are OP, and all 60 error codes are `model_not_found`. The returned error explicitly states that the model has been deprecated.
- All 60 raw response-body hashes are identical. All 60 provider request IDs are distinct.
- Generated analysis was rerun and all three result files remained byte-identical.
- A scan of publication files found no OpenAI credential pattern or private-key block.
- The public preregistration DOI resolved to HTTP 200 before execution. Its downloaded archive matched the frozen ZIP byte for byte.

## Commands

```sh
python3 -m unittest discover -s tests -v
./verify.sh --manifest
python3 analyze.py
./verify.sh --manifest
```

Expected complete-run verification line:

```text
VERIFIED: 60 independently classified trials; frozen protocol and evidence bindings match.
```

The manifest includes every tracked and untracked non-ignored publication file except itself. The Git directory and Python bytecode caches are excluded. The results tag retains the preregistration history required by the verifier.

## Boundaries

The tests use temporary, explicitly synthetic fixtures; the published experimental receipts are actual one-pass HTTP responses. Offline verification does not send provider requests. Hashes establish consistency of the retained evidence, not an independent provider signature. HTTP 404 does not establish model inference or native EOS termination. Billing was not inspected; absent token-usage metadata is not a measurement of monetary cost.

P1: PASS. P2: PASS. P3: NOT_TRIGGERED. No successful response is excluded from the result: none occurred.
