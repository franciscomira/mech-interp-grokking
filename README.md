# Interpretability: reverse-engineering a small transformer

Mechanistic interpretability of a small transformer I train myself. The model is a 1-layer transformer trained on modular addition (`a + b mod 113`), which is known to "grok": it first memorises the training set, then, under weight decay, abruptly generalises by learning a Fourier-based algorithm. The goal is to reproduce that finding from scratch and document how the circuit forms, as a public portfolio piece.

Training runs on Google Colab; this repo holds code, notes, figures and the write-up.

## Repo layout

| Folder | Purpose |
|---|---|
| `papers/` | Reference papers and `READING_LIST.md` |
| `notebooks/` | Colab notebooks, numbered by phase |
| `src/` | Reusable Python: model config, training loop, analysis helpers |
| `figures/` | Exported plots for the write-up |
| `notes/` | Learning notes, one markdown file per phase |
| `writeup/` | Final blog post draft |

## Plan

### Phase 1 - Foundations (~1 week)
ARENA chapter 1, TransformerLens tutorials, grokking paper.

### Phase 2 - Train (~1 week)
Train a 1-layer transformer on `a + b mod 113` with TransformerLens `HookedTransformer`. Use weight decay until it groks. Log train/test loss and save checkpoints.

### Phase 3 - Analyse (~2 weeks)
Attention patterns, Fourier analysis of embeddings, activation patching and ablations, circuit formation across checkpoints.

### Phase 4 - Extend (optional, ~1 week)
A second task or a 2-layer model; compare circuits.

### Phase 5 - Publish (~1 week)
Clean the repo, write a blog post with interactive Plotly charts, share on LinkedIn and LessWrong, add to CV.

## Setup
Open `notebooks/01_setup_check.ipynb` in Google Colab (GPU runtime) to verify the environment. Local dependencies for the helper code are in `requirements.txt`.
