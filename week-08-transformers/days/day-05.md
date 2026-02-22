# week-08-transformers - Day 05: Minimal Transformer Block

## Reading (5-15 minutes)
- [Encoder/decoder block breakdown](https://towardsdatascience.com/the-transformer-encoder-bidirectional-encoder-representations-from-transformers-8f55d6ef5a3a) - residual+norm sections.
- [LayerNorm docs](https://pytorch.org/docs/stable/generated/torch.nn.LayerNorm.html) - skim.

## How To Read (2-3 minutes)
- Write exact order: MHA -> residual+norm -> FFN -> residual+norm.

## Build (Detailed Coding / Practice)
1. Create `week-08-transformers/code/day05_transformer_block.py`.
2. Implement one decoder-style block with causal mask support.
3. Save forward shape trace to `artifacts/day-05-block-forward.txt`.

## Practice Drills
- Ablate residual once and compare output stats.

## Done When
- [ ] Block forward pass runs with correct shapes.

