# week-01-foundations - Day 06: Numerical Experiments: Mean, Variance, Histogram

## Reading (5-15 minutes)
- [NumPy statistics routines](https://numpy.org/doc/stable/reference/routines.statistics.html) - read `mean` and `var` docs.
- [Variance intuition](https://www.khanacademy.org/math/statistics-probability/summarizing-quantitative-data) - skim explanation.

## How To Read (2-3 minutes)
- Rewrite variance intuition in your own words in 2 lines.

## Build (Detailed Coding / Practice)
1. Create `week-01-foundations/code/day06_stats_experiment.py`.
2. Generate 3 synthetic datasets (normal, uniform, skewed) with fixed seed.
3. Compute and print mean/variance table for each dataset.
4. Save 3 histograms to `week-01-foundations/artifacts/day-06-hist-*.png`.
5. Document one surprising result in `week-01-foundations/notes/mistakes-and-fixes.md`.

## Practice Drills
- Double sample size and compare moment stability.
- Compare NumPy variance to a manual implementation.

## Done When
- [ ] All 3 distributions are analyzed.
- [ ] Histograms and table are saved.
- [ ] One interpretation note is documented.

````md
---

# 📘 Learnbook Chapter 06 — Numerical Experiments: Mean, Variance & Histogram

## 1️⃣ What Problem Are We Solving?

Numbers like **mean** and **variance** summarize data, but they are easier to trust when you **see them** and **experiment with them**.

Today you practiced:

- Generating synthetic datasets
- Measuring mean and variance
- Visualizing distributions with histograms
- Comparing numeric summaries to visual shape

This is the beginning of statistical intuition.

---

## 2️⃣ Why Numerical Experiments Matter

Statistics can feel abstract until you test them on real arrays.

Numerical experiments help you answer questions like:

- Do two datasets with similar means look the same?
- How much spread does variance actually represent?
- What changes when sample size increases?

Professional mindset:

> Don’t just compute a metric — inspect what it means.

---

## 3️⃣ Mean: The Center (But Not the Whole Story)

The **mean** is the average value.

```python
mean = np.mean(arr)
````

It tells you the center of the data, but it does **not** tell you:

* spread
* skew
* outliers
* shape of the distribution

Two datasets can have the same mean and look very different.

---

## 4️⃣ Variance: How Spread Out the Data Is

Variance measures how far values are, on average, from the mean (squared distance).

Intuition:

* Low variance → values are tightly clustered
* High variance → values are more spread out

```python
var = np.var(arr)
```

Mental model:

```text
Mean tells "where"
Variance tells "how spread"
```

---

## 5️⃣ Why Histograms Matter with Mean/Variance

A histogram shows the **shape** of the data.

This matters because mean and variance alone cannot reveal:

* skewness
* multimodality
* long tails
* unusual outliers

Example insight:

* A normal and a skewed distribution may have similar variance,
* but their histograms reveal very different shapes.

Professional rule:

> Pair summary statistics with a plot.

---

## 6️⃣ Your Three Synthetic Datasets (Why These Are Good Choices)

You generated:

* **Normal** distribution → symmetric, bell-shaped baseline
* **Uniform** distribution → flat spread across a range
* **Skewed** distribution → asymmetric shape with long tail

These are excellent learning cases because they train you to compare:

* center
* spread
* shape

Same tools, different behavior.

---

## 7️⃣ Reproducibility with Fixed Seed

Using a fixed seed (for example `np.random.seed(...)`) makes your results reproducible.

Why this matters:

* Same numbers across reruns
* Easier debugging
* Easier comparison after code changes

Professional rule:

> If you are learning or testing random behavior, set a seed.

---

## 8️⃣ Mean/Variance Table: What to Look For

When you print a summary table for each dataset, do not stop at the numbers.

Ask:

1. Which dataset has the highest mean?
2. Which has the highest variance?
3. Does the histogram visually match the variance?
4. Does skew change how you interpret the mean?

A good experiment is not just computing values — it is comparing expectations to results.

---

## 9️⃣ Variance in NumPy vs Manual Variance

A manual variance implementation is a great drill because it reinforces the formula:

```text
variance = average of (x - mean)^2
```

Typical manual steps:

1. Compute mean
2. Subtract mean from each value
3. Square differences
4. Average them

This helps you trust `np.var(...)` because you understand what it is doing.

---

## 🔟 Important Nuance: Population vs Sample Variance

By default, `np.var(arr)` computes **population variance** (`ddof=0`).

If you want **sample variance**, use:

```python
np.var(arr, ddof=1)
```

This can produce different values, especially for small datasets.

Professional mindset:

> Always know which variance definition your code is using.

---

## 1️⃣1️⃣ Sample Size and Stability (Your Drill Insight)

When you double sample size, statistics often become more stable:

* mean fluctuates less
* variance estimate usually stabilizes
* histogram shape looks closer to the “true” distribution

This is a core statistical idea:

> More data usually reduces randomness in summary estimates.

---

## 1️⃣2️⃣ Common Beginner Mistakes

❌ Interpreting mean without checking histogram
❌ Assuming same mean = same distribution
❌ Forgetting fixed seed when comparing runs
❌ Mixing sample variance and population variance unknowingly
❌ Judging spread only by eye without checking variance

---

## 1️⃣3️⃣ Professional Pattern: Stats + Visual + Note

A strong analysis workflow is:

1. Generate or load data
2. Compute summary metrics (mean, variance)
3. Plot histogram
4. Write one interpretation note
5. Record one surprising result

This builds statistical reasoning, not just coding ability.

---

## 1️⃣4️⃣ What Counts as a “Surprising Result”?

Examples of good surprises to document:

* A skewed dataset’s mean is pulled more than expected
* Uniform data looks “wider” than expected compared to normal
* Variance changed less than expected when sample size increased
* Histogram looked noisy despite similar mean/variance

The point is not to be “right” immediately — it is to notice and explain.

---

## 🔒 Day 06 Core Takeaway

> Mean and variance summarize data, but histograms reveal the story.

Statistics become powerful when you combine:
**numbers + visuals + interpretation**.

---