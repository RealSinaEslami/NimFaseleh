---
license: cc-by-sa-4.0
language:
  - fa
pretty_name: Nim Faseleh Corpus (Persian ZWNJ Corpus)
size_categories:
  - 10K<n<20K
task_categories:
  - text-classification
  - token-classification
  - fill-mask
task_ids:
  - grammatical-error-correction
  - morphological-analysis
  - language-modeling
---

# 📚 Nim Faseleh Corpus (Persian Zero-Width Non-Joiner Dataset)

## 🎯 Objective

The Nim Faseleh Corpus is designed to comprehensively cover Persian **Zero-Width Non-Joiner (ZWNJ)** usage patterns and compound word formations.

ZWNJ is one of the most critical yet under-addressed challenges in Persian Natural Language Processing. This dataset provides more than 14,000 standardized samples to support research and development in this area.

---

## 🔍 Why this dataset?

In Persian text, correct ZWNJ usage directly impacts both **grammatical correctness** and **semantic meaning**.

For example:

- «نمی‌روم» (correct) vs «نمی روم» (incorrect)
- «خودکارنویس» (correct) vs «خودکار نویس» (different meaning)

This dataset can serve as a **gold standard corpus** for training and evaluating text normalization and correction models.

---

## 📁 Dataset Structure

The data is provided in a CSV file named `Nim_Faseleh_Corpus.csv`.

| Column            | Type   | Description                              | Example     |
|------------------|--------|------------------------------------------|-------------|
| Word             | string | Word or compound expression              | آب‌انبار    |
| Category         | string | Lexical category (noun/adjective/etc.)   | Noun        |
| Starting_Letter  | string | First character for grouping             | آ           |
| Length           | int    | Number of characters                     | 8           |
| Is_Compound      | int    | Indicates ZWNJ/compound structure (0/1)  | 1           |
| Component_Count  | int    | Number of word components                | 2           |

---

## 📊 Statistics

- Total samples: 14,000+
- Full coverage of Persian alphabet (32 letters)
- Includes nouns, adjectives, verbs, adverbs, and idiomatic compounds
- Balanced structural diversity across compound formations

---

## 💡 Applications

1. **Text Normalization Models**  
   Training systems that convert informal or incorrect Persian text into standardized form.

2. **ZWNJ Evaluation Benchmark**  
   A benchmark dataset for evaluating the performance of Persian NLP models.

3. **ASR / TTS Post-processing**  
   Improving transcription quality in speech systems by enforcing orthographic consistency.

---

## 📜 License

This dataset is released under the **Creative Commons Attribution-ShareAlike 4.0 (CC BY-SA 4.0)** license.

---

## ✍️ Citation

If you use this dataset in your research, please cite it as follows:

```bibtex
@misc{NimFaseleh,
  author = {Sina Eslami},
  title = {Nim Faseleh Corpus: Persian Zero-Width Non-Joiner Dataset},
  year = {2026},
  publisher = {Hugging Face},
  url = {https://huggingface.co/datasets/AmirScorpion/NimFaseleh}
}

🤝 Contribution

Feedback, issues, and contributions are highly welcome.
Please use the Issues section to report problems or suggest improvements.

⭐ If you find this dataset useful, consider giving it a star to support the project.
