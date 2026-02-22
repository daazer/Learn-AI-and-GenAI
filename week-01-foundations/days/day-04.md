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
