# Interactive Notebooks — Statistical Foundations of LLMs

Interactive Jupyter notebooks accompanying the lecture slides (`presentation/RodriguesPC_LLM (1).pptx`). Designed for a graduate audience, including participants who have **never used Python or Jupyter** before. Each notebook opens with a 2-minute Jupyter primer and alternates explanatory Markdown, runnable code, visual output, and exercises with optional solutions.

## How to run

Everything is sized for the **free Google Colab tier** (CPU works; a T4 GPU speeds up the fine-tuning lab). Open a notebook in Colab, run cells top to bottom with **Shift + Enter**. The first code cell of each notebook runs `%pip install` for any missing packages (restart the kernel if prompted).

All LLM work uses **open models** (BioGPT, FLAN-T5, GPT-2, DistilBERT, T5-small) — **no API keys required**. Where a notebook can optionally use GPT-4, those cells are clearly marked and disabled by default.

## The notebooks

| # | File | Slides | Topic |
|---|------|--------|-------|
| 00 | `00_getting_started.ipynb` | — | **Start here if you're new to Python/Jupyter.** Full Colab walkthrough: opening, running cells, editing, fixing errors |
| 01 | `01_activity_slides_75_76.ipynb` | 75–80 | N-gram language models: counting, MLE, generation, smoothing, perplexity |
| 02 | `02_activity_slides_93_94.ipynb` | 93–94 | Word embeddings: Word2Vec vs. GloVe, analogies, PCA, polysemy |
| 03 | `03_activity_slides_192_199.ipynb` | 192–199 | Fine-tuning BERT for sentiment (transfer learning, Trainer API) |
| 04 | `04_activity_slides_252_260.ipynb` | 252–260 | One input, three architectures: DistilBERT / GPT-2 / T5 |
| 05 | `05_session3_prompt_engineering.ipynb` | Session 3 | Prompt engineering for biomedical abstracts |
| 06 | `06_activity_slides_321_323.ipynb` | 321–323 | Uncertainty & statistical inference in LLMs (bootstrap, entropy, tests) |
| 07 | `07_activity_slides_357_358.ipynb` | 357–360 | Embedding & detecting LLM watermarks (green-list + binomial z-test) |
| 08 | `08_case_study_hallucinations_bias.ipynb` | Responsible use | When LLMs go wrong: hallucinations, inconsistency, bias |

## Common structure

Every notebook follows the course style guide: Title → Learning objectives → Jupyter primer → Background → Imports → step-by-step examples → interactive exercises → challenge exercises → discussion questions → key takeaways → references. Random seeds are set for reproducibility.

See `COURSE_SUGGESTIONS.md` for proposed improvements to the slide deck and course flow.

Pre-run solution notebooks (with outputs) are in [`solutions_executed/`](solutions_executed/).
