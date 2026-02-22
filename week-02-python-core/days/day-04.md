# week-02-python-core - Day 04: Tokenization: Split vs Regex

## Reading (5-15 minutes)
- [Python regex howto](https://docs.python.org/3/howto/regex.html) - focus on split/findall.
- [spaCy tokenization notes](https://spacy.io/usage/linguistic-features#tokenization) - skim conceptual section.

## How To Read (2-3 minutes)
- Write one sentence about why whitespace split is insufficient.

## Build (Detailed Coding / Practice)
1. Create `week-02-python-core/code/day04_tokenizer.py`.
2. Implement `tokenize_split(text)` and `tokenize_regex(text)`; regex should preserve punctuation tokens.
3. Test with 4 strings including contractions and punctuation.
4. Save side-by-side comparison in `week-02-python-core/artifacts/day-04-tokenizer-compare.md`.
5. Document one known failure case in code comments.

## Practice Drills
- Add a URL/email case and inspect tokenizer behavior.
- Count token lengths and compare variants.

## Done When
- [ ] Both tokenizer versions run.
- [ ] Comparison artifact exists.
- [ ] At least one limitation is documented.
