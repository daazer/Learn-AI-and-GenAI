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
