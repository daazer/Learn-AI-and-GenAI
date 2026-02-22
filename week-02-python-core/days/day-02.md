# week-02-python-core - Day 02: CSV and JSON Handling

## Reading (5-15 minutes)
- [Python csv docs](https://docs.python.org/3/library/csv.html) - read DictReader/DictWriter usage.
- [Python json docs](https://docs.python.org/3/library/json.html) - read dump/load examples.

## How To Read (2-3 minutes)
- Write one sentence: when CSV is better than JSON and vice versa.

## Build (Detailed Coding / Practice)
1. Create `week-02-python-core/code/day02_csv_json.py`.
2. Create `week-02-python-core/artifacts/books.csv` with `title,author,year`.
3. Parse CSV into list of dicts, then save to `books.json`.
4. Implement `filter_by_year(records, min_year)` and print results.
5. Save transformed output summary to `week-02-python-core/artifacts/day-02-convert.md`.

## Practice Drills
- Add one malformed row and handle/record the failure clearly.
- Sort by year descending before writing JSON.

## Done When
- [ ] CSV->JSON conversion works.
- [ ] Filter function works on sample input.
- [ ] Summary markdown exists.
