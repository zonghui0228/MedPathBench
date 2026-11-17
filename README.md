# MedPathBench

**MedPathBench** is a patient-centered benchmark designed to evaluate the performance of large language models (LLMs) across sequential clinical decision pathways.

Unlike conventional medical benchmarks that primarily assess independent questions, MedPathBench captures the dependencies between consecutive clinical decisions, enabling systematic evaluation of LLMs in multi-step clinical reasoning.

## 📚 Dataset Overview

MedPathBench consists of:

- **746** clinical cases
- **1,905** sequentially dependent questions
- **9** clinical decision scenarios
- **2-4** interconnected questions per clinical case

Each case contains a shared clinical context followed by a sequence of related questions. The benchmark is designed to assess whether LLMs can maintain accurate and consistent decisions throughout an entire clinical pathway.

## ✨ Key Features

- **Patient-centered organization:** Clinical questions are grouped around shared patient cases rather than treated as independent items.

- **Sequential decision evaluation:** Captures dependencies between consecutive clinical questions through multi-turn interactions.

- **Pathway-level assessment:** Evaluates whether models can successfully complete an entire sequence of clinical decisions.

- **Error propagation analysis:** Investigates performance degradation across increasingly complex decision pathways.

- **Comprehensive model comparison:** Supports comparisons across clinical scenarios, patient demographics, and model scales.

## 🗂️ Evaluation Framework

MedPathBench supports multi-turn evaluation of LLMs using the following metrics:

- **Single Step Accuracy (SSA):** Accuracy at the individual question level.
- **Pathway Completion Rate (PCR):** Proportion of clinical pathways in which all questions are answered correctly.
- **Performance Gap (PG):** Difference between single-step accuracy and pathway completion rate.

These metrics provide complementary perspectives on individual decision accuracy and overall pathway reliability.

## 📈 Model Performance Comparison

Performance comparison of question-level and case-level across different large language models in sequential clinical reasoning.

| Model | SSA (%) | PCR (%) | PG (%) |
|:---|:---:|:---:|:---:|
| Gemini-3.5-Flash | 95.17 [94.11–96.05] | 88.74 [86.46–90.88] | 6.43 |
| Gemini-3.1-Flash-lite | 92.28 [91.00–93.40] | 82.44 [79.62–85.12] | 9.84 |
| DeepSeek-V4-Pro | 94.33 [93.20–95.28] | 87.00 [84.45–89.41] | 7.33 |
| DeepSeek-V4-Flash | 93.44 [92.24–94.47] | 84.58 [81.77–87.27] | 8.85 |
| Claude-Opus-4.7 | 93.49 [92.29–94.51] | 84.99 [82.44–87.53] | 8.50 |
| Claude-Opus-4.8 | 93.33 [92.12–94.37] | 84.58 [81.77–87.13] | 8.75 |
| GPT-5.5 | 92.60 [91.34–93.69] | 83.24 [80.29–85.92] | 9.35 |
| GPT-5.4 | 88.29 [86.77–89.66] | 75.60 [72.65–78.95] | 12.69 |
| Qwen3.5-27B | 92.02 [90.72–93.15] | 81.77 [78.82–84.45] | 10.25 |
| Qwen3.5-35B-A3B | 91.76 [90.44–92.91] | 81.23 [78.42–84.05] | 10.53 |


## 📬 Contact

For questions about the dataset or benchmark, please contact the zonghui0228@163.com.
