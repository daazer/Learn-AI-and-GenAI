# Week 08 Transformers

Focus: Attention-first architecture and autoregressive text generation

## Week Mission
Build practical mastery of this week's concepts through code-first exercises, reproducible experiments, and documented takeaways.

## Prerequisites
- Previous week completed (or equivalent comfort with listed skills).
- Local Python environment ready (python, pip, virtual environment).
- Basic Git usage for tracking incremental progress.

## Learning Outcomes (Definition of Success)
- [ ] Understand attention mathematically and operationally.
- [ ] Implement core transformer components from scratch.
- [ ] Train a tiny autoregressive transformer and sample text.
- [ ] Explain why attention architecture scales effectively.

## Core Tasks
- [ ] 53. Learn attention mechanism and intuition.
- [ ] 54. Implement scaled dot product attention.
- [ ] 55. Implement multi-head attention.
- [ ] 56. Implement positional encoding.
- [ ] 57. Build a minimal transformer block.
- [ ] 58. Train a tiny transformer on character data.
- [ ] 59. Implement autoregressive generation.
- [ ] 60. Write a summary note on why attention scales.

## Day-by-Day Execution Blueprint
- Day 1: Read and skim core concepts, define terms, and write a one-page mental model in notes/.
- Day 2: Implement the first half of core coding tasks with minimal abstractions.
- Day 3: Finish remaining coding tasks and validate with simple tests or assertions.
- Day 4: Run controlled experiments, track metrics, and save artifacts.
- Day 5: Refactor for clarity (naming, structure, docstrings, small helper functions).
- Day 6: Write a technical summary note: what worked, what failed, and why.
- Day 7: Review, tighten deliverables, and prepare handoff-ready week outputs.

## Guided Build Project
Build a tiny GPT-like character model with one or more transformer blocks and text sampling utilities.

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
- [ ] Attention and masking logic validated with shape/unit checks.
- [ ] Loss decreases consistently over training steps.
- [ ] Generated samples improve after training.

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
