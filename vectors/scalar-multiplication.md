<!-- SEO -->
<!-- Title: 3) Scalar Multiplication — Scalar Multiplication — Vectors for Tabular ML (Beginner) -->
<!-- Meta description: Learn 3) scalar multiplication — scalar multiplication with an online-store spreadsheet example, worked numbers, and NumPy. -->
<!-- Keywords: vectors, linear algebra, data science, spreadsheets, numpy -->

**Breadcrumbs:** Home > Vectors > 3) Scalar Multiplication — Scalar Multiplication

# 3) Scalar Multiplication — Scalar Multiplication

**Quick reminder: our dataset**  
Each customer is one row. Each column is a **feature** (a spreadsheet column). A **model** is a formula that uses features to make a guess.

`x = [age, income_k, website_visits_last_week, emails_opened_last_month, prior_purchases, satisfaction_score]`

## A) What it means
Scalar multiplication multiplies every entry in a vector by the same number.

## B) How to picture it
Stretch/shrink an arrow: same direction, new length.

```text
v:  •--> 
  2v: •---->
```

## C) Business example
If an effect vector is ‘per 1 extra email’, then 3 extra emails means 3× that vector.

## D) Where it shows up in basic ML
Plain words: Scaling helps when units differ.
In machine learning, this is feature scaling (normalization/standardization).

## E) Worked numeric example
All components scale by the same factor.

1. Effect e = [0.5, 1, 0.2] on [visits, opens, satisfaction].
2. Compute 3e.
3. 3e = [1.5, 3, 0.6].

| Item | Value |
|---|---|
| `e` | `[0.5, 1.0, 0.2]` |
| `3*e` | `[1.5, 3.0, 0.6]` |

## F) Tiny Python (NumPy) snippet
```python
import numpy as np
e = np.array([0.5, 1.0, 0.2])
print(3 * e)
```

## Try it yourself
1. Open a terminal.
2. Run `python -m pip install numpy`
3. Paste the code into `lesson.py` and run `python lesson.py`

> **Key takeaways**
> - Multiply every component.
> - Direction stays the same.

> **Common mistakes**
> - Scaling only one component.
> - Forgetting units.

## Practice questions (with answers)
1. **Practice 1: Using the numeric example, redo the calculation with one number changed. What do you get?**  
   *Answer: Follow the same steps; change only that component, then recompute.*
2. **Practice 2: Explain in one sentence what this operation means for customer rows in a spreadsheet.**  
   *Answer: It combines/compares/scales customer-feature columns in a consistent, column-by-column way.*

## Resources
- **Free video:** [Khan Academy — Vectors (Precalculus) (scaling section)](https://www.khanacademy.org/math/precalculus/x9e81a4f98389efdf%3Avectors)
- **Free practice:** [Khan Academy — Scalar multiplication (practice)](https://www.khanacademy.org/math/precalculus/x9e81a4f98389efdf%3Avectors/x9e81a4f98389efdf%3Ascalar-mul/e/scaling_vectors)
- **Applied tabular ML resource:** [Kaggle Learn — Intro to Machine Learning](https://www.kaggle.com/learn/intro-to-machine-learning)

## Visuals (optional)
- **Realistic image prompt:** Photorealistic scene of an online store marketer reviewing a spreadsheet while learning 3) scalar multiplication — scalar multiplication.
- **Infographic prompt:** Clean infographic showing 3) Scalar Multiplication — Scalar Multiplication with simple arrows and a tiny customer-feature table.
- **Alt text:** Illustration supporting 3) Scalar Multiplication — Scalar Multiplication with a simple vector sketch and a small customer table.
- **Caption:** 3) Scalar Multiplication — Scalar Multiplication explained with a small online-store spreadsheet example.

## Navigation
[← Previous lesson](vector-subtraction.md) | [Next lesson →](dot-product.md)
