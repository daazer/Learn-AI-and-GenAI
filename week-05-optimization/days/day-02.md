# week-05-optimization - Day 02: Gradient Checker

## Reading (5-15 minutes)
- [CS231n gradient check](https://cs231n.github.io/neural-networks-3/) - gradient checks section.
- [NumPy allclose](https://numpy.org/doc/stable/reference/generated/numpy.allclose.html) - tolerance usage.

## How To Read (2-3 minutes)
- Set acceptable relative-error threshold before coding.

## Build (Detailed Coding / Practice)
1. Create `week-05-optimization/code/day02_gradcheck.py`.
2. Implement `grad_check(f, x, analytic_grad_fn)` with finite differences.
3. Log max relative error and pass/fail to `artifacts/day-02-gradcheck.txt`.

## Practice Drills
- Corrupt one gradient value intentionally and confirm fail.

## Done When
- [ ] Checker detects incorrect gradients.

