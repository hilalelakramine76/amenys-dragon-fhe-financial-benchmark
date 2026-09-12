# AMENYS DRAGON AI — Encrypted Financial Due-Diligence Benchmark

**1,000,000 encrypted financial records.  
2/2 predefined due-diligence tasks.  
9m06.595s server-side encrypted computation.**

Created and led by **Hilal EL AKRAMINE**, Founder & CEO of **AMENYS**.

AMENYS DRAGON AI is an AMENYS financial analytics initiative focused on confidential financial computation.

---

## Benchmark result

| Metric | Result |
|---|---:|
| Financial records | 1,000,000 |
| Encryption scheme | CKKS |
| Server-side computation | 9m 06.595s |
| Task 01 — Margin Quality | PASS |
| Task 02 — Cash Conversion | PASS |
| Final score | **2 / 2** |

---

## Task 01 — Margin Quality

**Objective**

Determine whether Product Line B exhibits a material deterioration in gross-margin quality during the most recent 90-day period relative to its historical baseline.

**Predefined threshold**

300 basis points deterioration or more.

**Result**

- Baseline gross margin: **39.003105%**
- Recent gross margin: **32.190442%**
- Deterioration: **681.266 bps**
- Threshold: **300 bps**
- Result: **PASS**

---

## Task 02 — Cash Conversion

**Objective**

Determine whether payment behaviour among Tier-1 customers has materially deteriorated during the most recent 120-day period relative to the historical baseline.

**Predefined threshold**

10 days deterioration or more.

**Result**

- Baseline average delay: **2.014500 days**
- Recent average delay: **18.147928 days**
- Deterioration: **16.133428 days**
- Threshold: **10 days**
- Result: **PASS**

---

## Confidential computation model

The AMENYS server received:

- encrypted financial values
- approved structural metadata
- a public CKKS evaluation context

The AMENYS server did **not** receive:

- plaintext financial values
- the client secret decryption key
- the private ground truth

The encrypted analytical outputs were returned to the client and decrypted client-side.

---

## Cryptographic parameters

- Scheme: **CKKS**
- Library: **TenSEAL 0.3.16**
- Backend: **Microsoft SEAL**
- Polynomial modulus degree: **8192**
- Coefficient modulus bits: **[60, 40, 40, 60]**
- Global scale: **2^40**
- Packing capacity: **4096 slots per ciphertext**

See [`CRYPTO_PARAMETERS.md`](CRYPTO_PARAMETERS.md).

---

## Integrity and precommitment

The benchmark task definition was fixed before server execution.

**Task definition SHA-256**

`a4569b53dee6d7d36b484c6578421c3be0b1687cabac6a5152cda754d625784b`

**Encrypted transfer package SHA-256**

`371fff3f6d47b16037ac6a71b8557aee5f3cdf9e12c11c34f767ee700a32dec3`

See [`INTEGRITY_HASHES.txt`](INTEGRITY_HASHES.txt).

---

## Evidence

- [`TASK_DEFINITION.txt`](TASK_DEFINITION.txt)
- [`BENCHMARK_RESULTS.md`](BENCHMARK_RESULTS.md)
- [`CRYPTO_PARAMETERS.md`](CRYPTO_PARAMETERS.md)
- [`INTEGRITY_HASHES.txt`](INTEGRITY_HASHES.txt)
- [`LIMITATIONS.md`](LIMITATIONS.md)
- [`evidence/server_runtime.txt`](evidence/server_runtime.txt)
- [`evidence/resultats_taches_manifest.json`](evidence/resultats_taches_manifest.json)

---

## What this benchmark demonstrates

This benchmark demonstrates that the tested AMENYS DRAGON workflow successfully executed two predefined financial analytical tasks over encrypted financial values while the client retained the secret decryption key.

It demonstrates:

- 1,000,000 encrypted financial records processed
- 2 predefined financial due-diligence tasks
- 2 correct materiality classifications
- final score of **2/2**
- server-side encrypted computation completed in **9m06.595s**
- no client secret key provided to the AMENYS server

---

## What this benchmark does not claim

This benchmark does not claim that:

- every possible due-diligence task can be performed homomorphically
- AMENYS has been independently certified as the global FHE leader
- AMENYS has beaten every competing FHE platform
- DeepSeek or any other system was tested as a control in this benchmark

The purpose of this repository is to document a specific, reproducible encrypted financial analytics benchmark.

---

## AMENYS

**AMENYS — Confidential financial analytics for high-stakes decisions.**

Created and led by **Hilal EL AKRAMINE**.
