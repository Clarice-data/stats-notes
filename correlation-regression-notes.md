# Correlation & Regression

STA2023 | Unit 6

---

## Population vs. Sample Proportion

| | Notation | Example |
|---|---|---|
| Population proportion | p | 5/27 = 0.19 |
| Sample proportion (p-hat) | p̂ | 23/67 = 0.34 |

> Example: A store has 5 teddy bears out of every 27 stuffed animals (p = 0.19).
> A sample of 67 had 23 teddy bears (p̂ = 0.34).

---

## Correlation Coefficient — r

Measures the strength and direction of a linear relationship between two variables.

| r value | Strength |
|---|---|
| 1.00 | Perfect positive |
| 0.60–0.99 | Strong positive |
| 0.40–0.59 | Moderate positive |
| 0.20–0.39 | Weak positive |
| ~0.00 | No linear pattern |
| Negative values | Same scale, negative direction |

**Reading scatter plots:**
- r close to 1 → tight upward trend
- r close to −1 → tight downward trend
- r close to 0 → scattered, no clear pattern

---

## Permutations vs. Combinations (review)

Choosing 5 colors from 9, without replacement:

**Order matters → Permutation**
P(9, 5) = 9 × 8 × 7 × 6 × 5 = **15,120**

**Order doesn't matter → Combination**
C(9, 5) = 15,120 ÷ 120 = **126**

> Why divide by 120? Each group of 5 was counted 5! = 120 times in the permutation.

---

## Least-Squares Regression Line

**ŷ = b₀ + b₁x**

- b₁ (slope) = r · (sy / sx)
- b₀ (y-intercept) = ȳ − b₁x̄

**Using the equation:**
> Example: ŷ = 3.40 + 0.15x (predicting rental revenue from theater revenue)
> - Predicted value when x = 27.4: ŷ = 3.40 + 0.15(27.4) = **7.5 million**
> - Observed value at x = 27.4: **11.2 million**
> - Residual = observed − predicted = 11.2 − 7.5 = **3.7 million**

---

## Coefficient of Determination — r²

Proportion of variation in y that is explained by x.

> Example: r² = 0.81 means 81% of the variation in y is explained by x.

---
*STA2023 — Spring 2026*
