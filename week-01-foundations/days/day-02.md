# week-01-foundations - Day 02: Variables, Control Flow, and Functions

## Reading (5-15 minutes)
- [Python tutorial: control flow](https://docs.python.org/3/tutorial/controlflow.html) - read `if`, `for`, and function sections.
- [Real Python: defining functions](https://realpython.com/defining-your-own-python-function/) - skim args and returns.

## How To Read (2-3 minutes)
- Capture one example each for conditional, loop, and reusable function.

## Build (Detailed Coding / Practice)
1. Create `week-01-foundations/code/day02_basics.py`.
2. Implement `is_even(n)`, `grade_score(score)`, and `running_sum(nums)`.
3. Add inline assertions for at least 6 cases total.
4. Run script and save terminal output to `week-01-foundations/artifacts/day-02-output.txt`.
5. Append one paragraph to `week-01-foundations/notes/theory-summary.md` about `for` vs `while`.

## Practice Drills
- Break one assertion intentionally, rerun, then fix it.
- Refactor one function using a cleaner structure.

## Done When
- [ ] All assertions pass.
- [ ] Script output file exists.
- [ ] Theory note has one concrete rule for loop choice.

````md
---

# 📘 Learnbook Chapter 02 — Variables, Control Flow & Functions

## 1️⃣ What Problem Are We Solving?

Programming is about **decision-making and reuse**.

Today you learned how to:

- Store information (variables)
- Make decisions (`if`)
- Repeat work (`for`, `while`)
- Reuse logic (functions)

Without these, programs cannot scale beyond simple scripts.

---

## 2️⃣ Variables: Naming Memory

A variable is a labeled container for data.

```python
score = 85
name = "Alice"
is_active = True
````

Variables allow your program to:

* Remember state
* Transform values
* Pass information between functions

### Rule of Thumb

> If a value might change or be reused — give it a name.

---

## 3️⃣ Control Flow: Teaching the Program to Decide

### Conditionals (`if` / `elif` / `else`)

```python
def is_even(n):
    if n % 2 == 0:
        return True
    else:
        return False
```

Conditionals create branching logic.

Mental model:

```
Condition → True path
          → False path
```

---

## 4️⃣ Loops: Teaching the Program to Repeat

### `for` Loop (Known Range / Iterable)

```python
def running_sum(nums):
    total = 0
    for n in nums:
        total += n
    return total
```

Use `for` when:

* Iterating over a list
* Looping a known number of times
* Processing a collection

---

### `while` Loop (Condition-Based)

```python
count = 0
while count < 5:
    print(count)
    count += 1
```

Use `while` when:

* You don’t know how many iterations ahead of time
* Loop depends on a condition changing dynamically

---

## 🔁 For vs While — Concrete Rule

> Use `for` when iterating over a collection.
> Use `while` when looping depends on a condition not tied to a fixed collection.

If you can rewrite it cleanly with `for`, you probably should.

---

## 5️⃣ Functions: Creating Reusable Units

Functions prevent duplication and improve clarity.

```python
def grade_score(score):
    if score >= 90:
        return "A"
    elif score >= 80:
        return "B"
    else:
        return "C"
```

A function has:

* Inputs (parameters)
* Logic (body)
* Output (return value)

Think of it as:

```
Input → Transformation → Output
```

---

## 6️⃣ Assertions: Your First Safety Net

Assertions verify expectations.

```python
assert is_even(2) is True
assert is_even(3) is False
```

If an assertion fails:

* Execution stops
* You immediately know something broke

Professional mindset:

> If it matters, assert it.

---

## 7️⃣ Clean Code Refactoring Principle

Bad:

```python
if n % 2 == 0:
    return True
else:
    return False
```

Better:

```python
return n % 2 == 0
```

Cleaner code:

* Removes redundancy
* Reduces indentation
* Improves readability

Refactoring is not rewriting — it is improving structure without changing behavior.

---

## 8️⃣ Common Beginner Mistakes

❌ Forgetting `return`
❌ Mutating variables unintentionally
❌ Infinite `while` loops
❌ Overcomplicating conditionals
❌ Writing logic outside reusable functions

---

## 9️⃣ Professional Pattern: Small Pure Functions

Good functions:

* Do one thing
* Have clear inputs
* Return predictable outputs
* Avoid hidden side effects

Example:

```python
def running_sum(nums):
    total = 0
    for n in nums:
        total += n
    return total
```

It depends only on `nums`.
It does not modify external state.
It is testable.

---

## 🔒 Day 02 Core Takeaway

> Control flow gives your program intelligence.
> Functions give your program structure.

When you combine both, you move from scripting to real programming.

---