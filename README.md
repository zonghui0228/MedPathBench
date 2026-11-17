# MedPathBench

**MedPathBench** is a patient-centered benchmark designed to evaluate the performance of large language models (LLMs) across sequential clinical decision pathways.

Unlike conventional medical benchmarks that primarily assess independent questions, MedPathBench captures the dependencies between consecutive clinical decisions, enabling systematic evaluation of LLMs in multi-step clinical reasoning.

## Dataset Overview

MedPathBench consists of:

- **746** clinical cases
- **1,905** sequentially dependent questions
- **9** clinical decision scenarios
- **2-4** interconnected questions per clinical case

Each case contains a shared clinical context followed by a sequence of related questions. The benchmark is designed to assess whether LLMs can maintain accurate and consistent decisions throughout an entire clinical pathway.

## Evaluation Framework

MedPathBench supports multi-turn evaluation of LLMs using the following metrics:

- **Single Step Accuracy (SSA):** Accuracy at the individual question level.
- **Pathway Completion Rate (PCR):** Proportion of clinical pathways in which all questions are answered correctly.
- **Performance Gap (PG):** Difference between single-step accuracy and pathway completion rate.

These metrics provide complementary perspectives on individual decision accuracy and overall pathway reliability.

## Contact

For questions about the dataset or benchmark, please contact the corresponding authors.
