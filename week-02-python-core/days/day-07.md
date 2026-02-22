# week-02-python-core - Day 07: Pytest + Pipeline Summary

## Reading (5-15 minutes)
- [pytest getting started](https://docs.pytest.org/en/stable/getting-started.html) - read first example.
- [Python testing guide](https://realpython.com/python-testing/) - skim organization section.

## How To Read (2-3 minutes)
- Write one rule for deterministic preprocessing tests.

## Build (Detailed Coding / Practice)
1. Create `week-02-python-core/code/test_tokenizer.py` and `test_vocab.py`.
2. Write at least 6 tests covering tokenization, unknown chars, and round-trip decode.
3. Run `python -m pytest week-02-python-core/code -q` and save output to `week-02-python-core/artifacts/day-07-test-output.txt`.
4. Write `week-02-python-core/notes/theory-summary.md` describing raw text -> tokens -> ids -> batches.
5. Write `week-02-python-core/notes/weekly-retrospective.md` with brittle points and fixes.

## Practice Drills
- Intentionally break one test, observe failure, then fix it.
- Add one regression test for a bug found this week.

## Done When
- [ ] At least 6 tests run.
- [ ] Test-output artifact exists.
- [ ] Theory summary explains full pipeline clearly.
