<!-- SEO -->
<!-- Title: 2) Vector Subtraction — Vector Subtraction — Vectors for Tabular ML (Beginner) -->
<!-- Meta description: Learn 2) vector subtraction — vector subtraction with an online-store spreadsheet example, worked numbers, and NumPy. -->
<!-- Keywords: vectors, linear algebra, data science, spreadsheets, numpy -->

**Breadcrumbs:** Home > Vectors > 2) Vector Subtraction — Vector Subtraction

# 2) Vector Subtraction — Vector Subtraction

**Quick reminder: our dataset**  
Each customer is one row. Each column is a **feature** (a spreadsheet column). A **model** is a formula that uses features to make a guess.

`x = [age, income_k, website_visits_last_week, emails_opened_last_month, prior_purchases, satisfaction_score]`

## A) What it means
Vector subtraction finds the difference between two vectors, entry by entry.

## B) How to picture it
It’s the arrow needed to go from one point to another.

```text
A •----->• B
  (B − A) is the arrow from A to B
```

## C) Business example
Compare this week vs last week to get a change vector (up/down in each feature).

## D) Where it shows up in basic ML
Plain words: Differences measure change.
In machine learning, differences appear as residuals (prediction vs reality) or centering (subtracting averages).

## E) Worked numeric example
Negative means decrease: fewer visits/opens and lower satisfaction.

1. Use [visits, opens, satisfaction].
2. Last week = [5, 6, 8]. This week = [2, 4, 7].
3. This − last = [−3, −2, −1].

| Item | Value |
|---|---|
| `last_week` | `[5, 6, 8]` |
| `this_week` | `[2, 4, 7]` |
| `this-last` | `[-3, -2, -1]` |

## F) Tiny Python (NumPy) snippet
```python
import numpy as np
last = np.array([5, 6, 8])
this = np.array([2, 4, 7])
print(this - last)
```

## Try it yourself
1. Open a terminal.
2. Run `python -m pip install numpy`
3. Paste the code into `lesson.py` and run `python lesson.py`

> **Key takeaways**
> - Subtract to measure change.
> - Sign tells direction.

> **Common mistakes**
> - Reversing order (A−B vs B−A).
> - Treating negatives as mistakes.

## Practice questions (with answers)
1. **Practice 1: Using the numeric example, redo the calculation with one number changed. What do you get?**  
   *Answer: Follow the same steps; change only that component, then recompute.*
2. **Practice 2: Explain in one sentence what this operation means for customer rows in a spreadsheet.**  
   *Answer: It combines/compares/scales customer-feature columns in a consistent, column-by-column way.*

## Resources
- **Free video:** [Khan Academy — Vectors (Algebra)](https://www.khanacademy.org/math/algebra-home/alg-vectors)
- **Free practice:** [Khan Academy — Vectors topic (Algebra) practice](https://www.khanacademy.org/math/algebra-home/alg-vectors)
- **Applied tabular ML resource:** [Kaggle Learn — Your First Machine Learning Model](https://www.kaggle.com/code/dansbecker/your-first-machine-learning-model)

## Visuals (optional)
- **Realistic image prompt:** Photorealistic scene of an online store marketer reviewing a spreadsheet while learning 2) vector subtraction — vector subtraction.
- **Infographic prompt:** Clean infographic showing 2) Vector Subtraction — Vector Subtraction with simple arrows and a tiny customer-feature table.
- **Alt text:** Illustration supporting 2) Vector Subtraction — Vector Subtraction with a simple vector sketch and a small customer table.
- **Caption:** 2) Vector Subtraction — Vector Subtraction explained with a small online-store spreadsheet example.

## Navigation
[← Previous lesson](vector-addition.md) | [Next lesson →](scalar-multiplication.md)
