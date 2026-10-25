# Contributing

Thanks for helping grow this list! Please open a PR or an issue with the paper/blog link.

## Scope

Foundation models for biology that are **unified**: one model covering multiple molecular modalities (DNA, RNA, protein, small molecules, cells, text), multiple scales, or multiple tasks. Single-modality models are in scope only if they explicitly target cross-modality generalization (e.g. central-dogma genomic models).

## Entry format

Add the entry to the right section, **newest first**:

```markdown
- **ModelName**: Full Paper Title [![Paper](https://img.shields.io/badge/Paper-b31b1b)](PAPER_URL) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](CODE_URL) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](HF_URL) <br> *Organization* · Venue YYYY · `YYYY-MM` · `DNA` `Protein` `Text`
```

For works without a paper, prefix with 🌐 and use the Blog badge:

```markdown
- 🌐 **ModelName**: Short description [![Blog](https://img.shields.io/badge/Blog-0A66C2)](BLOG_URL) <br> *Organization* · `YYYY-MM` · `Protein` `Cell`
```

Rules:
- Omit badges for links that don't exist.
- Date is the first public release (preprint or blog), not the publication date.
- Use preprint venue (`arXiv`, `bioRxiv`) until a peer-reviewed venue exists, then update it.
- Modality tags: `DNA` `RNA` `Protein` `Molecule` `Structure` `Cell` `Text` `Image`.
