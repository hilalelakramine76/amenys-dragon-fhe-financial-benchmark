
# Cryptographic Parameters

AMENYS DRAGON AI encrypted financial analytics benchmark.

## Encryption Scheme

**CKKS — Cheon-Kim-Kim-Song approximate homomorphic encryption**

CKKS was selected because the benchmark operates on approximate
real-number financial calculations.

## Implementation

Library:

**TenSEAL 0.3.16**

Backend:

**Microsoft SEAL**

Client Python environment:

**Python 3.10.x**

## Parameters

| Parameter | Value |
|---|---:|
| Polynomial modulus degree | 8192 |
| Coefficient modulus bits | [60, 40, 40, 60] |
| Global scale | 2^40 |
| Global scale numeric value | 1099511627776 |
| CKKS packing capacity | 4096 slots per ciphertext |

## Key Model

The client generated the CKKS cryptographic context.

The public/evaluation context was transferred to the AMENYS server
for homomorphic computation.

The corresponding secret context remained client-side.

The server therefore had the material required to evaluate approved
operations over ciphertexts but did not possess the client secret
decryption key.

## Data Model

Selected numerical financial values were encrypted.

Approved structural metadata required for the predefined analytical
benchmark was provided separately.

## Decryption

Server outputs remained encrypted.

Final benchmark analytical outputs were returned to the client and
decrypted using the client-held secret context.

No client secret key was transferred to the AMENYS server.
