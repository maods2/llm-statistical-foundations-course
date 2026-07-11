# Interactive Notebooks — Statistical Foundations of LLMs

Interactive Jupyter notebooks accompanying the lecture slides.Each notebook opens with a 2-minute Jupyter primer and alternates explanatory Markdown, runnable code, visual output, and exercises with optional solutions.

## How to run

Everything is sized for the **free Google Colab tier** (CPU works; a T4 GPU speeds up the fine-tuning lab). Open a notebook in Colab, run cells top to bottom with **Shift + Enter**. The first code cell of each notebook runs `%pip install` for any missing packages (restart the kernel if prompted).

All LLM work uses **open models** (BioGPT, FLAN-T5, GPT-2, DistilBERT, T5-small) — **no API keys required**. Where a notebook can optionally use GPT-4, those cells are clearly marked and disabled by default.

## The notebooks

| Lab | File | Slides | Topic |
|---|------|--------|-------|
| 00 | `00_getting_started.ipynb` | — | **Start here if you're new to Python/Jupyter.** Full Colab walkthrough: opening, running cells, editing, fixing errors |
| Lab 1 | `lab1_ngram_language_models.ipynb` | 76–79 | N-gram language models: counting, MLE, generation, smoothing, perplexity |
| Lab 2 | `lab2_word_embeddings.ipynb` | 93–96 | Word embeddings: Word2Vec vs. GloVe, analogies, PCA, polysemy |
| Lab 3 | `lab3_small_transformers.ipynb` | 201–205 | One input, three architectures: DistilBERT / GPT-2 / T5 |
| Lab 4 | `lab4_finetuning_bert.ipynb` | 246–247 | Fine-tuning BERT for sentiment (transfer learning, Trainer API) |
| Lab 5 | `lab5_prompt_engineering.ipynb` | 275–278 | Prompt engineering for biomedical abstracts |
| Lab 6 | `lab6_uncertainty_inference.ipynb` | 307–308 | Uncertainty & statistical inference in LLMs (bootstrap, entropy, tests) |
| Lab 7 | `lab7_watermarking.ipynb` | 343–344 | Embedding & detecting LLM watermarks (green-list + binomial z-test) |
| Case Study | `case_study_hallucinations_bias.ipynb` | 347–349 | When LLMs go wrong: hallucinations, inconsistency, bias |

## Common structure

Every notebook follows the course style guide: Title → Learning objectives → Jupyter primer → Background → Imports → step-by-step examples → interactive exercises → challenge exercises → discussion questions → key takeaways → references. Random seeds are set for reproducibility.


Pre-run solution notebooks (with outputs) are in [`solutions_executed/`](solutions_executed/).
