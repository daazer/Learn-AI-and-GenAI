# Week 07 Language Models

Focus: Sequence modeling foundations from n-grams to simple recurrent networks

## Week Mission
Build practical mastery of this week's concepts through code-first exercises, reproducible experiments, and documented takeaways.

## Prerequisites
- Previous week completed (or equivalent comfort with listed skills).
- Local Python environment ready (python, pip, virtual environment).
- Basic Git usage for tracking incremental progress.

## Learning Outcomes (Definition of Success)
- [ ] Build and evaluate classical statistical language models.
- [ ] Compute perplexity consistently for text corpora.
- [ ] Implement a basic character-level RNN pipeline.
- [ ] Explain tradeoffs between n-grams and recurrent models.

## Core Tasks
- [ ] 46. Learn n-gram language models.
- [ ] 47. Implement a unigram and bigram model.
- [ ] 48. Implement smoothing for n-grams.
- [ ] 49. Evaluate perplexity on small text.
- [ ] 50. Build a simple RNN from scratch.
- [ ] 51. Train the RNN on character-level text.
- [ ] 52. Write a summary note on sequence modeling.

## Day-by-Day Execution Blueprint
- Day 1: Read and skim core concepts, define terms, and write a one-page mental model in notes/.
- Day 2: Implement the first half of core coding tasks with minimal abstractions.
- Day 3: Finish remaining coding tasks and validate with simple tests or assertions.
- Day 4: Run controlled experiments, track metrics, and save artifacts.
- Day 5: Refactor for clarity (naming, structure, docstrings, small helper functions).
- Day 6: Write a technical summary note: what worked, what failed, and why.
- Day 7: Review, tighten deliverables, and prepare handoff-ready week outputs.

## Guided Build Project
Create a language modeling mini-suite: n-gram baseline + character RNN with side-by-side evaluation.

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
- [ ] Perplexity reported for at least 2 modeling approaches.
- [ ] RNN generates coherent short character sequences.
- [ ] Smoothing improves bigram quality on sparse inputs.

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
- Day 01: [`days/day-01.md`](days/day-01.md) - N-gram LM Foundations
- Day 02: [`days/day-02.md`](days/day-02.md) - Unigram + Bigram Implementation
- Day 03: [`days/day-03.md`](days/day-03.md) - Smoothing
- Day 04: [`days/day-04.md`](days/day-04.md) - Perplexity Evaluation
- Day 05: [`days/day-05.md`](days/day-05.md) - RNN Cell From Scratch
- Day 06: [`days/day-06.md`](days/day-06.md) - Train Character RNN
- Day 07: [`days/day-07.md`](days/day-07.md) - Week 7 Synthesis
