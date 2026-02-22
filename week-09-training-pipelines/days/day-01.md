# week-09-training-pipelines - Day 01: Padding and Masks

## Reading (5-15 minutes)
- [Attention mask glossary](https://huggingface.co/docs/transformers/glossary#attention-mask) - skim.
- [pad_sequence docs](https://pytorch.org/docs/stable/generated/torch.nn.utils.rnn.pad_sequence.html) - concept.

## How To Read (2-3 minutes)
- Write one rule: padded tokens must not affect loss.

## Build (Detailed Coding / Practice)
1. Create `week-09-training-pipelines/code/day01_padding_masking.py`.
2. Implement `pad_batch` and `make_attention_mask` for variable-length sequences.
3. Save sample batch+mask to `artifacts/day-01-pad-mask.json`.

## Practice Drills
- Assert mask sum equals non-pad token count.

## Done When
- [ ] Padding/mask utilities work and are verified.

