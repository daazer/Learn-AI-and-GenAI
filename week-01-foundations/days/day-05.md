# week-01-foundations - Day 05: Matplotlib Essentials

## Reading (5-15 minutes)
- [Matplotlib quick start](https://matplotlib.org/stable/users/explain/quick_start.html) - read figure/axes basics.
- [Pyplot tutorial](https://matplotlib.org/stable/tutorials/pyplot.html) - skim labels and savefig.

## How To Read (2-3 minutes)
- Focus on titles, axis labels, legend, and saving to file.

## Build (Detailed Coding / Practice)
1. Create `week-01-foundations/code/day05_plots.py`.
2. Generate one histogram and one line plot from synthetic data.
3. Save `week-01-foundations/artifacts/histogram.png` and `week-01-foundations/artifacts/line_plot.png`.
4. Add titles and axis labels on both plots.
5. Write interpretation notes in `week-01-foundations/artifacts/day-05-readme.md`.

## Practice Drills
- Change histogram bins (10 vs 30) and note visual change.
- Add grid to line plot and decide if readability improves.

## Done When
- [ ] Both image files exist and render.
- [ ] Both plots are labeled.
- [ ] Interpretation notes mention what the plots mean.
---

# 📘 Learnbook Chapter 05 — Matplotlib Essentials

## 1️⃣ What Problem Are We Solving?

Data is easier to understand when you can **see it**.

Today you learned how to create basic visualizations with Matplotlib:

- Histogram (distribution)
- Line plot (trend/change)
- Titles and labels
- Saving plots to files

This is the foundation of exploratory data analysis.

---

## 2️⃣ Matplotlib Mental Model: Figure and Axes

Matplotlib plotting becomes much easier when you separate:

- **Figure** = the whole canvas/image
- **Axes** = the actual plot area (chart)

Think of it like:

```text
Figure = page
Axes   = chart drawn on the page
````

Most confusion comes from mixing these concepts.

---

## 3️⃣ Why Labels Matter (Professional Habit)

A plot without labels is just decoration.

Every plot should answer:

* What is this showing? (**title**)
* What is on the x-axis? (**x label**)
* What is on the y-axis? (**y label**)
* Which line is which? (**legend**, if multiple lines)

Professional rule:

> If someone screenshots your chart with no context, it should still be understandable.

---

## 4️⃣ Histogram: Understanding Distribution

A histogram shows how values are distributed across ranges (bins).

Typical questions it helps answer:

* Where do most values cluster?
* Is the data spread out or tight?
* Is it skewed left/right?
* Are there outliers?

Example concept:

```python
plt.hist(data, bins=10)
plt.title("Value Distribution")
plt.xlabel("Value")
plt.ylabel("Frequency")
```

### What “bins” changes

* **Fewer bins (e.g., 10):** smoother, simpler summary
* **More bins (e.g., 30):** more detail, more noise

This is why your drill (10 vs 30 bins) matters:
you are learning that visualization choices affect interpretation.

---

## 5️⃣ Line Plot: Understanding Trends

A line plot shows how a value changes across an ordered axis (often time or steps).

Typical questions it helps answer:

* Is the trend increasing or decreasing?
* Is there a pattern or cycle?
* Where are jumps or drops?

Example concept:

```python
plt.plot(x, y, label="signal")
plt.title("Trend Over Time")
plt.xlabel("Step")
plt.ylabel("Value")
plt.legend()
```

Use line plots when order matters.

---

## 6️⃣ Synthetic Data Is Still Valuable

Even when data is randomly generated (synthetic), plotting is useful for learning:

* Plotting API basics
* Labeling habits
* Save/export workflow
* Visual interpretation practice

Professional mindset:

> Practice plotting mechanics on synthetic data so you are ready for real data later.

---

## 7️⃣ Saving Plots to Files (Reproducible Output)

You saved plots as:

* `histogram.png`
* `line_plot.png`

This is important because it makes your work:

* Shareable
* Checkable
* Reusable in reports/docs
* Independent of interactive sessions

Core command:

```python
plt.savefig("path/to/file.png")
```

Professional rule:

> If a plot matters, save it.

---

## 8️⃣ Grid: Readability vs Clutter

A grid can improve readability, especially for line plots, by making values easier to estimate.

Example:

```python
plt.grid(True)
```

But a grid is not always better.

Use your judgment:

* Good for quantitative reading
* Can add visual clutter if overused

This is a design decision, not just a coding step.

---

## 9️⃣ Plot Interpretation Is Part of the Task

Making a chart is only half the job.

You also wrote interpretation notes. That is excellent practice.

A useful interpretation note should say:

1. **What the plot shows**
2. **What pattern you notice**
3. **What it might mean**
4. **Any limits/cautions** (e.g., synthetic data)

Example interpretation style:

* “The histogram is centered near X, suggesting most values cluster there.”
* “The line plot shows an upward trend with small fluctuations.”
* “Changing bins from 10 to 30 reveals more local variation.”

Professional rule:

> Charts communicate visually; notes communicate reasoning.

---

## 🔟 Common Beginner Mistakes

❌ Forgetting `plt.savefig(...)` before closing/showing
❌ Missing title or axis labels
❌ Using a line plot when a histogram is needed (or vice versa)
❌ Overcrowded plots with unclear meaning
❌ Writing no interpretation after plotting

---

## 1️⃣1️⃣ Professional Plot Checklist

Before calling a plot “done,” verify:

* [ ] Correct plot type for the question
* [ ] Title added
* [ ] X-axis label added
* [ ] Y-axis label added
* [ ] Legend added (if needed)
* [ ] File saved to artifact path
* [ ] Interpretation written in plain language

This checklist will scale with you as plots get more advanced.

---

## 1️⃣2️⃣ Why This Matters for AI / Data Work

Visualization is essential in ML and analytics for:

* Checking data quality
* Understanding distributions
* Spotting outliers
* Inspecting training metrics (loss/accuracy curves)
* Communicating results to others

Matplotlib is a foundation tool — even when higher-level libraries are used later.

---

## 🔒 Day 05 Core Takeaway

> A good plot is not just generated — it is labeled, saved, and interpreted.

You are learning to move from “I made a chart” to “I communicated evidence.”

---