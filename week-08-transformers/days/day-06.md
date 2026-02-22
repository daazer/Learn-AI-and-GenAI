# week-08-transformers - Day 06: Train Tiny Transformer

## Reading (5-15 minutes)
- [nanoGPT README](https://github.com/karpathy/nanoGPT) - skim config/training flow.
- [Causal LM task guide](https://huggingface.co/docs/transformers/tasks/language_modeling) - causal section.

## How To Read (2-3 minutes)
- Set tiny config explicitly before coding: context, heads, layers, dim.

## Build (Detailed Coding / Practice)
1. Create `week-08-transformers/code/day06_train_tiny_transformer.py`.
2. Train on character data, log train/val loss, and save checkpoint.
3. Store checkpoint + curve in `artifacts/day-06-*`.

## Practice Drills
- Resume once from checkpoint to verify recovery.

## Done When
- [ ] Training loop runs and checkpoint is loadable.

