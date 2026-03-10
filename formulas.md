# STA2023 Formula Reference

Master formulas reference for Elementary Statistics — updated as course progresses.

---

## Unit 1 — Descriptive Statistics

**Mean**
- Population: μ = Σx / N
- Sample: x̄ = Σx / n

**Standard Deviation**
- Population: σ = √[ Σ(x − μ)² / N ]
- Sample: s = √[ Σ(x − x̄)² / (n − 1) ]

**Variance**
- Population: σ² = Σ(x − μ)² / N
- Sample: s² = Σ(x − x̄)² / (n − 1)

**Five-Number Summary**
Min → Q1 → Median (Q2) → Q3 → Max

**IQR:** Q3 − Q1

**Outlier Fences**
- Lower: Q1 − 1.5(IQR)
- Upper: Q3 + 1.5(IQR)

**Z-Score**
- z = (x − μ) / σ  ← population
- z = (x − x̄) / s ← sample

---

## Unit 2 — Probability

**Basic:** P(A) = favorable outcomes / total outcomes

**Complement:** P(A′) = 1 − P(A)

**Addition Rule**
- Mutually exclusive: P(A ∪ B) = P(A) + P(B)
- General: P(A ∪ B) = P(A) + P(B) − P(A ∩ B)

**Multiplication Rule**
- Independent: P(A ∩ B) = P(A) × P(B)
- Dependent: P(A ∩ B) = P(A) × P(B | A)

**Conditional:** P(B | A) = P(A ∩ B) / P(A)

**Counting Methods**
| Method | Formula | When |
|---|---|---|
| Factorial | n! | Arrange ALL n items |
| Permutation | nPr = n! / (n−r)! | Order matters |
| Combination | nCr = n! / [r!(n−r)!] | Order doesn't matter |

---

## Unit 3 — Random Variables & Distributions

**Expected Value:** μ = E(X) = Σ [ x · P(x) ]

**Variance:** σ² = Σ [ (x − μ)² · P(x) ]

**Standard Deviation:** σ = √[ Σ (x − μ)² · P(x) ]

**Binomial Distribution**
Use when: fixed trials, two outcomes, constant probability, independent trials.

| Formula | What it gives |
|---|---|
| P(X = k) = nCk · pᵏ · (1−p)^(n−k) | Probability of exactly k successes |
| μ = np | Mean |
| σ² = np(1−p) | Variance |
| σ = √[np(1−p)] | Standard deviation |

**Normal Distribution**
- 68% within 1σ, 95% within 2σ, 99.7% within 3σ
- Convert to Z: z = (x − μ) / σ

---

## Unit 4 — Confidence Intervals

**Mean (σ known):** x̄ ± z* · (σ / √n)

**Mean (σ unknown):** x̄ ± t* · (s / √n)  — df = n − 1

**Proportion:** p̂ ± z* · √[ p̂(1 − p̂) / n ]

**Margin of Error:** E = z* · (σ / √n)

**Sample Size:** n = (z* · σ / E)²  — always round UP

| Confidence Level | z* |
|---|---|
| 90% | 1.645 |
| 95% | 1.96 |
| 99% | 2.576 |

---

## Unit 5 — Hypothesis Testin
