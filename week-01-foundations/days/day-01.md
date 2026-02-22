# week-01-foundations - Day 01: Python Environment and Repo Scaffolding

## Reading (5-15 minutes)
- [Python venv docs](https://docs.python.org/3/library/venv.html) - read "Creating virtual environments".
- [Packaging guide: pip + venv](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/) - focus on activation and install commands.

## How To Read (2-3 minutes)
- Write down the 4 commands you must memorize: create venv, activate, install, freeze requirements.

## Build (Detailed Coding / Practice)
1. Create `week-01-foundations/code/hello_env.py` that prints `sys.version` and `sys.executable`.
2. Create `week-01-foundations/code/requirements.txt` with `numpy` and `matplotlib`.
3. Run `python -m venv .venv`, activate, and run `pip install -r week-01-foundations/code/requirements.txt`.
4. Run `python week-01-foundations/code/hello_env.py` and save output to `week-01-foundations/artifacts/day-01-output.txt`.
5. Document exact setup commands in `week-01-foundations/notes/setup.md`.

## Practice Drills
- Deactivate and reactivate environment once to verify you can recover quickly.
- Run `pip list` and confirm packages are installed in the venv.

## Done When
- [ ] `hello_env.py` runs successfully.
- [ ] `notes/setup.md` is copy-pasteable.
- [ ] `artifacts/day-01-output.txt` exists.

---

# 📘 Learnbook Chapter 01 — Python Environments & Why They Matter

## 1️⃣ What Problem Are We Solving?

When you install Python packages globally:

- Projects conflict
- Versions break each other
- System Python becomes messy
- Reproducibility disappears

A **virtual environment (venv)** solves this by creating an isolated Python installation **per project**.

Think of it as:

> One project = One sandboxed Python world.

---

## 2️⃣ What `venv` Actually Does

When you run:

```bash
python -m venv .venv
````

Python:

* Creates a new folder `.venv/`
* Copies or symlinks the Python interpreter
* Creates its own `site-packages`
* Adds activation scripts

After activation, `pip install` installs packages **inside that folder only**.

---

## 3️⃣ The Commands You Must Memorize

These are foundational. Burn them into memory.

### Create environment

```bash
python -m venv .venv
```

### Activate (Mac/Linux)

```bash
source .venv/bin/activate
```

### Activate (Windows)

```bash
.venv\Scripts\activate
```

### Install packages

```bash
pip install -r requirements.txt
```

### Freeze current environment

```bash
pip freeze > requirements.txt
```

If you know these commands, you can recover any Python project.

---

## 4️⃣ What `sys.version` and `sys.executable` Teach You

Your script:

```python
import sys
print(sys.version)
print(sys.executable)
```

Teaches you:

* Which Python version is running
* Which interpreter path is being used

If activation worked correctly, `sys.executable` should point inside:

```
.../.venv/bin/python
```

If it doesn’t — you are NOT inside the virtual environment.

This is your debugging signal.

---

## 5️⃣ Mental Model: Python Layers

Think in layers:

```
Your Code
↓
Installed Packages (numpy, matplotlib)
↓
Virtual Environment
↓
System Python
↓
Operating System
```

Each layer isolates risk.

---

## 6️⃣ Reproducibility Principle

A professional project must be:

* Cloneable
* Installable
* Runnable

From scratch.

This is why `requirements.txt` exists.

Without it:

* You cannot reproduce results.
* Your project is fragile.

With it:

* Any machine can recreate your environment in minutes.

---

## 7️⃣ Common Beginner Mistakes

❌ Installing packages without activating venv
❌ Forgetting to commit `requirements.txt`
❌ Committing the entire `.venv` folder
❌ Not verifying `sys.executable`

---

## 8️⃣ Professional Standard Setup Flow

```bash
git clone <repo>
cd project
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python main.py
```

If your project supports this flow, you are operating at professional baseline.

---

## 🔒 Day 01 Core Takeaway

> A Python project without an isolated environment is not a real project.

You now control your runtime.

That’s step one toward engineering discipline.

---

```

If you’d like, I can standardize a **chapter template** so every day has:
- Concept
- Mental model
- Commands
- Failure cases
- Professional practice
- Reflection questions

That would turn this into a cohesive learnbook instead of daily notes.
```
