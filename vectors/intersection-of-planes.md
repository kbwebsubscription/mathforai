<!-- SEO -->
<!-- Title: 9) Intersection of Planes — Intersection of Planes — Vectors for Tabular ML (Beginner) -->
<!-- Meta description: Learn 9) intersection of planes — intersection of planes with an online-store spreadsheet example, worked numbers, and NumPy. -->
<!-- Keywords: vectors, linear algebra, data science, spreadsheets, numpy -->

**Breadcrumbs:** Home > Vectors > 9) Intersection of Planes — Intersection of Planes

# 9) Intersection of Planes — Intersection of Planes

**Quick reminder: our dataset**  
Each customer is one row. Each column is a **feature** (a spreadsheet column). A **model** is a formula that uses features to make a guess.

`x = [age, income_k, website_visits_last_week, emails_opened_last_month, prior_purchases, satisfaction_score]`

## A) What it means
Two planes usually intersect in a line (many solutions).

## B) How to picture it
Two sheets cross; overlap is a line.

```text
\ plane 1
   \____ line
   / 
  / plane 2
```

## C) Business example
Meet multiple rules at once (example: high buy-likelihood and low stop-risk). The overlap gives profiles satisfying both.

## D) Where it shows up in basic ML
Plain words: Intersection means meeting constraints.
In data science, this relates to optimization (best choices under rules).

## E) Worked numeric example
Solve the two plane equations to get a line of solutions.

1. Use (x,y,z)=[visits,opens,satisfaction].
2. Plane1: x+y+z=6. Plane2: x−y+z=2.
3. Subtract → y=2.
4. Then x+z=4 → set x=t, z=4−t.
5. Line: [t,2,4−t].

| Item | Value |
|---|---|
| `parametric` | `[t,2,4−t]` |
| `point+dir` | `[0,2,4] + t[1,0,−1]` |

## F) Tiny Python (NumPy) snippet
```python
import numpy as np
for t in [0,1,2]:
    v=np.array([t,2,4-t])
    print(v, v.sum(), v[0]-v[1]+v[2])
```

## Try it yourself
1. Open a terminal.
2. Run `python -m pip install numpy`
3. Paste the code into `lesson.py` and run `python lesson.py`

> **Key takeaways**
> - Plane intersections often give a line.
> - Solve by combining equations.

> **Common mistakes**
> - Expecting one solution.
> - Losing track of feature↔variable mapping.

## Practice questions (with answers)
1. **Practice 1: Using the numeric example, redo the calculation with one number changed. What do you get?**  
   *Answer: Follow the same steps; change only that component, then recompute.*
2. **Practice 2: Explain in one sentence what this operation means for customer rows in a spreadsheet.**  
   *Answer: It combines/compares/scales customer-feature columns in a consistent, column-by-column way.*

## Resources
- **Free video:** [MIT OpenCourseWare — 18.06 Linear Algebra](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/)
- **Free practice:** [MIT OCW — Linear Algebra problem sets with solutions](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/resources/problem-sets-with-solutions/)
- **Applied tabular ML resource:** [scikit-learn — LogisticRegression documentation](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)

## Visuals (optional)
- **Realistic image prompt:** Photorealistic scene of an online store marketer reviewing a spreadsheet while learning 9) intersection of planes — intersection of planes.
- **Infographic prompt:** Clean infographic showing 9) Intersection of Planes — Intersection of Planes with simple arrows and a tiny customer-feature table.
- **Alt text:** Illustration supporting 9) Intersection of Planes — Intersection of Planes with a simple vector sketch and a small customer table.
- **Caption:** 9) Intersection of Planes — Intersection of Planes explained with a small online-store spreadsheet example.

## Navigation
[← Previous lesson](intersection-of-lines-3d.md)
