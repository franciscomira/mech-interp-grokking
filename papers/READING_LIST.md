# Reading list

## Local copies (this folder)
- `nanda2023_grokking_progress_measures.pdf` - Nanda et al., *Progress measures for grokking via mechanistic interpretability* (arXiv 2301.05217)
- `elhage2021_mathematical_framework.html` - Elhage et al., *A Mathematical Framework for Transformer Circuits*
- `olsson2022_induction_heads.html` - Olsson et al., *In-context Learning and Induction Heads*

## Online
- ARENA (arena.education): https://www.arena.education/ - Chapter 1: Transformer Interpretability: https://arena-chapter1-transformer-interp.streamlit.app/
- TransformerLens docs: https://transformerlensorg.github.io/TransformerLens/
- TransformerLens tutorials / Main Demo (Colab): https://colab.research.google.com/github/TransformerLensOrg/TransformerLens/blob/main/demos/Main_Demo.ipynb
- TransformerLens repo (demos folder): https://github.com/TransformerLensOrg/TransformerLens/tree/main/demos
- Neel Nanda, Mechanistic Interpretability Explainer & Glossary: https://www.neelnanda.io/mechanistic-interpretability/glossary
- Neel Nanda, Getting Started in Mechanistic Interpretability: https://www.neelnanda.io/mechanistic-interpretability/getting-started
- Neel Nanda, A Mechanistic Interpretability Analysis of Grokking (blog post, key reference for Phase 3 Fourier analysis): https://www.alignmentforum.org/posts/N6WM6hs7RQMKDhYjB/a-mechanistic-interpretability-analysis-of-grokking (link from memory, not verified; also linked from the glossary's Grokking entry)

## Phase 1: glossary reading order (about 60-90 min)
The glossary is about 220k characters. Use it as a reference, not a linear read. Note: "residual stream" has no entry of its own; it is defined under Transformer Basics.

1. Intro, "how to read"
2. MI General: features, circuit, intervening
3. Linear Algebra: basis, activation space, residual stream space
4. Basic Concepts: logits, softmax, cross-entropy
5. Training Dynamics: memorisation, generalisation, phase transition, grokking
6. Transformer Basics; Components: LayerNorm, unembedding, MLP
7. Attention Heads: head steps, information routing
8. Math Framework entries: QK-Circuit, OV-Circuit, Composition, Freezing attention patterns
9. Superposition (skim)
10. Techniques: ablation, logit lens, direct logit attribution, activation patching, logit difference
11. Optional: induction head, previous-token head

Skip for now: BERTology, scaling laws, positional-embedding variants, RMSNorm, encoder-decoder models, RLHF, SoLU, IOI, PCA/t-SNE/probing, notable models, BPE details.
