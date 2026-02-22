# week-02-python-core - Day 06: Batch Iterator and Dataset Class

## Reading (5-15 minutes)
- [Iterator protocol docs](https://docs.python.org/3/library/stdtypes.html#iterator-types) - skim `__iter__` and `__next__`.
- [DataLoader concepts](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) - read concept section only.

## How To Read (2-3 minutes)
- Write one note separating batch size from sequence length.

## Build (Detailed Coding / Practice)
1. Create `week-02-python-core/code/day06_batching.py`.
2. Implement `TextDataset` with `__len__` and `__getitem__`.
3. Implement `batch_iter(items, batch_size, drop_last=False)`.
4. Pad encoded sequences to fixed length with pad id and save 3 sample batches to `week-02-python-core/artifacts/day-06-batches.json`.
5. Add shape logging for each batch.

## Practice Drills
- Compare behavior with `drop_last=True` vs `False`.
- Test batch size 1 and batch size > dataset length.

## Done When
- [ ] Dataset and iterator both work.
- [ ] Padding is explicit and reproducible.
- [ ] Sample batch artifact exists.
