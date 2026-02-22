# Week 06 Neural Network Basics

Focus: Building and stabilizing small neural networks from first principles

## Week Mission
Build practical mastery of this week's concepts through code-first exercises, reproducible experiments, and documented takeaways.

## Prerequisites
- Previous week completed (or equivalent comfort with listed skills).
- Local Python environment ready (python, pip, virtual environment).
- Basic Git usage for tracking incremental progress.

## Learning Outcomes (Definition of Success)
- [ ] Implement forward and backward passes for a small network.
- [ ] Train with stable softmax and cross-entropy calculations.
- [ ] Apply regularization to reduce overfitting.
- [ ] Diagnose common instability symptoms in small NN training.

## Core Tasks
- [ ] 38. Learn perceptron and activation functions.
- [ ] 39. Implement a 2-layer neural network from scratch.
- [ ] 40. Implement backprop for the 2-layer network.
- [ ] 41. Learn softmax and implement it safely.
- [ ] 42. Build a small classifier on toy data.
- [ ] 43. Learn regularization: L2 and dropout.
- [ ] 44. Implement dropout in the 2-layer network.
- [ ] 45. Write a summary note on training stability.

## Day-by-Day Execution Blueprint
- Day 1: Read and skim core concepts, define terms, and write a one-page mental model in notes/.
- Day 2: Implement the first half of core coding tasks with minimal abstractions.
- Day 3: Finish remaining coding tasks and validate with simple tests or assertions.
- Day 4: Run controlled experiments, track metrics, and save artifacts.
- Day 5: Refactor for clarity (naming, structure, docstrings, small helper functions).
- Day 6: Write a technical summary note: what worked, what failed, and why.
- Day 7: Review, tighten deliverables, and prepare handoff-ready week outputs.

## Guided Build Project
Ship a no-framework 2-layer classifier with backprop, regularization toggles, and experiment logs.

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
- [ ] Backprop gradients validated against numerical approximations.
- [ ] Classifier beats random baseline by a large margin.
- [ ] At least one overfitting vs regularization comparison plot.

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
