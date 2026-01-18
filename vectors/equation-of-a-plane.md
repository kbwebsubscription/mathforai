<!-- SEO -->
<!-- Title: 7) Equation of a Plane — Equation of a Plane — Vectors for Tabular ML (Beginner) -->
<!-- Meta description: Learn 7) equation of a plane — equation of a plane with an online-store spreadsheet example, worked numbers, and NumPy. -->
<!-- Keywords: vectors, linear algebra, data science, spreadsheets, numpy -->

**Breadcrumbs:** Home > Vectors > 7) Equation of a Plane — Equation of a Plane

# 7) Equation of a Plane — Equation of a Plane

**Quick reminder: our dataset**  
Each customer is one row. Each column is a **feature** (a spreadsheet column). A **model** is a formula that uses features to make a guess.

`x = [age, income_k, website_visits_last_week, emails_opened_last_month, prior_purchases, satisfaction_score]`

## A) What it means
A plane is all points satisfying a linear rule like w·x = b.

## B) How to picture it
A flat sheet; w is perpendicular (normal) to it.

```text
w ↑
  ---------
```

## C) Business example
Use a weighted score and a threshold to separate likely buyers vs unlikely.

## D) Where it shows up in basic ML
Plain words: One rule can separate two groups.
In machine learning, the separator is called a decision boundary.

## E) Worked numeric example
If score ≥ threshold, predict likely to buy.

1. x=[opens,prior_purchases,satisfaction]=[4,2,7].
2. w=[0.6,1.0,0.5], b=6.0.
3. w·x=7.9 ≥ 6.0 → likely.

| Item | Value |
|---|---|
| `x` | `[4, 2, 7]` |
| `w` | `[0.6, 1.0, 0.5]` |
| `b` | `6.0` |
| `w·x` | `7.9` |

## F) Tiny Python (NumPy) snippet
```python
import numpy as np
x = np.array([4, 2, 7])
w = np.array([0.6, 1.0, 0.5])
b = 6.0
print(np.dot(w, x), np.dot(w, x) >= b)
```

## Try it yourself
1. Open a terminal.
2. Run `python -m pip install numpy`
3. Paste the code into `lesson.py` and run `python lesson.py`

> **Key takeaways**
> - Plane = one linear rule.
> - Separates groups with a threshold.

> **Common mistakes**
> - Forgetting threshold b.
> - Thinking it’s only 3D (it generalizes).

## Practice questions (with answers)
1. **Practice 1: Using the numeric example, redo the calculation with one number changed. What do you get?**  
   *Answer: Follow the same steps; change only that component, then recompute.*
2. **Practice 2: Explain in one sentence what this operation means for customer rows in a spreadsheet.**  
   *Answer: It combines/compares/scales customer-feature columns in a consistent, column-by-column way.*

## Resources
- **Free video:** [MIT OpenCourseWare — 18.06 Linear Algebra](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/)
- **Free practice:** [Paul's Online Notes — Equations of Planes (practice)](https://tutorial.math.lamar.edu/problems/calcii/eqnsofplanes.aspx)
- **Applied tabular ML resource:** [Google ML Crash Course — Logistic Regression](https://developers.google.com/machine-learning/crash-course/logistic-regression)

## Visuals (optional)
- **Realistic image prompt:** Photorealistic scene of an online store marketer reviewing a spreadsheet while learning 7) equation of a plane — equation of a plane.
- **Infographic prompt:** Clean infographic showing 7) Equation of a Plane — Equation of a Plane with simple arrows and a tiny customer-feature table.
- **Alt text:** Illustration supporting 7) Equation of a Plane — Equation of a Plane with a simple vector sketch and a small customer table.
- **Caption:** 7) Equation of a Plane — Equation of a Plane explained with a small online-store spreadsheet example.

## Navigation
[← Previous lesson](vector-line-equation.md) | [Next lesson →](intersection-of-lines-3d.md)
