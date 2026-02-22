# week-09-training-pipelines - Day 06: Gradient Clipping

## Reading (5-15 minutes)
- [clip_grad_norm docs](https://pytorch.org/docs/stable/generated/torch.nn.utils.clip_grad_norm_.html) - read usage.
- [Exploding gradients recap](https://neptune.ai/blog/understanding-gradient-clipping-and-how-it-can-fix-exploding-gradients-problem) - skim.

## How To Read (2-3 minutes)
- Write where clipping is applied in train step order.

## Build (Detailed Coding / Practice)
1. Create `week-09-training-pipelines/code/day06_grad_clip.py`.
2. Train one high-LR run without clipping and one with clipping; log gradient norms.
3. Save CSV + plot to `artifacts/day-06-gradnorm.*`.

## Practice Drills
- Compare thresholds 0.5 vs 1.0.

## Done When
- [ ] Gradient clipping impact is measured and documented.

