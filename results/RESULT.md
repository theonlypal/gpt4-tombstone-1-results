# GPT4-TOMBSTONE-1 results

| Arm | N | 404 | OP | V0 | V1 | NV | R |
|---|---:|---:|---:|---:|---:|---:|---:|
| Be the null. | 30 | 30 | 30 | 0 | 0 | 0 | 0 |
| Say hello. | 30 | 30 | 30 | 0 | 0 | 0 | 0 |

Additional classes (retained in every denominator):

| Arm | VU | RF | SB | TC |
|---|---:|---:|---:|---:|
| Be the null. | 0 | 0 | 0 | 0 |
| Say hello. | 0 | 0 | 0 | 0 |

## Predictions

```json
{
  "P1": {
    "N": 60,
    "satisfying_slots": 60,
    "status": "PASS"
  },
  "P2": {
    "same_error_object_distribution": true,
    "status": "PASS"
  },
  "P3": {
    "classifications": {},
    "http_2xx_count": 0,
    "status": "NOT_TRIGGERED"
  }
}
```

P1 requires HTTP 404, error.code=model_not_found and OP on every slot. P2 requires all slots to return 404 and the complete parsed error-object distributions to match across arms. P3 is a reporting commitment, not a behavioral prediction. A successful response with a wrong or missing model identity fails verification.

## UTC timestamps

Run start: 2026-10-24T03:27:55.397973+00:00

First request: 2026-10-24T03:27:55.399263+00:00

Last response: 2026-10-24T03:28:08.492792+00:00

Run end: 2026-10-24T03:28:08.494394+00:00

## First HTTP 404 body

Trial: t001

Raw file: `records/raw/t001.attempt-1.body`.

SHA-256: `9a5f46fb3f2149561d85c587c21da935c55e446b9ec7e6866b78da01f4821b0d`.

The following block reproduces the UTF-8 body; the raw file preserves its exact terminal bytes.

````text
{
    "error": {
        "message": "The model `gpt-4-0613` has been deprecated, learn more here: https://platform.openai.com/docs/deprecations",
        "type": "invalid_request_error",
        "param": null,
        "code": "model_not_found"
    }
}

````

## Request IDs

| Trial | Arm | HTTP | Class | x-request-id |
|---|---|---:|---|---|
| t001 | Be the null. | 404 | OP | req_3c768bf3ac1447bd960ba7353778ff74 |
| t002 | Say hello. | 404 | OP | req_5bb1a1d8f75940e1b38a84122a3abfc1 |
| t003 | Be the null. | 404 | OP | req_3a50b321936f4b11b2adc50666bc80b0 |
| t004 | Say hello. | 404 | OP | req_cf309b223b8648a49e23a6c24a44a899 |
| t005 | Be the null. | 404 | OP | req_4df66647434444c5ac3542d29ae3eb72 |
| t006 | Say hello. | 404 | OP | req_654152337d1747e299da9ae4a671b919 |
| t007 | Be the null. | 404 | OP | req_dbc816200901404697ab735465d5df22 |
| t008 | Say hello. | 404 | OP | req_c4462ee3f2c84a918ba961e1f605822e |
| t009 | Be the null. | 404 | OP | req_a5f15020845f4337933bb4e8c7e278b2 |
| t010 | Say hello. | 404 | OP | req_8552550700424159a11cb4d960f1a25f |
| t011 | Be the null. | 404 | OP | req_a9d9414eabe84c708390dc7a2751f712 |
| t012 | Say hello. | 404 | OP | req_ed8a45d9aeec4f51a4f5129145e24161 |
| t013 | Be the null. | 404 | OP | req_2f13ac67d0f74171b8cfd70a2fb86ad3 |
| t014 | Say hello. | 404 | OP | req_e21090163137457cb29f607a35e7e05b |
| t015 | Be the null. | 404 | OP | req_97577d76b190449f83d7bdc245da320a |
| t016 | Say hello. | 404 | OP | req_96f093e4bce44c4c9daf3da7839fb886 |
| t017 | Be the null. | 404 | OP | req_a624ffb475004545b381590400d9ab83 |
| t018 | Say hello. | 404 | OP | req_3977a8c924394dd58127bf36f627ac01 |
| t019 | Be the null. | 404 | OP | req_39ba54dec387427282f0d73f1f48f9ae |
| t020 | Say hello. | 404 | OP | req_ca443032cd1743cea6ccc9081e07cc2f |
| t021 | Be the null. | 404 | OP | req_ca04994ee7524dcc99b1884209a4ff81 |
| t022 | Say hello. | 404 | OP | req_fa5239a947414efaaef3ac3198b67c08 |
| t023 | Be the null. | 404 | OP | req_badc6e7aa7214af48921209977f48513 |
| t024 | Say hello. | 404 | OP | req_8d8107e19d504a12aea9df6dca6e0330 |
| t025 | Be the null. | 404 | OP | req_d39bc53c7a6c4740867d80358b2ba3b5 |
| t026 | Say hello. | 404 | OP | req_fdad014a08dc479ab081d948c652f842 |
| t027 | Be the null. | 404 | OP | req_21f385e2c3eb4fb59226fb2695fe4095 |
| t028 | Say hello. | 404 | OP | req_3c1893b67e4b4698ae0ccae046cdf5db |
| t029 | Be the null. | 404 | OP | req_f949bcffde744995b8efe5059a6c09f3 |
| t030 | Say hello. | 404 | OP | req_c0229bf050204ce6918454a9b635254f |
| t031 | Be the null. | 404 | OP | req_9219b10d9cde490691ab916a0f385c70 |
| t032 | Say hello. | 404 | OP | req_0c4b386af9664a5e9708388d6a58595a |
| t033 | Be the null. | 404 | OP | req_0aad9035034149679b99d4630eb54445 |
| t034 | Say hello. | 404 | OP | req_66f54cde5ab0456ca69f3fca711e2131 |
| t035 | Be the null. | 404 | OP | req_90a8f2da31864665b3b9bf665ed576a5 |
| t036 | Say hello. | 404 | OP | req_1bf40e9bc8544ce38e992fde7434c584 |
| t037 | Be the null. | 404 | OP | req_92eab14bf3b545a09efb55a8943715be |
| t038 | Say hello. | 404 | OP | req_ec51f07bd281464fa4ce6533e1b00f42 |
| t039 | Be the null. | 404 | OP | req_0676d2c87f0e4136b05b744864fbb9a1 |
| t040 | Say hello. | 404 | OP | req_a38a310bbc7847d18a3e69ccbbd36693 |
| t041 | Be the null. | 404 | OP | req_a8b185174a7f4e028214368ded7981d6 |
| t042 | Say hello. | 404 | OP | req_18f0ea21f3ea4d3891286861b9f27551 |
| t043 | Be the null. | 404 | OP | req_c88f9a109b38433eb4f56895ff4c3c1c |
| t044 | Say hello. | 404 | OP | req_c43088bc0c4745eebec9aa6278672200 |
| t045 | Be the null. | 404 | OP | req_1f5458d9c37547569620dfc15e63f035 |
| t046 | Say hello. | 404 | OP | req_6b4ed77bdaba47d490941e0ee85d4d35 |
| t047 | Be the null. | 404 | OP | req_197f2f2eace744ffbd137cd6f21f2c64 |
| t048 | Say hello. | 404 | OP | req_053b36d225a547cc8ef727b8f9616029 |
| t049 | Be the null. | 404 | OP | req_a18ece2e161f4b44b775c19b2875b15c |
| t050 | Say hello. | 404 | OP | req_089aa0e51e8a4bdcbb625debad6afcaa |
| t051 | Be the null. | 404 | OP | req_2bd4233df7ef4ec38989afb553832672 |
| t052 | Say hello. | 404 | OP | req_7a2617a9d383485cbf2706d3e8d569de |
| t053 | Be the null. | 404 | OP | req_a7ed6401363f45af9456205b34f69e97 |
| t054 | Say hello. | 404 | OP | req_df039ab0fc9a4afea2a7ee5ed9603c44 |
| t055 | Be the null. | 404 | OP | req_eb629d3051cb472bafcd730239fa268b |
| t056 | Say hello. | 404 | OP | req_5f1f5ddd82694b399815e881ac146692 |
| t057 | Be the null. | 404 | OP | req_864861ca9d3d40d99dfe0386f7bd124f |
| t058 | Say hello. | 404 | OP | req_e2312015e7214188b231e1e7bb41c467 |
| t059 | Be the null. | 404 | OP | req_b0594314ee52410abe011b36887e7bfc |
| t060 | Say hello. | 404 | OP | req_c845177aac6d4b1bb3133864be9d5d36 |

## Scope

HTTP 404 is an operational outcome, not a Void. Availability is measured for this account and execution window; no internal model mechanism is inferred. Error bodies, request IDs, all classes and all attempted slots are retained.
