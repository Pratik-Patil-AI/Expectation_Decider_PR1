# 📊 Expectation Decider: Probability & Statistics Analytics Report

> **Probability & statistics analysis predicting student exam outcomes — empirical/theoretical probability, hypergeometric distribution, Venn diagrams, contingency tables, and Bayes' Theorem.**

[![Python](https://img.shields.io/badge/Python-Analysis-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)]()
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)

---

# 🎥 Video Explanation

[![Watch the video](https://img.youtube.com/vi/LgM7wWTBUOo/maxresdefault.jpg)](https://youtu.be/LgM7wWTBUOo)

**[▶️ Or click here to watch directly](https://youtu.be/LgM7wWTBUOo)**

---

# Expectation Decider — Probability & Statistics Project

Predicting whether a student passes a competitive mathematics exam, using probability theory applied to a 200-student dataset (study hours, attendance, group-discussion participation, and previous test scores).

## 📁 Repository Structure

| File | Description |
|---|---|
| `Expectation_Decider.ipynb` | Full practical analysis — Markdown explanations + executable code cells, covering all 7 tasks |
| `Expectation_Decider_Theory.pdf` | Theory write-up (Component A1) — definitions, formulas, step-by-step derivations |
| `students_dataset.csv` | The 200-student dataset used throughout the analysis |
| `README.md` | This file |

## 📊 Dataset

`students_dataset.csv` — 200 rows, 6 columns:

| Column | Description |
|---|---|
| `student_id` | Unique student identifier |
| `study_hours` | Hours studied per week |
| `attendance` | Attendance percentage in lectures |
| `group_discussion` | Participation in group discussions (Yes/No) |
| `previous_test_score` | Marks out of 100 on the last internal test |
| `final_exam_pass` | Result of the competitive exam (Pass/Fail) |

## ✅ Tasks Covered in the Notebook
 
### 1. Understanding the Basics
Defines probability from first principles (a measure between 0 and 1 of how likely an event is) and walks through the core vocabulary — experiment, sample space, event, mutually exclusive events, independent events, and conditional probability — with each term grounded in a concrete example from the dataset. Identifies three probability events directly from the data: a student studying more than 10 hrs/week, a student attending more than 80% of classes, and a student passing the final exam.
 
### 2. Types of Events — Empirical vs. Theoretical Probability
Distinguishes the two ways probability gets calculated. **Empirical probability** is computed as observed relative frequency: P(Pass) = 88/200 = 0.44, taken directly from the 200 recorded outcomes. **Theoretical probability** is computed from the classical (equally-likely-outcomes) model: P(study_hours > 10) = 74/200 = 0.37, by simply counting favourable vs. total outcomes rather than relying on the exam result.
 
### 3. Random Variable & Probability Distribution
Defines the random variable **X = "number of students who pass, out of 3 randomly selected (without replacement)"** and identifies it as following a **hypergeometric distribution** (since sampling is without replacement from a finite population of 200). Builds the full probability distribution table for X = 0, 1, 2, 3, then derives the **mean E[X] ≈ 1.32** and **variance Var[X] ≈ 0.73**, with an interpretation of what these values mean in context.
 
### 4. Venn Diagram in Probability
Constructs a two-set Venn diagram: **Set A** = students studying more than 10 hrs/week (74 students), **Set B** = students with attendance above 80% (77 students), with the **overlap (A ∩ B)** = 26 students satisfying both conditions — rendered visually with `matplotlib-venn` and generated directly from the dataset rather than hardcoded.
 
### 5. Contingency Table & Probability Calculations
Cross-tabulates `group_discussion` (Yes/No) against `final_exam_pass` (Pass/Fail) into a full contingency table with row/column totals. From it, calculates the **joint probability** P(Group Discussion = Yes ∩ Pass) = 0.295, the **marginal probability** P(Pass) = 0.44, and the **conditional probability** P(Pass | Group Discussion = Yes) = 0.4876.
 
### 6. Understanding Relationships
Explains the intuition behind conditional probability in plain language — narrowing the sample space to only the sub-group that satisfies the given condition, then asking what fraction of that smaller group satisfies the event of interest. Runs a formal **independence check** (comparing P(A∩B) to P(A)·P(B)) to determine that group-discussion participation and passing the exam are **dependent**, not independent or mutually exclusive events.
 
### 7. Bayes' Theorem Application
Applies Bayes' Theorem to a real inference question: given P(High Attendance | Pass) = 0.70, P(High Attendance | Fail) = 0.40, and P(High Attendance) = 0.60, calculates **P(Pass | High Attendance) ≈ 0.5833 (58.33%)** — showing how observing high attendance updates the prior 50% belief of passing upward, with the full formula, substitution, and interpretation shown step-by-step.
 
### Final Summary
Closes with a consolidated, data-driven summary of which factors most affect the probability of passing — highlighting attendance and study hours as the strongest positive predictors, with group-discussion participation as a secondary, statistically dependent factor.

## 🛠️ How to Run

```bash
pip install pandas numpy matplotlib matplotlib-venn scipy
jupyter notebook Expectation_Decider.ipynb
```

## 👨‍💻 Author

**Pratik Patil**

---

## ⭐ Support

Star ⭐ this repo if you like it!

---
**Expectation Decider** · Mathematics & Advanced Statistics
