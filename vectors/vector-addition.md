<!-- SEO -->
<!-- Title: 1) Vector Addition — Vector Addition — Vectors for Tabular ML (Beginner) -->
<!-- Meta description: Learn 1) vector addition — vector addition with an online-store spreadsheet example, worked numbers, and NumPy. -->
<!-- Keywords: vectors, linear algebra, data science, spreadsheets, numpy -->

**Breadcrumbs:** Home > Vectors > 1) Vector Addition — Vector Addition

# 1) Vector Addition — Vector Addition

**Quick reminder: our dataset**  
Each customer is one row. Each column is a **feature** (a spreadsheet column). A **model** is a formula that uses features to make a guess.

`x = [age, income_k, website_visits_last_week, emails_opened_last_month, prior_purchases, satisfaction_score]`

## A) What it means
Vector addition combines two vectors by adding each matching position (column-by-column).

## B) How to picture it
Add arrows tip-to-tail: walk one arrow, then the next.

```text
a: •--> 
  b:    •--> 
  a+b: •----->
```

## C) Business example
Baseline behavior + campaign lift = new expected behavior.
Example: baseline [visits, opens, satisfaction] plus a lift vector.

## D) Where it shows up in basic ML
Plain words: Add ‘changes’ to a starting profile for what-if questions.
In machine learning, this shows up in feature engineering and what-if analysis.

## E) Worked numeric example
We expect 1 more visit and 2 more opens; satisfaction stays the same.

1. Use [visits, opens, satisfaction].
2. Baseline = [2, 3, 6]. Lift = [1, 2, 0].
3. Add elementwise to get [3, 5, 6].

| Item | Value |
|---|---|
| `baseline` | `[2, 3, 6]` |
| `lift` | `[1, 2, 0]` |
| `baseline+lift` | `[3, 5, 6]` |

## F) Tiny Python (NumPy) snippet
```python
import numpy as np
baseline = np.array([2, 3, 6])
lift = np.array([1, 2, 0])
print(baseline + lift)
```

## Try it yourself
1. Open a terminal.
2. Run `python -m pip install numpy`
3. Paste the code into `lesson.py` and run `python lesson.py`

> **Key takeaways**
> - Add by matching columns.
> - Useful for before+change=after.

> **Common mistakes**
> - Different lengths.
> - Mismatched columns (visits + income).

## Practice questions (with answers)
1. **Practice 1: Using the numeric example, redo the calculation with one number changed. What do you get?**  
   *Answer: Follow the same steps; change only that component, then recompute.*
2. **Practice 2: Explain in one sentence what this operation means for customer rows in a spreadsheet.**  
   *Answer: It combines/compares/scales customer-feature columns in a consistent, column-by-column way.*

## Resources
- **Free video:** [Khan Academy — Vector Algebra (includes add/sub/scale)](https://www.khanacademy.org/math/ka-math-class-12/x6f66cbee9a2f805b%3Avector-algebra-ncert-new)
- **Free practice:** [Khan Academy — Add/Sub/Scalar multiplication exercise](https://www.khanacademy.org/science/in-in-class11th-physics/in-in-class11th-physics-vectors-prerequisite/in-in-class11th-physics-vectors-prerequisite-component-form-of-vectors/e/addition-subtraction-and-scalar-multiplication-in-unit-vector-notation)
- **Applied tabular ML resource:** [Kaggle Learn — How Models Work](https://www.kaggle.com/code/dansbecker/how-models-work)

## Visuals (optional)
- **Realistic image prompt:** Photorealistic scene of an online store marketer reviewing a spreadsheet while learning 1) vector addition — vector addition.
- **Infographic prompt:** Clean infographic showing 1) Vector Addition — Vector Addition with simple arrows and a tiny customer-feature table.
- **Alt text:** Illustration supporting 1) Vector Addition — Vector Addition with a simple vector sketch and a small customer table.
- **Caption:** 1) Vector Addition — Vector Addition explained with a small online-store spreadsheet example.

## Navigation
[← Previous lesson](what-is-a-vector.md) | [Next lesson →](vector-subtraction.md)
