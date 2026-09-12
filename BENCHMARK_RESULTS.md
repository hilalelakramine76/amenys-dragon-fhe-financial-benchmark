
# AMENYS DRAGON AI — Benchmark Results

## Final Result

**1,000,000 encrypted financial records**

**Server-side encrypted computation: 9m06.595s**

**Final score: 2/2**

---

## Task 01 — Margin Quality

### Objective

Determine whether Product Line B exhibits a material deterioration
in gross-margin quality during the most recent 90-day period
relative to its historical baseline.

### Predefined threshold

300 basis points.

### Decrypted analytical output

| Metric | Result |
|---|---:|
| Historical gross margin | 39.003105% |
| Recent gross margin | 32.190442% |
| Deterioration | 681.266 bps |
| Materiality threshold | 300 bps |
| Result | **PASS** |

### Due-diligence interpretation

Product Line B experienced material late-period gross-margin
deterioration.

Historical margin performance should therefore not be annualised
blindly.

Pricing, procurement and supplier-cost drivers warrant further
investigation and forward EBITDA should be stress-tested.

---

## Task 02 — Cash Conversion

### Objective

Determine whether payment behaviour among Tier-1 customers
has materially deteriorated during the most recent 120-day period
relative to the historical baseline.

### Predefined threshold

10 days.

### Decrypted analytical output

| Metric | Result |
|---|---:|
| Historical average delay | 2.014500 days |
| Recent average delay | 18.147928 days |
| Deterioration | 16.133428 days |
| Materiality threshold | 10 days |
| Result | **PASS** |

### Due-diligence interpretation

Tier-1 payment behaviour materially deteriorated.

Working capital should therefore be normalised, collection risk
investigated and the NWC peg reviewed before underwriting future
cash generation.

---

# Score

| Task | Result |
|---|---:|
| Task 01 — Margin Quality | PASS |
| Task 02 — Cash Conversion | PASS |
| **Final Score** | **2/2** |

---

## Runtime

Server-side encrypted computation:

**9 minutes 06.595 seconds**

Measured using the operating system `time` command.

Client-side encryption was measured separately and is not included
in this server runtime.

---

## Confidentiality Condition

During server-side execution, the AMENYS server did not possess:

- the plaintext financial values
- the client secret decryption key
- the private ground truth

The final analytical results were decrypted client-side.
