# week-02-python-core - Day 03: Recursive Text Loader

## Reading (5-15 minutes)
- [os.walk docs](https://docs.python.org/3/library/os.html#os.walk) - read recursion example.
- [NLTK text processing chapter](https://www.nltk.org/book/ch03.html) - skim tokenization context only.

## How To Read (2-3 minutes)
- Note why stable sort order matters for reproducible training.

## Build (Detailed Coding / Practice)
1. Create `week-02-python-core/code/day03_loader.py`.
2. Implement `load_texts(root_dir)` to recursively load `.txt` files in sorted order.
3. Create test corpus under `week-02-python-core/artifacts/corpus/` with nested dirs and 3+ files.
4. Return list records: `path`, `text`, `n_chars`.
5. Save dataset stats to `week-02-python-core/artifacts/day-03-loader-summary.md`.

## Practice Drills
- Ensure non-txt files are skipped.
- Verify repeated runs produce same file ordering.

## Done When
- [ ] Recursive loader works for nested folders.
- [ ] Summary file includes counts and total chars.
- [ ] Output ordering is deterministic.
