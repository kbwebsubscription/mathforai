<!-- SEO -->
<!-- Title: 4) Dot Product — Dot Product — Vectors for Tabular ML (Beginner) -->
<!-- Meta description: Learn 4) dot product — dot product with an online-store spreadsheet example, worked numbers, and NumPy. -->
<!-- Keywords: vectors, linear algebra, data science, spreadsheets, numpy -->

**Breadcrumbs:** Home > Vectors > 4) Dot Product — Dot Product

# 4) Dot Product — Dot Product

**Quick reminder: our dataset**  
Each customer is one row. Each column is a **feature** (a spreadsheet column). A **model** is a formula that uses features to make a guess.

`x = [age, income_k, website_visits_last_week, emails_opened_last_month, prior_purchases, satisfaction_score]`

## A) What it means
Dot product multiplies matching entries and adds them up to get one score.

## B) How to picture it
A weighted scoring recipe.

```text
score = (w1*x1) + (w2*x2) + ...
```

## C) Business example
Use weights (importance) to compute a buy-after-email score: score = w·x.

## D) Where it shows up in basic ML
Plain words: A formula makes a score and then uses a threshold for yes/no.
In machine learning, this is a linear model using weights and a dot product.

## E) Worked numeric example
Compare the score to a threshold to decide likely vs unlikely.

1. x = [visits, opens, prior_purchases] = [3, 4, 2].
2. w = [0.4, 0.3, 0.8].
3. w·x = 0.4×3 + 0.3×4 + 0.8×2 = 4.0.

| Item | Value |
|---|---|
| `x` | `[3, 4, 2]` |
| `w` | `[0.4, 0.3, 0.8]` |
| `w·x` | `4.0` |

## F) Tiny Python (NumPy) snippet
```python
import numpy as np
x = np.array([3, 4, 2])
w = np.array([0.4, 0.3, 0.8])
print(np.dot(w, x))
```

## Try it yourself
1. Open a terminal.
2. Run `python -m pip install numpy`
3. Paste the code into `lesson.py` and run `python lesson.py`

> **Key takeaways**
> - Turns many features into one score.
> - Weights express importance.

> **Common mistakes**
> - Length mismatch.
> - Not scaling features first.

## Practice questions (with answers)
1. **Practice 1: Using the numeric example, redo the calculation with one number changed. What do you get?**  
   *Answer: Follow the same steps; change only that component, then recompute.*
2. **Practice 2: Explain in one sentence what this operation means for customer rows in a spreadsheet.**  
   *Answer: It combines/compares/scales customer-feature columns in a consistent, column-by-column way.*

## Resources
- **Free video:** [3Blue1Brown — Essence of Linear Algebra (playlist)](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)
- **Free practice:** [MIT OCW — Linear Algebra problem sets with solutions](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/resources/problem-sets-with-solutions/)
- **Applied tabular ML resource:** [scikit-learn — Linear Models (weights · features)](https://scikit-learn.org/stable/modules/linear_model.html)

## Visuals (optional)
- **Realistic image prompt:** Photorealistic scene of an online store marketer reviewing a spreadsheet while learning 4) dot product — dot product.
- **Infographic prompt:** Clean infographic showing 4) Dot Product — Dot Product with simple arrows and a tiny customer-feature table.
- **Alt text:** Illustration supporting 4) Dot Product — Dot Product with a simple vector sketch and a small customer table.
- **Caption:** 4) Dot Product — Dot Product explained with a small online-store spreadsheet example.

## Navigation
[← Previous lesson](scalar-multiplication.md) | [Next lesson →](cross-product.md)
