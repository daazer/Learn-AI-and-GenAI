# week-04-probability-stats - Day 06: Entropy, Cross-Entropy, KL

## Reading (5-15 minutes)
- [Entropy intuition](https://www.youtube.com/watch?v=YtebGVx-Fxw) - first 10 min.
- [SciPy entropy docs](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.entropy.html) - formula/examples.

## How To Read (2-3 minutes)
- Note clearly that KL is asymmetric.

## Build (Detailed Coding / Practice)
1. Create `week-04-probability-stats/code/day06_information.py`.
2. Implement entropy/cross_entropy/kl with epsilon guard.
3. Save metric comparisons to `artifacts/day-06-information.csv`.

## Practice Drills
- Verify KL(p||p) ~= 0 and KL(p||q) != KL(q||p).

## Done When
- [ ] Metrics implemented safely with asymmetry demo.

