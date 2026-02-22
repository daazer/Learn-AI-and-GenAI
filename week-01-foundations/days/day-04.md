# week-01-foundations - Day 04: NumPy Arrays and Vectorization

## Reading (5-15 minutes)
- [NumPy quickstart](https://numpy.org/doc/stable/user/quickstart.html) - read array creation/indexing.
- [NumPy broadcasting](https://numpy.org/doc/stable/user/basics.broadcasting.html) - read rules and examples.

## How To Read (2-3 minutes)
- Write one vectorized operation that replaces a Python loop.

## Build (Detailed Coding / Practice)
1. Create `week-01-foundations/code/day04_numpy.py`.
2. Implement `normalize(arr)` and `pairwise_add(a,b)` using NumPy only.
3. Seed with `np.random.seed(42)`, run on test arrays, and print shape checks.
4. Save numeric summary to `week-01-foundations/artifacts/day-04-stats.txt`.
5. Add one note in `notes/mistakes-and-fixes.md` about a broadcasting error you fixed.

## Practice Drills
- Implement loop-based normalization and compare with vectorized output.
- Trigger one shape mismatch intentionally, then fix it.

## Done When
- [ ] Vectorized functions run without loops in core logic.
- [ ] Stats artifact exists.
- [ ] Broadcasting pitfall documented.

````md
---

# 📘 Learnbook Chapter 04 — NumPy Arrays & Vectorization

## 1️⃣ What Problem Are We Solving?

Pure Python loops work, but they become slow and verbose for numeric computing.

NumPy solves this by providing:

- Fast array operations
- Vectorized math
- Broadcasting across shapes

This is the foundation of data science, machine learning, and scientific computing in Python.

---

## 2️⃣ Arrays vs Python Lists

A Python list is a general-purpose container.

```python
nums = [1, 2, 3]
````

A NumPy array is a numeric data structure optimized for computation.

```python
import numpy as np
arr = np.array([1, 2, 3])
```

Why arrays matter:

* Faster numeric operations
* Elementwise math
* Shape-aware programming

Mental model:

```text
List  = flexible container
Array = math-ready block of numbers
```

---

## 3️⃣ Vectorization: Replacing Loops with Array Math

### Loop-based style (works, but slower and noisier)

```python
out = []
for x in nums:
    out.append(x * 2)
```

### Vectorized style (preferred with NumPy)

```python
out = arr * 2
```

Vectorization means:

> Write the operation once, apply it to the whole array.

This makes code:

* Shorter
* Clearer
* Faster

---

## 4️⃣ Shapes Are a Core Concept

Every NumPy array has a shape.

```python
arr.shape
```

Examples:

* `(5,)` → 1D array with 5 elements
* `(3, 4)` → 2D array with 3 rows, 4 columns

Professional rule:

> Before debugging values, check shapes.

Shape mistakes are one of the most common NumPy errors.

---

## 5️⃣ Normalization: Scaling Data for Stable Computation

A normalization function transforms values to a comparable scale.

Common examples:

* Min-max scaling
* Mean/std normalization (standardization)

Vectorized min-max style example:

```python
def normalize(arr):
    arr = np.asarray(arr, dtype=float)
    return (arr - arr.min()) / (arr.max() - arr.min())
```

Why this matters in ML:

* Features can have different ranges
* Scaling improves optimization and model behavior
* Prevents large-value features from dominating

### Important Edge Case

If all values are equal, then:

```python
arr.max() - arr.min() == 0
```

That causes division by zero.

Professional mindset:

> Define behavior for constant arrays (e.g., return zeros).

---

## 6️⃣ Pairwise Addition: Elementwise Operations

Your `pairwise_add(a, b)` should use NumPy math directly:

```python
a + b
```

This performs elementwise addition when shapes are compatible.

Example:

```python
[1, 2, 3] + [10, 20, 30]  ->  [11, 22, 33]
```

With NumPy arrays:

```python
np.array([1, 2, 3]) + np.array([10, 20, 30])
```

No loop needed.

---

## 7️⃣ Broadcasting: Small Array Expands to Fit

Broadcasting lets NumPy operate on arrays of different shapes **when rules allow**.

Example:

```python
np.array([1, 2, 3]) + 10
# [11, 12, 13]
```

Here, `10` is broadcast across all elements.

Another example:

```python
np.array([[1], [2], [3]]) + np.array([10, 20])
```

Shapes can expand logically without copying data in the way you might expect from manual loops.

Mental model:

```text
NumPy tries to align shapes from the right.
If dimensions match (or one is 1), broadcasting can happen.
```

---

## 8️⃣ Common Broadcasting Pitfall

A shape mismatch can fail like this:

```python
(3,) + (2,)
```

These are incompatible for elementwise addition.

Typical fixes:

* Reshape one array
* Use matching lengths
* Add a dimension intentionally (`reshape`, `np.newaxis`)

Professional debugging checklist:

1. Print `a.shape`
2. Print `b.shape`
3. Check intended output shape
4. Reshape explicitly

---

## 9️⃣ Loop vs Vectorized Thinking

### Loop thinking

* "Take one item at a time"

### Vectorized thinking

* "Transform the whole array at once"

This shift is important because most numerical libraries (NumPy, pandas, PyTorch, TensorFlow) are built around array/tensor operations.

---

## 🔟 Reproducibility with Random Seeds

Using:

```python
np.random.seed(42)
```

makes your random outputs reproducible.

Why this matters:

* Easier debugging
* Stable practice results
* Comparable outputs across runs

Professional rule:

> If randomness affects output, set a seed during development and learning.

---

## 1️⃣1️⃣ Common Beginner Mistakes

❌ Mixing Python lists and NumPy arrays unintentionally
❌ Forgetting to check `.shape`
❌ Using loops in core numeric logic when vectorization is possible
❌ Ignoring division-by-zero in normalization
❌ Assuming broadcasting always works

---

## 1️⃣2️⃣ Professional Pattern: Shape-First, Then Math

A strong NumPy workflow is:

1. Convert inputs to arrays (`np.asarray`)
2. Check shapes
3. Apply vectorized math
4. Validate output shape
5. Handle edge cases

This leads to code that is easier to trust and debug.

---

## 🔒 Day 04 Core Takeaway

> NumPy is not just a faster list — it is a different way of thinking.

When you think in arrays, shapes, and vectorized operations, numeric programming becomes simpler, cleaner, and scalable.

---