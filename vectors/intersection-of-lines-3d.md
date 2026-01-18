<!-- SEO -->
<!-- Title: 8) Intersection of Lines in 3D — Intersection of Lines in 3D — Vectors for Tabular ML (Beginner) -->
<!-- Meta description: Learn 8) intersection of lines in 3d — intersection of lines in 3d with an online-store spreadsheet example, worked numbers, and NumPy. -->
<!-- Keywords: vectors, linear algebra, data science, spreadsheets, numpy -->

**Breadcrumbs:** Home > Vectors > 8) Intersection of Lines in 3D — Intersection of Lines in 3D

# 8) Intersection of Lines in 3D — Intersection of Lines in 3D

**Quick reminder: our dataset**  
Each customer is one row. Each column is a **feature** (a spreadsheet column). A **model** is a formula that uses features to make a guess.

`x = [age, income_k, website_visits_last_week, emails_opened_last_month, prior_purchases, satisfaction_score]`

## A) What it means
Lines intersect if one point lies on both for some t and s.

## B) How to picture it
In 3D, lines can be skew and never meet.

```text
\  (line 1)
   \
    | (line 2)
```

## C) Business example
Two different customer-change plans might reach the same final profile. Intersection means both plans land on the same point.

## D) Where it shows up in basic ML
Plain words: Find values that make both rules true.
In machine learning, this is solving a system of equations.

## E) Worked numeric example
Both lines meet at [2,2,4].

1. L1(t)=[1,2,3]+t[1,0,1]=[1+t,2,3+t].
2. L2(s)=[2,1,4]+s[0,1,0]=[2,1+s,4].
3. Solve: 1+t=2 → t=1; 2=1+s → s=1; check z.
4. Intersection [2,2,4].

| Item | Value |
|---|---|
| `intersection` | `[2, 2, 4]` |
| `t` | `1` |
| `s` | `1` |

## F) Tiny Python (NumPy) snippet
```python
import numpy as np
p0=np.array([1,2,3]); d1=np.array([1,0,1])
q0=np.array([2,1,4]); d2=np.array([0,1,0])
t=s=1
print(p0+t*d1, q0+s*d2)
```

## Try it yourself
1. Open a terminal.
2. Run `python -m pip install numpy`
3. Paste the code into `lesson.py` and run `python lesson.py`

> **Key takeaways**
> - Intersection = same point for both lines.
> - Many 3D lines do not intersect.

> **Common mistakes**
> - Not checking all coordinates.
> - Assuming close lines intersect.

## Practice questions (with answers)
1. **Practice 1: Using the numeric example, redo the calculation with one number changed. What do you get?**  
   *Answer: Follow the same steps; change only that component, then recompute.*
2. **Practice 2: Explain in one sentence what this operation means for customer rows in a spreadsheet.**  
   *Answer: It combines/compares/scales customer-feature columns in a consistent, column-by-column way.*

## Resources
- **Free video:** [MIT OpenCourseWare — 18.06 Linear Algebra](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/)
- **Free practice:** [Khan Academy — Shortest distance between two lines (practice)](https://www.khanacademy.org/exercise/shortest-distance-between-two-lines)
- **Applied tabular ML resource:** [Kaggle Learn — How Models Work](https://www.kaggle.com/code/dansbecker/how-models-work)

## Visuals (optional)
- **Realistic image prompt:** Photorealistic scene of an online store marketer reviewing a spreadsheet while learning 8) intersection of lines in 3d — intersection of lines in 3d.
- **Infographic prompt:** Clean infographic showing 8) Intersection of Lines in 3D — Intersection of Lines in 3D with simple arrows and a tiny customer-feature table.
- **Alt text:** Illustration supporting 8) Intersection of Lines in 3D — Intersection of Lines in 3D with a simple vector sketch and a small customer table.
- **Caption:** 8) Intersection of Lines in 3D — Intersection of Lines in 3D explained with a small online-store spreadsheet example.

## Navigation
[← Previous lesson](equation-of-a-plane.md) | [Next lesson →](intersection-of-planes.md)
