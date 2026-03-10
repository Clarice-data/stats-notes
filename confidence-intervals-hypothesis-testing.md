# Confidence Intervals & Hypothesis Testing

STA2023 | Unit 4 & 5

---

## PART 1: Confidence Intervals

A confidence interval gives a range of plausible values for an unknown population parameter.
Instead of saying "the mean is 50," you say "I'm 95% confident the mean is between 47 and 53."

**Structure:** Point Estimate ± Margin of Error

---

### CI for a Mean (σ known — use Z)
x̄ ± z* · (σ / √n)

### CI for a Mean (σ unknown — use t)
x̄ ± t* · (s / √n) — df = n − 1

> When to use Z vs t: If you know σ, use Z. If you only have s, use t. In real life, almost always t.

### CI for a Proportion
p̂ ± z* · √[ p̂(1 − p̂) / n ]
- Check conditions: np̂ ≥ 5 and n(1−p̂) ≥ 5

### Critical Values (z*)
| Confidence Level | z* |
|---|---|
| 90% | 1.645 |
| 95% | 1.96 |
| 99% | 2.576 |

### Margin of Error
E = z* · (σ / √n)

### Sample Size Formula
n = (z* · σ / E)² — always round UP

---

### Worked Example
Sample of 36 students, mean = 78, σ = 12. Build a 95% CI.
1. x̄ = 78, σ = 12, n = 36, z* = 1.96
2. E = 1.96 · (12 / √36) = 1.96 · 2 = 3.92
3. CI: 78 ± 3.92 → **(74.08, 81.92)**
4. Interpretation: "We are 95% confident the true mean is between 74.08 and 81.92."

---

## PART 2: Hypothesis Testing

We assume H₀ is true, then ask: is our sample data too unlikely if H₀ were true?
- If yes → reject H₀
- If no → fail to reject H₀ (never "accept" H₀)

---

### Setting Up Hypotheses
| Hypothesis | Symbol | Meaning |
|---|---|---|
| Null | H₀ | Status quo. Always has = |
| Alternative | H₁ | The claim being tested. Has ≠, <, or > |

**Tail direction:**
- H₁: μ ≠ value → two-tailed
- H₁: μ < value → left-tailed
- H₁: μ > value → right-tailed

---

### Step-by-Step Process
1. State H₀ and H₁
2. Set α (usually 0.05)
3. Calculate test statistic
4. Find p-value
5. Make decision: reject or fail to reject H₀
6. State conclusion in context

---

### Test Statistics
**Mean (σ known):** z = (x̄ − μ₀) / (σ / √n)

**Mean (σ unknown):** t = (x̄ − μ₀) / (s / √n), df = n − 1

**Proportion:** z = (p̂ − p₀) / √[ p₀(1−p₀) / n ]

---

### Decision Rules
**P-value method:**
- p-value ≤ α → Reject H₀
- p-value > α → Fail to Reject H₀

---

### Type I and Type II Errors
| | H₀ True | H₀ False |
|---|---|---|
| Reject H₀ | Type I Error (α) | Correct |
| Fail to Reject H₀ | Correct | Type II Error (β) |

- **Type I:** False positive — rejected H₀ but it was true
- **Type II:** False negative — kept H₀ but it was false

---

### Worked Example
Company claims average delivery = 5 days. Sample of 40: x̄ = 5.8, s = 2.1. Test at α = 0.05.
1. H₀: μ = 5 — H₁: μ ≠ 5 (two-tailed)
2. α = 0.05
3. t = (5.8 − 5) / (2.1 / √40) = 0.8 / 0.332 = **2.41**
4. df = 39, p-value ≈ 0.021
5. 0.021 < 0.05 → **Reject H₀**
6. Conclusion: Sufficient evidence that mean delivery time is not 5 days.

---

### Quick Reference
| Situation | Use |
|---|---|
| σ known, testing mean | Z-test |
| σ unknown, testing mean | T-test |
| Testing proportion | Z-test for proportion |
| Want a range for parameter | Confidence Interval |
| Testing a specific claim | Hypothesis Test |

---
*STA2023 — Spring 2026*
