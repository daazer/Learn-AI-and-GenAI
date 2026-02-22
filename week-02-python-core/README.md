# Week 02 Python Core

Focus: Data handling and NLP-ready preprocessing pipelines

## Week Mission
Build practical mastery of this week's concepts through code-first exercises, reproducible experiments, and documented takeaways.

## Prerequisites
- Previous week completed (or equivalent comfort with listed skills).
- Local Python environment ready (python, pip, virtual environment).
- Basic Git usage for tracking incremental progress.

## Learning Outcomes (Definition of Success)
- [ ] Read and write common data formats safely.
- [ ] Implement reusable text preprocessing components.
- [ ] Create a small vocabulary system with encode/decode support.
- [ ] Write basic tests for deterministic preprocessing behavior.

## Core Tasks
- [ ] 8. Learn file I/O, CSV, JSON handling.
- [ ] 9. Implement a data loader for text files.
- [ ] 10. Implement tokenization by splitting and by regex.
- [ ] 11. Implement a character vocabulary and index mapping.
- [ ] 12. Implement a simple batch iterator.
- [ ] 13. Learn Python OOP basics and write a Dataset class.
- [ ] 14. Learn unit testing basics and test the tokenizer.
- [ ] 15. Write a summary note on data pipelines.

## Day-by-Day Execution Blueprint
- Day 1: Read and skim core concepts, define terms, and write a one-page mental model in notes/.
- Day 2: Implement the first half of core coding tasks with minimal abstractions.
- Day 3: Finish remaining coding tasks and validate with simple tests or assertions.
- Day 4: Run controlled experiments, track metrics, and save artifacts.
- Day 5: Refactor for clarity (naming, structure, docstrings, small helper functions).
- Day 6: Write a technical summary note: what worked, what failed, and why.
- Day 7: Review, tighten deliverables, and prepare handoff-ready week outputs.

## Guided Build Project
Build a tiny text preprocessing package (loader, tokenizer, vocab, batcher) with unit tests and sample outputs.

## Deliverables
- notes/
- code/
- artifacts/

## Minimum File Outputs
- notes/theory-summary.md
- notes/mistakes-and-fixes.md
- notes/weekly-retrospective.md
- code/run_all (script or notebook)
- artifacts/results.md

## Quality Checklist
- [ ] Tokenizer tests pass with edge cases.
- [ ] Vocabulary encode/decode is reversible for in-vocab text.
- [ ] Sample mini-batches are logged under artifacts/.

## Reflection Prompts
- Which concept still feels intuitive weak, and what concrete example clarified it?
- Which implementation detail caused the most bugs, and how was it fixed?
- Which metric best indicated progress this week, and why?
- What should be simplified before building on this in the next week?

## Stretch Goals (Optional)
- Add one extra experiment that changes a meaningful assumption.
- Compare two implementation strategies and document tradeoffs.
- Add simple automation (Makefile or script) to run repetitive steps.

## End-of-Week Gate
Mark the week complete only when:
- All core tasks are checked.
- Deliverables exist in notes/, code/, and artifacts/.
- You can explain the week's key idea in plain language without notes.


## Daily Learning Guides
- Day 01: [`days/day-01.md`](days/day-01.md) - File I/O with Pathlib
- Day 02: [`days/day-02.md`](days/day-02.md) - CSV and JSON Handling
- Day 03: [`days/day-03.md`](days/day-03.md) - Recursive Text Loader
- Day 04: [`days/day-04.md`](days/day-04.md) - Tokenization: Split vs Regex
- Day 05: [`days/day-05.md`](days/day-05.md) - Character Vocabulary Mapping
- Day 06: [`days/day-06.md`](days/day-06.md) - Batch Iterator and Dataset Class
- Day 07: [`days/day-07.md`](days/day-07.md) - Pytest + Pipeline Summary
