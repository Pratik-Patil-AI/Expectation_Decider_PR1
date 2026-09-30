# 🎥 Video Explanation
**[▶️ Watch the video walkthrough here — paste your Google Drive / YouTube link]**

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

1. **Understanding the Basics** — definition of probability, key terminology, three example events from the dataset
2. **Types of Events** — empirical vs. theoretical probability, calculated from the data
3. **Random Variable & Probability Distribution** — hypergeometric distribution of "students passing out of 3 randomly selected," with mean and variance
4. **Venn Diagram** — study hours vs. attendance, with overlap
5. **Contingency Table** — group discussion vs. exam result, with joint / marginal / conditional probabilities
6. **Understanding Relationships** — conditional probability intuition, independence check
7. **Bayes' Theorem** — probability of passing given high attendance

Each section closes with a final summary of which factors most affect the probability of passing.

## 🛠️ How to Run

```bash
pip install pandas numpy matplotlib matplotlib-venn scipy
jupyter notebook Expectation_Decider.ipynb
```

## 📌 Notes

- The dataset was generated programmatically for this project (per the assignment's instructions) with realistic dependencies between study hours, attendance, test scores, group discussion, and the pass outcome.
- All calculations in the theory PDF are reproduced and verified live in the notebook.

---
**Expectation Decider** · Mathematics & Advanced Statistics
