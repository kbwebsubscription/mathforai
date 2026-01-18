<!-- SEO -->
<!-- Title: 6) Vector Equation of a Line — Vector Equation of a Line — Vectors for Tabular ML (Beginner) -->
<!-- Meta description: Learn 6) vector equation of a line — vector equation of a line with an online-store spreadsheet example, worked numbers, and NumPy. -->
<!-- Keywords: vectors, linear algebra, data science, spreadsheets, numpy -->

**Breadcrumbs:** Home > Vectors > 6) Vector Equation of a Line — Vector Equation of a Line

# 6) Vector Equation of a Line — Vector Equation of a Line

**Quick reminder: our dataset**  
Each customer is one row. Each column is a **feature** (a spreadsheet column). A **model** is a formula that uses features to make a guess.

`x = [age, income_k, website_visits_last_week, emails_opened_last_month, prior_purchases, satisfaction_score]`

## A) What it means
Line in vector form: x(t) = x0 + t·d (start at x0, move in direction d).

## B) How to picture it
Start point plus direction arrow; changing t slides along.

```text
x0 •-----> d
     •  •  •
```

## C) Business example
A customer profile gradually changes (more visits and opens over weeks). A line models that steady path.

## D) Where it shows up in basic ML
Plain words: Move inputs a little and see how a model’s score changes.
In machine learning, this is sensitivity analysis.

## E) Worked numeric example
As t grows, visits/opens rise steadily; satisfaction rises slowly.

1. Use x=[visits,opens,satisfaction].
2. x0=[2,1,6], d=[1,1,0.5].
3. x(0)=[2,1,6], x(1)=[3,2,6.5], x(2)=[4,3,7].

| Item | Value |
|---|---|
| `x0` | `[2, 1, 6]` |
| `d` | `[1, 1, 0.5]` |
| `x(0)` | `[2, 1, 6]` |
| `x(1)` | `[3, 2, 6.5]` |
| `x(2)` | `[4, 3, 7.0]` |

## F) Tiny Python (NumPy) snippet
```python
import numpy as np
x0 = np.array([2, 1, 6.0])
d = np.array([1, 1, 0.5])
for t in [0, 1, 2]:
    print(t, x0 + t*d)
```

## Try it yourself
1. Open a terminal.
2. Run `python -m pip install numpy`
3. Paste the code into `lesson.py` and run `python lesson.py`

> **Key takeaways**
> - Line = moving in one direction.
> - Great for what-if paths.

> **Common mistakes**
> - Forgetting t can be any real number.
> - Wrong feature order.

## Practice questions (with answers)
1. **Practice 1: Using the numeric example, redo the calculation with one number changed. What do you get?**  
   *Answer: Follow the same steps; change only that component, then recompute.*
2. **Practice 2: Explain in one sentence what this operation means for customer rows in a spreadsheet.**  
   *Answer: It combines/compares/scales customer-feature columns in a consistent, column-by-column way.*

## Resources
- **Free video:** [MIT OpenCourseWare — 18.06 Linear Algebra](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/)
- **Free practice:** [Paul's Online Notes — Equations of Lines (practice)](https://tutorial.math.lamar.edu/problems/calciii/EqnsOfLines.aspx)
- **Applied tabular ML resource:** [Kaggle Learn — Intro to Machine Learning](https://www.kaggle.com/learn/intro-to-machine-learning)

## Visuals (optional)
- **Realistic image prompt:** Photorealistic scene of an online store marketer reviewing a spreadsheet while learning 6) vector equation of a line — vector equation of a line.
- **Infographic prompt:** Clean infographic showing 6) Vector Equation of a Line — Vector Equation of a Line with simple arrows and a tiny customer-feature table.
- **Alt text:** Illustration supporting 6) Vector Equation of a Line — Vector Equation of a Line with a simple vector sketch and a small customer table.
- **Caption:** 6) Vector Equation of a Line — Vector Equation of a Line explained with a small online-store spreadsheet example.

## Navigation
[← Previous lesson](cross-product.md) | [Next lesson →](equation-of-a-plane.md)
