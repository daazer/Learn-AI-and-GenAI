# week-02-python-core - Day 01: File I/O with Pathlib

## Reading (5-15 minutes)
- [Python pathlib docs](https://docs.python.org/3/library/pathlib.html) - skim file read/write methods.
- [Python I/O tutorial](https://docs.python.org/3/tutorial/inputoutput.html#reading-and-writing-files) - read context-manager examples.

## How To Read (2-3 minutes)
- Write one rule for text vs binary mode in pipelines.

## Build (Detailed Coding / Practice)
1. Create `week-02-python-core/code/day01_fileio.py`.
2. Implement `read_text(path)` and `write_text(path, text)` using `pathlib.Path`.
3. Create `week-02-python-core/artifacts/sample_input.txt` with 5 lines.
4. Write line/char counts to `week-02-python-core/artifacts/day-01-summary.json`.
5. Add clean missing-file handling in code.

## Practice Drills
- Temporarily rename file and verify error handling branch.
- Run script twice and confirm deterministic output.

## Done When
- [ ] Summary JSON exists.
- [ ] Helpers are reusable functions.
- [ ] Missing-file error is explicit and controlled.
