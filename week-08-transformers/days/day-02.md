# week-08-transformers - Day 02: Scaled Dot-Product Attention

## Reading (5-15 minutes)
- [Annotated transformer attention](https://nlp.seas.harvard.edu/2018/04/03/attention.html) - scaled-dot formula.
- [Masking concept](https://huggingface.co/docs/transformers/glossary#attention-mask) - skim.

## How To Read (2-3 minutes)
- Write why dividing by sqrt(d_k) stabilizes softmax.

## Build (Detailed Coding / Practice)
1. Create `week-08-transformers/code/day02_scaled_attention.py`.
2. Implement `scaled_dot_attention(Q,K,V,mask=None)` with stable softmax and masking.
3. Save test log to `artifacts/day-02-attention-tests.txt`.

## Practice Drills
- Test with and without causal mask.

## Done When
- [ ] Function supports masking and passes shape checks.

