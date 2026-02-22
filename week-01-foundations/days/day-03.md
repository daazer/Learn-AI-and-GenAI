# week-01-foundations - Day 03: Core Data Structures in Practice

## Reading (5-15 minutes)
- [Python tutorial: data structures](https://docs.python.org/3/tutorial/datastructures.html) - read lists/dicts/sets/tuples.
- [collections.Counter docs](https://docs.python.org/3/library/collections.html#collections.Counter) - read basic usage.

## How To Read (2-3 minutes)
- For each structure, write one ML preprocessing use case.

## Build (Detailed Coding / Practice)
1. Create `week-01-foundations/code/day03_structures.py`.
2. Implement `word_count(text)`, `unique_tokens(text)`, and `index_pairs(items)`.
3. Use two sample text strings and print outputs with labels.
4. Save output to `week-01-foundations/artifacts/day-03-structures.txt`.
5. Add a mapping table to `week-01-foundations/notes/theory-summary.md`: structure -> AI use case.

## Practice Drills
- Compare dict counts vs Counter counts on same text.
- Add one edge case: empty string input.

## Done When
- [ ] All three functions run correctly.
- [ ] Artifact output exists.
- [ ] Theory table is present.

---

# 📘 Learnbook Chapter 03 — Core Data Structures in Practice

## 1️⃣ What Problem Are We Solving?

Programs don’t just compute — they **organize information**.

Today you learned how to structure data using:

- Lists
- Tuples
- Dictionaries
- Sets
- `collections.Counter`

These are the building blocks of everything from APIs to machine learning pipelines.

---

## 2️⃣ Lists — Ordered, Mutable Sequences

Lists store ordered collections.

```python
tokens = ["machine", "learning", "is", "fun"]
````

Use lists when:

* Order matters
* You need indexing
* You may modify elements

Example use case (ML preprocessing):

```python
def unique_tokens(text):
    tokens = text.split()
    return list(set(tokens))
```

Mental model:

```
List = Ordered container
```

---

## 3️⃣ Tuples — Ordered, Immutable Records

Tuples are like lists but immutable.

```python
pair = (index, value)
```

Use tuples when:

* Data should not change
* Representing fixed records
* Returning multiple values

Example:

```python
def index_pairs(items):
    pairs = []
    for i, item in enumerate(items):
        pairs.append((i, item))
    return pairs
```

Mental model:

```
Tuple = Locked record
```

---

## 4️⃣ Dictionaries — Key → Value Mapping

Dictionaries are hash maps.

```python
counts = {"machine": 2, "learning": 1}
```

Use dictionaries when:

* You need fast lookup
* You are counting
* You are mapping identifiers

Example word counter:

```python
def word_count(text):
    counts = {}
    for word in text.split():
        counts[word] = counts.get(word, 0) + 1
    return counts
```

Mental model:

```
Dictionary = Instant lookup table
```

Time complexity (average):

* Lookup → O(1)
* Insert → O(1)

---

## 5️⃣ Sets — Unordered Unique Elements

Sets remove duplicates automatically.

```python
unique = set(["a", "b", "a"])
# {"a", "b"}
```

Use sets when:

* You only care about uniqueness
* You need fast membership testing

ML example:

* Removing duplicate tokens
* Vocabulary construction

Mental model:

```
Set = Uniqueness filter
```

---

## 6️⃣ Counter — Specialized Dictionary for Counting

`Counter` simplifies counting logic.

```python
from collections import Counter

counts = Counter(text.split())
```

Compared to manual dict counting:

* Cleaner
* More readable
* Built-in utilities (most_common)

Example:

```python
Counter("a a b b b".split())
# {'b': 3, 'a': 2}
```

Professional rule:

> Use built-in tools when they clearly express intent.

---

## 7️⃣ Structure → AI Use Case Mapping

| Structure | AI / ML Use Case        |
| --------- | ----------------------- |
| List      | Token sequences         |
| Tuple     | (index, token) pairs    |
| Dict      | Word frequency table    |
| Set       | Vocabulary extraction   |
| Counter   | Fast frequency analysis |

These patterns appear constantly in NLP and preprocessing pipelines.

---

## 8️⃣ Edge Cases Matter

Always consider:

```python
word_count("")
unique_tokens("")
```

Empty input should:

* Not crash
* Return empty structure
* Remain predictable

Professional mindset:

> Handle edge cases early.

---

## 9️⃣ Dict vs Counter — When to Use What

Manual dictionary:

* More control
* Educational clarity

`Counter`:

* Cleaner
* Faster to implement
* Expresses counting intent directly

If your function’s purpose is counting → prefer `Counter`.

---

## 🔒 Day 03 Core Takeaway

> The power of Python comes from choosing the right data structure.

If your structure matches your problem, the solution becomes simple.

If your structure is wrong, everything becomes complicated.

Master the structures — the algorithms become easier.

---