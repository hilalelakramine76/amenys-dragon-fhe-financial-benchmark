
# Benchmark Scope and Limitations

This repository documents a specific AMENYS DRAGON AI encrypted
financial analytics experiment.

The benchmark produced a successful **2/2 score**, but its scope
should be interpreted precisely.

## What the benchmark demonstrates

The tested workflow successfully executed two predefined financial
analytical tasks over encrypted financial values:

1. detection of material gross-margin deterioration for Product Line B
2. detection of material deterioration in Tier-1 customer payment behaviour

The benchmark operated over a dataset containing 1,000,000 synthetic
financial records.

The corresponding client secret decryption key was not supplied to
the AMENYS server.

The private benchmark ground truth was not supplied to the AMENYS
server.

The measured server-side encrypted computation completed in
9m06.595s.

Both predefined tasks passed their respective materiality thresholds.

Final score:

**2/2**

## What the benchmark does not demonstrate

This experiment does not demonstrate that every possible financial
due-diligence procedure can be performed homomorphically.

It does not establish that every financial model or analytical
operation can be executed with the same runtime.

It does not constitute an independent cryptographic security audit.

It does not constitute an independently administered benchmark.

It does not establish superiority over every FHE implementation,
financial analytics platform, AI system, accounting firm or advisory
firm.

No DeepSeek, OpenAI, Big Four or other external system was executed
as a comparative control in this benchmark.

No claim of comparative superiority should therefore be inferred
from this repository.

## Dataset

The benchmark dataset is synthetic.

Its purpose is controlled experimental validation rather than the
representation of a real client engagement.

## Approximate Arithmetic

CKKS is an approximate-number homomorphic encryption scheme.

Small numerical approximation differences may therefore occur
relative to plaintext arithmetic.

The benchmark's primary outcome is based on predefined financial
materiality classifications rather than bit-for-bit numerical
identity.

## Independent Validation

The current benchmark was conducted and documented by AMENYS / its
founder.

External reproduction or independent third-party validation would
provide an additional level of assurance beyond the evidence
contained in this repository.

## Intellectual Property

This repository documents benchmark conditions and results.

It intentionally does not disclose proprietary AMENYS DRAGON
analytical architecture, confidential transformation logic,
internal decision methodology or other protected know-how.
