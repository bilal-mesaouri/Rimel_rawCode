# Rimel_rawCode

This repository contains multiple notebooks and analyses addressing various sub-questions about code generation models’ performance on different benchmarks (BigCodeBench, HumanEval, etc.).

---

## 1. Sub-question: Instruction Fine-tuning Impact on Results

- **Main Notebook:** [Instruction Fine-tuning Impact](https://colab.research.google.com/drive/1zavfs-BUJ0X7YmQ_1EJ1Fh4w0fV6oFBe?usp=sharing)
- **Raw Exploration:** [Raw Notebook](https://colab.research.google.com/drive/1i4UI3um5qACOXF0urY7AxvsgPH5zT88v?usp=sharing)
- **Unfinished Experiment on Model Size Impact:** [Model Size Exploration](https://colab.research.google.com/drive/1hcDSzSYkVeEBgM4kHqZahygHm57A5JND?usp=sharing)

---

## 2. Sub-question: How Does Specialization in a Specific Programming Language Influence Benchmark Performance?

- **Notebook:** [Language Specialization Analysis](https://colab.research.google.com/drive/1qhC_mFKfJUFnXG6jE7TSVWtb75IFQuOs?usp=sharing)

---

## 3. Sub-question: Are “Coder” Models Particularly Sensitive to “Complete” vs. “Instruct” Prompts?

We hypothesize that explicitly labeled *“Coder”* models (e.g., StarCoder, DeepSeek-Coder, etc.) might behave differently when evaluated on “complete” vs. “instruct” tasks, due to their specialized focus on code generation.

**Notebook:**
- [Coder Models Analysis](https://colab.research.google.com/drive/1fC87v9_g7mKbjfQGnMqj6HpzRqxYkXre?usp=sharing)

### Quick Summary
- **Objective:**  
  Filter “Coder” models from BigCodeBench and compare their “complete” vs. “instruct” scores.
- **Average Gap:**  
  Approximately 9 points difference (complete – instruct), similar to non-“Coder” models overall.
- **Size Influence:**  
  Larger “Coder” models (≥50 B) tend to show a bigger gap (>10 points).
- **Conclusion:**  
  Despite their specialization, “Coder” models still generally exhibit “complete > instruct.” Future work could investigate the proportion of instruction-like data in their pre-training and how that affects performance.

---
