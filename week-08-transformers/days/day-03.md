# week-08-transformers - Day 03: Multi-Head Attention

## Reading (5-15 minutes)
- [Transformer paper section 3.2](https://arxiv.org/abs/1706.03762) - read multi-head paragraph.
- [PyTorch MHA docs](https://pytorch.org/docs/stable/generated/torch.nn.MultiheadAttention.html) - concept level.

## How To Read (2-3 minutes)
- Note why multiple heads can capture different relations.

## Build (Detailed Coding / Practice)
1. Create `week-08-transformers/code/day03_multihead.py`.
2. Implement projection to heads, scaled attention per head, and concat+output projection.
3. Save shape validation to `artifacts/day-03-multihead-shapes.md`.

## Practice Drills
- Run with 1 and 4 heads; compare params.

## Done When
- [ ] Multi-head output shapes are correct.

