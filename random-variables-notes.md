# Random Variables & Distributions

STA2023 | Unit 3

---

## What is a Random Variable?
A random variable (X) is a variable whose value is the numerical outcome of a random event.

- **Discrete:** countable outcomes (0, 1, 2, 3...) — like number of heads
- **Continuous:** any value in a range — like height or weight

---

## Probability Distribution
A table or formula showing every possible value of X and its probability.

**Rules every probability distribution must follow:**
1. Every P(x) must be between 0 and 1
2. All P(x) values must sum to exactly 1

| x | P(x) |
|---|---|
| 0 | 0.20 |
| 1 | 0.45 |
| 2 | 0.30 |
| 3 | 0.05 |
| **Total** | **1.00** |

---

## Expected Value — E(X)
The mean of the distribution. What you'd expect on average over many trials.

**μ = E(X) = Σ [ x · P(x) ]**

Using the table above:
μ = (0)(0.20) + (1)(0.45) + (2)(0.30) + (3)(0.05) = **1.20**

---

## Standard Deviation of a Distribution
σ = √[ Σ (x − μ)² · P(x) ]

Steps:
1. Find μ (expected value)
2. For each x: calculate (x − μ)²
3. Multiply each by P(x)
4. Sum them all → that's σ²
5. Take the square root → that's σ

---

## Binomial Distribution
Use binomial when ALL FOUR conditions are met:
1. **Fixed** number of trials (n)
2. Only **two outcomes**: success or failure
3. **Constant** probability of success (p) each trial
4. Trials are **independent**

**Formula:** P(X = k) = ₙCₖ · pᵏ · (1−p)^(n−k)

**Mean & Standard Deviation:**
- μ = np
- σ = √[np(1−p)]

> Example: Flip a fair coin 10 times. P(exactly 6 heads)?
> n=10, k=6, p=0.5
> P(X=6) = ₁₀C₆ · (0.5)⁶ · (0.5)⁴ = **0.2051**

---

## Normal Distribution
Bell-shaped and symmetric. Described by μ (center) and σ (spread).

**Empirical Rule (68-95-99.7):**
- 68% of data within μ ± 1σ
- 95% of data within μ ± 2σ
- 99.7% of data within μ ± 3σ

**Converting to Z-score:** z = (x − μ) / σ

**Reading the Z-table:**
- Table gives area to the LEFT of z
- P(X < value) → look up z directly
- P(X > value) → 1 − table value
- P(a < X < b) → table(z_b) − table(z_a)

---

## Discrete vs. Continuous at a Glance

| Feature | Discrete | Continuous (Normal) |
|---|---|---|
| Values | Countable (0,1,2...) | Any real number in range |
| Distribution | Probability table | Bell curve |
| Find exact P(x) | Yes | No — find P(a < X < b) |
| Key formula | Binomial or table | Z-score + Z-table |

---

## Practice Problems
1. Is X = number of siblings discrete or continuous?
2. A distribution: P(0)=0.1, P(1)=0.4, P(2)=0.3, P(3)=0.2. Find E(X).
3. A test has 8 true/false questions. If guessing (p=0.5), find P(exactly 5 correct).
4. For the same test, find the mean and standard deviation of correct guesses.
5. Heights are normally distributed: μ=65in, σ=3in. What % of people are between 62 and 68 inches?

---
*STA2023 — Spring 2026*
