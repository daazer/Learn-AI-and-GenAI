# week-09-training-pipelines - Day 02: Dataset Splits + Eval Loop

## Reading (5-15 minutes)
- [Cross-validation basics](https://scikit-learn.org/stable/modules/cross_validation.html) - skim split rationale.
- [Training/eval loop concept](https://pytorch.org/tutorials/beginner/introyt/trainingyt.html) - eval section.

## How To Read (2-3 minutes)
- Write one anti-leakage rule for splitting.

## Build (Detailed Coding / Practice)
1. Create `week-09-training-pipelines/code/day02_split_eval.py`.
2. Implement seeded train/val/test split and evaluation loop returning avg loss + metric.
3. Save split counts and metrics to `artifacts/day-02-split-eval.md`.

## Practice Drills
- Check ID overlap across splits is zero.

## Done When
- [ ] Split and eval loop are deterministic and leakage-free.

