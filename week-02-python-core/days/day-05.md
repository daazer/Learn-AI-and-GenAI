# week-02-python-core - Day 05: Character Vocabulary Mapping

## Reading (5-15 minutes)
- [Python dictionaries refresher](https://docs.python.org/3/tutorial/datastructures.html#dictionaries) - quick read.
- [HF tokenization intro](https://huggingface.co/learn/nlp-course/chapter6/1) - skim why vocab mapping matters.

## How To Read (2-3 minutes)
- Write why deterministic vocab ordering matters for checkpoint compatibility.

## Build (Detailed Coding / Practice)
1. Create `week-02-python-core/code/day05_vocab.py`.
2. Implement class `CharVocab` with `fit`, `encode`, `decode`.
3. Reserve id 0=`<unk>`, id 1=`<pad>`.
4. Run round-trip tests on in-vocab strings and unknown-char tests.
5. Save vocab stats to `week-02-python-core/artifacts/day-05-vocab.json`.

## Practice Drills
- Verify unknown chars map to `<unk>` id.
- Assert decode(encode(x)) == x for in-vocab text.

## Done When
- [ ] Class supports fit/encode/decode.
- [ ] Unknown mapping path is tested.
- [ ] Vocab artifact exists.
