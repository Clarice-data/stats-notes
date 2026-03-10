# Probability — Rules, Counting & Conditional

STA2023 | Unit 2

---

## The Big Idea
Probability = how likely something is to happen.

P(A) = favorable outcomes / total outcomes

Always between 0 (impossible) and 1 (certain).

---

## Complement Rule
If you know the probability something happens, you automatically know the probability it doesn't.

**P(A′) = 1 − P(A)**

> Example: If P(rain) = 0.3, then P(no rain) = 1 − 0.3 = 0.7

---

## Addition Rule — P(A OR B)

**Mutually exclusive** (can't both happen at same time):
P(A ∪ B) = P(A) + P(B)

**Not mutually exclusive** (can overlap):
P(A ∪ B) = P(A) + P(B) − P(A ∩ B)

> Why subtract? Because you'd count the overlap twice otherwise.

---

## Multiplication Rule — P(A AND B)

**Independent** (one doesn't affect the other):
P(A ∩ B) = P(A) × P(B)

**Dependent** (one affects the other):
P(A ∩ B) = P(A) × P(B | A)

---

## Conditional Probability — P(B | A)
"Given that A already happened, what's the probability of B?"

**P(B | A) = P(A ∩ B) / P(A)**

> Example: P(Ace | already drew a red card) — the sample space has changed.

---

## Counting Methods

**Factorial — n!**
Use when arranging ALL items in a line, order matters.
4! = 4 × 3 × 2 × 1 = 24

**Permutation — nPr**
Use when order MATTERS and you choose r from n.
nPr = n! / (n − r)!
> Example: How many ways to arrange 3 books from a shelf of 8? 8P3 = 336

**Combination — nCr**
Use when order does NOT matter.
nCr = n! / [r!(n − r)!]
> Example: How many ways to choose 3 people from a group of 8? 8C3 = 56

**Memory trick:** Permutation = PIN code (order matters). Combination = fruit salad (order doesn't matter).

---

## Common Mistakes
- Forgetting to subtract the overlap in the addition rule
- Using multiplication rule for OR problems (that's addition)
- Confusing permutation and combination — ask: does ORDER matter?
- Not updating the sample space for conditional probability

---
*STA2023 — Spring 2026*
