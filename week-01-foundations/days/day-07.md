# week-01-foundations - Day 07: Weekly Synthesis: Linear vs Nonlinear

## Reading (5-15 minutes)
- [3Blue1Brown linear transformation intro](https://www.youtube.com/watch?v=kYB8IZa5AuE) - watch first 8-10 min.
- [Linear function definition](https://en.wikipedia.org/wiki/Linear_function) - skim definition/examples.

## How To Read (2-3 minutes)
- Capture one linear and one nonlinear pattern from your own week-1 code.

## Build (Detailed Coding / Practice)
1. Create `week-01-foundations/notes/linear-vs-nonlinear.md` with 3 concrete examples each.
2. Create `week-01-foundations/notes/weekly-retrospective.md` with wins, blockers, fixes, next-week prep.
3. Create `week-01-foundations/code/run_all.ps1` to run day02-day06 scripts.
4. Run `run_all.ps1` once and log pass/fail in `week-01-foundations/artifacts/results.md`.
5. Clean file naming so scripts use day prefixes consistently.

## Practice Drills
- Explain linear vs nonlinear to a beginner in 5 sentences in your notes.
- Add one TODO for week 2 pipeline improvements.

## Done When
- [ ] Retrospective and concept note are complete.
- [ ] Run-all script exists and executes.
- [ ] Results log captures outcomes.

````md
---

# 📘 Learnbook Chapter 07 — Weekly Synthesis: Linear vs Nonlinear

## 1️⃣ What Problem Are We Solving?

This week you learned many tools (functions, loops, data structures, NumPy, plotting, statistics).

Now the goal is different:

- **Connect concepts**
- **Recognize patterns**
- **Build a mental model**
- **Improve your workflow**

The key concept for this synthesis is:

- **Linear** behavior
- **Nonlinear** behavior

This distinction appears everywhere in programming, math, and machine learning.

---

## 2️⃣ What “Linear” Means (Practical Intuition)

A relationship is **linear** when changes are proportional and consistent.

If input changes by a fixed amount, output changes in a predictable fixed way.

Examples (intuition):

- `y = 2x + 3`
- adding a constant to every value
- scaling an array by a constant

Mental model:

```text
Straight-line behavior
Predictable rate of change
````

In code, linear often feels like:

* “apply the same rule to every element”
* “output changes steadily as input changes”

---

## 3️⃣ What “Nonlinear” Means (Practical Intuition)

A relationship is **nonlinear** when output does not change at a constant rate.

Small input changes can produce different-sized output changes depending on where you are.

Examples:

* thresholds (`if score >= 90: "A"`)
* squaring (`x^2`)
* distributions with skew/outliers affecting summary behavior
* piecewise logic

Mental model:

```text
Curved / threshold / piecewise behavior
Rate of change is not constant
```

In code, nonlinear often appears when:

* branching logic exists
* categories replace continuous values
* interactions depend on conditions or shape

---

## 4️⃣ Linear vs Nonlinear in Your Week 1 Work

You were already using both types of thinking.

### Likely Linear Patterns from Week 1

* **Pairwise array addition** in NumPy (`a + b`)
* **Running sum accumulation** (adds values in a consistent way)
* **Line plot of a simple trend** (if generated from linear-like data)
* **Scaling/normalization components** (subtracting min, dividing by range are linear operations individually)

### Likely Nonlinear Patterns from Week 1

* **`grade_score(score)`** (threshold-based categories)
* **`is_even(n)`** (modulo-based classification)
* **Histogram shape interpretation** (visual patterns are not a linear rule)
* **Skewed distributions** (mean/variance behavior can be unintuitive)

Professional insight:

> Real programs usually combine linear operations with nonlinear decisions.

---

## 5️⃣ Why This Distinction Matters for ML and AI

Machine learning models often combine:

* **Linear transformations** (weighted sums, matrix operations)
* **Nonlinearities** (activation functions, thresholds, decision boundaries)

Why?

* Purely linear systems are limited in what patterns they can represent.
* Nonlinearity allows models to represent complex behavior.

This week you built intuition for both without needing advanced ML yet.

---

## 6️⃣ Weekly Synthesis of What You Actually Learned

### Day 01 — Environment & Reproducibility

You learned how to make work repeatable.

Core skill:

* isolated Python environment
* install + run + document

Why it matters:

* no reproducibility → no trustworthy project

---

### Day 02 — Program Structure

You learned how to express logic.

Core skill:

* variables
* conditionals
* loops
* functions
* assertions

Why it matters:

* this is how programs become readable and testable

---

### Day 03 — Data Structures

You learned how to represent information correctly.

Core skill:

* list / tuple / dict / set / Counter
* choosing structure by problem type

Why it matters:

* correct structure reduces complexity

---

### Day 04 — NumPy & Vectorization

You learned array thinking.

Core skill:

* vectorized operations
* shapes
* broadcasting
* debugging by shape checks

Why it matters:

* numerical programming becomes scalable

---

### Day 05 — Matplotlib

You learned visual communication.

Core skill:

* histogram and line plot
* labels and titles
* saving figures
* writing interpretation

Why it matters:

* analysis is incomplete without communication

---

### Day 06 — Numerical Experiments

You learned statistical intuition.

Core skill:

* mean and variance
* synthetic distributions
* histogram + summary together
* surprising-result documentation

Why it matters:

* metrics become meaningful only when interpreted

---

## 7️⃣ Weekly Retrospective Framework (What to Write)

Your retrospective should not be vague. Use concrete evidence.

### Wins

What worked well?

* Which scripts ran cleanly?
* Which concept clicked?
* Which habit improved (naming, saving outputs, assertions)?

### Blockers

What slowed you down?

* environment issues
* shape mismatch
* plotting confusion
* edge cases

### Fixes

What specifically solved the blocker?

* printed shapes
* added assertions
* rewrote function
* checked docs
* simplified logic

### Next-Week Prep

What will make Week 2 smoother?

* standardized script naming
* reusable helper functions
* better artifact folder structure
* a run-all workflow

Professional rule:

> Retrospectives should produce actions, not just feelings.

---

## 8️⃣ Run-All Script: Why It’s a Big Step

Creating `run_all.ps1` is more important than it looks.

It moves you from:

* manually running files one by one

to:

* repeatable execution workflow

This is an early automation habit.

Benefits:

* faster feedback
* easier debugging
* easier regression checking
* better project discipline

Mental model:

```text
Manual execution -> Scripted execution -> Reliable workflow
```

---

## 9️⃣ Results Log: Pass/Fail Is a Professional Habit

Logging pass/fail outcomes in `results.md` teaches an important engineering behavior:

* record what happened
* avoid guessing later
* separate “I think it worked” from “it ran successfully”

A simple log can include:

* script name
* pass/fail
* timestamp
* error note (if any)

This is lightweight but powerful.

---

## 🔟 File Naming Consistency Is Not Cosmetic

Cleaning filenames to use day prefixes consistently improves:

* discoverability
* automation
* sorting
* maintenance

Example benefit:

* `day02_...`, `day03_...`, `day04_...` sort naturally
* run-all scripts become easier to manage

Professional insight:

> Naming is part of system design.

---

## 1️⃣1️⃣ Common Week-1 Patterns You Should Keep

✅ Save outputs to artifact files
✅ Write short interpretation notes
✅ Use fixed seeds for reproducibility
✅ Add assertions for correctness
✅ Check shapes before debugging values
✅ Use the right data structure for the task

These habits matter more than any single syntax detail.

---

## 1️⃣2️⃣ Common Week-1 Mistakes to Avoid Repeating

❌ Running code without saving results
❌ Trusting output without assertions/checks
❌ Debugging NumPy math without printing shapes
❌ Making plots without labels
❌ Writing notes that are too vague (“it worked”)
❌ Inconsistent file names that break automation

---

## 1️⃣3️⃣ Beginner-Friendly 5-Sentence Explanation (Linear vs Nonlinear)

A **linear** pattern changes at a steady rate, like adding the same amount each time.
A **nonlinear** pattern does not change at a steady rate, and it may curve or have thresholds.
In code, simple arithmetic on arrays is often linear.
Conditionals like grading rules (`A`, `B`, `C`) are nonlinear because outputs change by ranges, not smoothly.
Most real programs and ML systems combine both.

---

## 1️⃣4️⃣ Week 2 Prep Mindset

Week 1 was about foundations.
Week 2 should build on that with better workflow and cleaner pipelines.

One strong TODO idea:

* **Create a shared utility module for repeated tasks** (loading data, saving outputs, printing summaries)

This reduces duplication and makes your project easier to grow.

---

## 🔒 Day 07 Core Takeaway

> Week 1 was not just about learning syntax — it was about building engineering habits.

You now have:

* reproducible setup
* structured code
* data handling
* numerical thinking
* visualization
* statistical intuition
* a workflow mindset

That is a real foundation.

---