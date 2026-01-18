<!-- SEO -->
<!-- Title: 0) What is a vector — What is a vector — Vectors for Tabular ML (Beginner) -->
<!-- Meta description: Learn 0) what is a vector — what is a vector with an online-store spreadsheet example, worked numbers, and NumPy. -->
<!-- Keywords: vectors, linear algebra, data science, spreadsheets, numpy -->

**Breadcrumbs:** Home > Vectors > 0) What is a vector — What is a vector

# 0) What is a vector — What is a vector

**Quick reminder: our dataset**  
Each customer is one row. Each column is a **feature** (a spreadsheet column). A **model** is a formula that uses features to make a guess.

`x = [age, income_k, website_visits_last_week, emails_opened_last_month, prior_purchases, satisfaction_score]`

## A) What it means
A vector is an ordered list of numbers. In our spreadsheet, a customer’s feature values in one row form a vector.

## B) How to picture it
You can picture a vector as an arrow (direction + length) or as a neat row of numbers.

```text
start •-----> • end
```

## C) Business example
A customer row becomes a feature vector like:

x = [age, income_k, website_visits_last_week, emails_opened_last_month, prior_purchases, satisfaction_score]

This lets us do math with customer profiles instead of treating them as loose facts.

## D) Where it shows up in basic ML
Plain words: Turn each row into a vector so a formula can produce a score and make a guess.
In machine learning, this is called a feature vector (and the formula is a model).

## E) Worked numeric example
Customer A: age 30, income 60k, visits 3, opens 4, prior purchases 2, satisfaction 7/10.

1. Pick a customer’s feature values (small, interpretable numbers).
2. Write them in the agreed order of columns.
3. That ordered list is the vector.

| Item | Value |
|---|---|
| `x` | `[30, 60, 3, 4, 2, 7]` |

## F) Tiny Python (NumPy) snippet
```python
import numpy as np
x = np.array([30, 60, 3, 4, 2, 7])
print(x)
```

## Try it yourself
1. Open a terminal.
2. Run `python -m pip install numpy`
3. Paste the code into `lesson.py` and run `python lesson.py`

> **Key takeaways**
> - A vector is an ordered list of numbers.
> - A customer row = one feature vector.
> - Order matters.

> **Common mistakes**
> - Mixing up feature order.
> - Ignoring different units (age vs income).

## Practice questions (with answers)
1. **Practice 1: Using the numeric example, redo the calculation with one number changed. What do you get?**  
   *Answer: Follow the same steps; change only that component, then recompute.*
2. **Practice 2: Explain in one sentence what this operation means for customer rows in a spreadsheet.**  
   *Answer: It combines/compares/scales customer-feature columns in a consistent, column-by-column way.*

## Resources
- **Free video:** [Khan Academy — Vectors (Precalculus)](https://www.khanacademy.org/math/precalculus/x9e81a4f98389efdf%3Avectors)
- **Free practice:** [Khan Academy — Vectors practice (Precalculus)](https://www.khanacademy.org/math/precalculus/x9e81a4f98389efdf%3Avectors)
- **Applied tabular ML resource:** [Kaggle Learn — Intro to Machine Learning](https://www.kaggle.com/learn/intro-to-machine-learning)

## Visuals (optional)
- **Realistic image prompt:** Photorealistic scene of an online store marketer reviewing a spreadsheet while learning 0) what is a vector — what is a vector.
- **Infographic prompt:** Clean infographic showing 0) What is a vector — What is a vector with simple arrows and a tiny customer-feature table.
- **Alt text:** Illustration supporting 0) What is a vector — What is a vector with a simple vector sketch and a small customer table.
- **Caption:** 0) What is a vector — What is a vector explained with a small online-store spreadsheet example.

## Navigation
[Next lesson →](vector-addition.md)
