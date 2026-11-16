<div align="center">

# Awesome Unified Biology Foundation Models [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**A curated list of papers, technical reports, and blogs on _unified_ foundation models for biology: models that span multiple molecular modalities (DNA, RNA, protein, small molecules, cells, text) and scales.**

![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)
![License: CC0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)
![Last Commit](https://img.shields.io/github/last-commit/Steven51516/awesome-unified-bio-fm)

</div>

> [!NOTE]
> 🔥 Entries are sorted **newest first** within each section. Works released only as blogs, websites, or model cards (no paper) are welcome and marked with 🌐.
> Missing something? Open an issue or PR (see [CONTRIBUTING.md](CONTRIBUTING.md)).

## 📰 News

- **2026-10**: Repository created with the first 26 entries.

## 📑 Table of Contents

- [Tokenizers](#-tokenizers)
- [Unified Biology LLMs](#-unified-biology-llms)
  - [Multi-Modality / Generalist](#multi-modality--generalist)
  - [Genomics](#genomics)
  - [Protein](#protein)
  - [Cell & Tissue](#cell--tissue)
- [Structure Prediction & Generation](#-structure-prediction--generation)
  - [All-Atom](#all-atom)
  - [Protein](#protein-1)
- [Benchmarks & Analyses](#-benchmarks--analyses)
- [Inspiration: General-Domain Unified Multimodal Generation](#-inspiration-general-domain-unified-multimodal-generation)

## Legend

| Badge | Meaning |
| --- | --- |
| ![Paper](https://img.shields.io/badge/Paper-b31b1b) | arXiv / bioRxiv / journal paper |
| ![Code](https://img.shields.io/badge/Code-181717?logo=github) | Official code |
| ![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black) | Released weights |
| ![Blog](https://img.shields.io/badge/Blog-0A66C2) | Blog post / project page |
| 🌐 | No paper; blog, website, or model card only |

---

## 🧩 Tokenizers

*Discrete tokenizers that turn biological structures and cell states into tokens a language model can read and write.*

- **ADT**: All-Atom Diffusion Tokenizer for 3D Molecular Structures [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2610.23265) <br> *PKU, Shanghai AI Lab, CUHK* · arXiv · `2026-10` · `Protein` `Molecule` `Structure`
- **SLL**: Learning Latent Protein Languages for Autoregressive Generation [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2610.03978) <br> *University of Missouri* · arXiv · `2026-10` · `Protein`
- **ProFiT**: Flow-Matching-Based Protein Structure Tokenizer Made Efficient and Easy [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2609.33129) <br> *Tsinghua AIR* · arXiv · `2026-09` · `Protein` `Structure`
- **APT**: Adaptive Protein Tokenization [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2602.06418) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/rdilip/apt) <br> *Caltech (Van Valen Lab)* · arXiv · `2026-02` · `Protein` `Structure`
- **StructGPT**: From Static Structures to Ensembles: Studying and Harnessing Protein Structure Tokenization [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2511.10056) <br> *IDEA* · arXiv · `2025-11` · `Protein` `Structure`
- **GCP-VQVAE**: A Geometry-Complete Language for Protein 3D Structure [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.1101/2025.10.01.679833) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/mahdip72/vq_encoder_decoder) <br> *University of Missouri* · bioRxiv · `2025-10` · `Protein` `Structure`
- **StructTokBench**: Protein Structure Tokenization: Benchmarking and New Recipe [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2503.00089) <br> *Yuan et al.* · arXiv · `2025-03` · `Protein` `Structure`
- **Mol-StrucTok**: Tokenizing 3D Molecule Structure with Quantized Spherical Coordinates [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2412.01564) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/KyGao/Mol-StrucTok) <br> *Gao et al.* · arXiv · `2024-12` · `Molecule` `Structure`

## 🧬 Unified Biology LLMs

*Single LLMs that read and write biological modalities natively, via a shared vocabulary, early-fusion tokens, or biology-as-text, including LLMs that reason in language and drive structure generation.*

### Multi-Modality / Generalist

- **Trion-1**: Unifying Language, Protein Sequence, and Structure with Diffusion Language Models [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2610.31215) <br> *Tsinghua (GenSI Lab)* · arXiv · `2026-10` · `Protein` `Structure` `Text`
- **SciReasoner (native structural reasoning)**: Accurate, Interdisciplinary and Transparent Structure-property Understanding with Deep Native Structural Reasoning [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2607.07708) <br> *Shanghai AI Lab* · arXiv · `2026-07` · `Protein` `Molecule` `Structure` `Text`
- **BioMatrix**: Towards a Comprehensive Biological Foundation Model Spanning the Modality Matrix of Sequences, Structures, and Language [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2606.22138) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/QizhiPei/BioMatrix) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/collections/QizhiPei/biomatrix) <br> *Renmin Univ., Shanghai AI Lab* · arXiv · `2026-06` · `Protein` `Molecule` `Structure` `Text`
- **LOGOS**: Speaking the Language of Science: Toward a General-Purpose Generative Foundation Model for the Natural Sciences [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2606.16905) <br> *Alibaba* · arXiv · `2026-06` · `Protein` `Molecule` `Structure`
- **SciReasoner**: Laying the Scientific Reasoning Ground Across Disciplines [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2509.21320) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/open-sciencelab/SciReason) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/SciReason) <br> *Shanghai AI Lab* · arXiv · `2025-09` · `DNA` `RNA` `Protein` `Molecule` `Text`
- **TxGemma**: Efficient and Agentic LLMs for Therapeutics [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2504.06196) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/collections/google/txgemma-release-67dd92e931c857d15e4d1e87) [![Blog](https://img.shields.io/badge/Blog-0A66C2)](https://developers.google.com/health-ai-developer-foundations/txgemma) <br> *Google* · arXiv · `2025-04` · `DNA` `RNA` `Protein` `Molecule` `Cell` `Text`
- **Uni-3D-AR**: Unified Cross-Scale 3D Generation and Understanding via Autoregressive Modeling [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2503.16278) <br> *Lu et al.* · arXiv · `2025-03` · `Molecule` `Protein` `Structure`
- **NExT-Mol**: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2502.12638) <br> *Liu et al.* · ICLR 2025 · `2025-02` · `Molecule` `Structure`

### Genomics

- 🌐 **Carbon-X**: Open DNA-understanding LLM built on Qwen3-14B [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/HuggingFaceBio/Carbon-X) [![Blog](https://img.shields.io/badge/Blog-0A66C2)](https://huggingface.co/spaces/HuggingFaceBio/Carbon-X-Release) <br> *Hugging Face* · Blog · `2026-10` · `DNA` `Text`

### Protein

- **COS**: Chain of Structures: Connecting Reasoning and Generation for Protein Design [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.64898/2026.10.09.758133) <br> *Scinetics, HKUST* · bioRxiv · `2026-10` · `Protein` `Structure` `Text`
- **Prompteina**: Designing Protein Structures from Natural Language [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2610.13917) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/jleechung/prompteina) <br> *University of Washington* · arXiv · `2026-10` · `Protein` `Structure` `Text`
- **Fold2Reason**: Does Learning Protein Folding Generalize to Broader Reasoning? [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2609.38879) <br> *GENTEL Lab* · arXiv · `2026-09` · `Protein` `Structure` `Text`
- **Proteo-R1**: Reasoning Foundation Models for De Novo Protein Design [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2605.02937) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/smiles724/Proteo-R1) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/thinking-bio-lab/proteor1-generate) [![Blog](https://img.shields.io/badge/Blog-0A66C2)](https://smiles724.github.io/r1/) <br> *Stanford, UTokyo/RIKEN, CUHK* · ICML 2026 · `2026-05` · `Protein` `Structure` `Text`
- **ProteinReasoner**: Modality-chain reasoning enables multimodal protein modelling and design [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.1101/2025.07.21.665832) <br> *Liu et al.* · bioRxiv · `2025-07` · `Protein` `Structure`
- **Pinal**: Programmable design of functional proteins from natural language [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://doi.org/10.1038/s41586-026-11205-z) <br> *Westlake University* · Nature 2026 · `2024-08` · `Protein` `Structure` `Text`
- **ESM3**: Simulating 500 million years of evolution with a language model [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.1101/2024.07.01.600583) <br> *EvolutionaryScale* · Science 2025 · `2024-07` · `Protein` `Structure` `Text`

### Cell & Tissue

- **TissueNarrator**: Generative Modeling of Spatial Transcriptomics with Large Language Models [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.1101/2025.11.24.690325) <br> *CMU* · bioRxiv · `2025-11` · `Cell` `Text`
- **CellTok**: Early-Fusion Multimodal Large Language Model for Single-Cell Transcriptomics via Tokenization [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.1101/2025.10.22.684047) <br> *Tsinghua, Alibaba* · bioRxiv · `2025-10` · `Cell` `Text`
- **C2S-Scale**: Scaling Large Language Models for Next-Generation Single-Cell Analysis [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.1101/2025.04.14.648850) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/vandijklab/cell2sentence) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/vandijklab/C2S-Scale-Gemma-2-27B) <br> *Yale, Google* · bioRxiv · `2025-04` · `Cell` `Text`
- **Cell2Sentence**: Teaching Large Language Models the Language of Biology [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.1101/2023.09.11.557287) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/vandijklab/cell2sentence) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/vandijklab/pythia-160m-c2s) <br> *Yale* · ICML 2024 · `2023-09` · `Cell` `Text`

## 🧊 Structure Prediction & Generation

*Structure models that serve as the structural backbone of unified biology systems.*

### All-Atom

- **RFD4-Proteina**: All-atom generative design across proteins, nucleic acids, sugars, and modified residues [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://rfd4-proteina.org/assets/paper/RFD4-Proteina.pdf) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/RosettaCommons/RFD4-Proteina) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/nvidia/RFD4-Proteina) [![Blog](https://img.shields.io/badge/Blog-0A66C2)](https://rfd4-proteina.org/) <br> *UW IPD (Baker Lab), NVIDIA* · Preprint · `2026-10` · `Protein` `DNA` `RNA` `Molecule` `Structure`
- **OpenDDE**: Folding, Reasoning, and Scaling with Open-source Drug Discovery Engine [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2607.03787) <br> *Aureka AI Research* · arXiv · `2026-07` · `Protein` `Molecule` `Structure`
- **Protenix-v2**: Broadening the Reach of Structure Prediction and Biomolecular Design [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.64898/2026.04.10.717613) <br> *ByteDance Seed* · bioRxiv · `2026-04` · `Protein` `Molecule` `Structure`
- **Boltz-1**: Democratizing Biomolecular Interaction Modeling [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.1101/2024.11.19.624167) <br> *MIT* · bioRxiv · `2024-11` · `Protein` `Molecule` `Structure`
- **AlphaFold 3**: Accurate Structure Prediction of Biomolecular Interactions with AlphaFold 3 [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.nature.com/articles/s41586-024-07487-w) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/google-deepmind/alphafold3) <br> *Google DeepMind, Isomorphic Labs* · Nature 2024 · `2024-05` · `Protein` `DNA` `RNA` `Molecule` `Structure`

### Protein

- **AtlasFold**: Protein structure prediction with metagenomic-scale language models [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.64898/2026.09.04.749352) <br> *KAIST* · bioRxiv · `2026-09` · `Protein` `Structure`
- **ESMFold2**: Language Modeling Materializes a World Model of Protein Biology [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.64898/2026.06.03.729735) <br> *EvolutionaryScale* · bioRxiv · `2026-06` · `Protein` `Structure`
- **Proteina-Complexa**: Scaling Atomistic Protein Binder Design with Generative Pretraining and Test-Time Compute [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2603.27950) <br> *NVIDIA* · ICLR 2026 · `2026-03` · `Protein` `Structure`
- **PAR**: Protein Autoregressive Modeling via Multiscale Structure Generation [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2602.04883) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/bytedance-Seed/par-protein) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/collections/ByteDance-Seed/par) [![Blog](https://img.shields.io/badge/Blog-0A66C2)](https://par-protein.github.io/) <br> *ByteDance Seed* · ICML 2026 · `2026-02` · `Protein` `Structure`
- **PPIFlow**: High-Affinity Protein Binder Design via Flow Matching and In Silico Maturation [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.64898/2026.01.19.700484) <br> *Changping Laboratory* · bioRxiv · `2026-01` · `Protein` `Structure`
- **SimpleFold**: Folding Proteins is Simpler than You Think [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2509.18480) <br> *Apple* · arXiv · `2025-09` · `Protein` `Structure`
- **Ambient Proteins**: Training Diffusion Models on Low Quality Structures [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.1101/2025.07.03.663105) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/jozhang97/ambient-proteins) <br> *UT Austin* · bioRxiv · `2025-07` · `Protein` `Structure`
- **La-Proteina**: Atomistic Protein Generation via Partially Latent Flow Matching [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2507.09466) <br> *NVIDIA* · ICLR 2026 · `2025-07` · `Protein` `Structure`
- **APM**: An All-Atom Generative Model for Designing Protein Complexes [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2504.13075) <br> *Chen et al.* · arXiv · `2025-04` · `Protein` `Structure`
- **Proteina**: Scaling Flow-based Protein Structure Generative Models [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2503.00710) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/NVIDIA-Digital-Bio/proteina) [![Blog](https://img.shields.io/badge/Blog-0A66C2)](https://research.nvidia.com/labs/genair/proteina/) <br> *NVIDIA* · ICLR 2025 · `2025-03` · `Protein` `Structure`
- **DPLM-2**: A Multimodal Diffusion Protein Language Model [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2410.13782) <br> *ByteDance Research, Nanjing University* · arXiv · `2024-10` · `Protein` `Structure`
- **DPLM**: Diffusion Language Models Are Versatile Protein Learners [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2402.18567) <br> *ByteDance Research, Nanjing University* · ICML 2024 · `2024-02` · `Protein`

## 📊 Benchmarks & Analyses

*Benchmarks and analysis papers for evaluating unified biology models.*

- **BioMirage**: When Do Biological Reasoning Models Use Their Biological Inputs? [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2610.00898) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/mims-harvard/bio-mirage) [![Blog](https://img.shields.io/badge/Blog-0A66C2)](https://zitniklab.hms.harvard.edu/biomirage) <br> *Harvard (Zitnik Lab)* · arXiv · `2026-10` · `DNA` `Protein` `Cell` `Text`
- **PROTEAN**: Beyond De Novo Generation: Can LLM Agents Perform Text-Guided Protein Structure Editing? [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2610.17765) <br> *Shanghai AI Lab* · arXiv · `2026-10` · `Protein` `Structure` `Text`
- **FoldBench**: Benchmarking all-atom biomolecular structure prediction with FoldBench [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://www.biorxiv.org/content/10.1101/2025.05.22.655600) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/BEAM-Labs/FoldBench) <br> *BEAM Labs* · Nature Communications · `2025-05` · `Protein` `RNA` `DNA` `Molecule` `Structure`

## 🎨 Inspiration: General-Domain Unified Multimodal Generation

*Not biology models: unified understanding + generation architectures from vision-language that may transfer to biology.*

- **WeLM-Image**: A Unified Image Generation Model towards Visual Intelligence [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2611.07392) <br> *WeChat Vision, Tencent* · arXiv · `2026-11` · `Text` `Image`
- **UniAR**: Unified Multimodal Autoregressive Modeling with Shared Context-Visual Tokenizer is Key to Unification [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2606.18249) <br> *Peng et al.* · arXiv · `2026-06` · `Text` `Image`
- **Qwen-Image-2.0**: Qwen-Image-2.0 Technical Report [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2605.10730) [![Blog](https://img.shields.io/badge/Blog-0A66C2)](https://qwen.ai/blog?id=qwen-image-2.0) <br> *Alibaba Qwen* · arXiv · `2026-05` · `Text` `Image`
- **SenseNova-U1**: Unifying Multimodal Understanding and Generation with NEO-unify Architecture [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2605.12500) <br> *SenseTime* · arXiv · `2026-05` · `Text` `Image`
- 🌐 **GLM-Image**: Autoregressive + diffusion-decoder hybrid for knowledge-dense image generation [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/zai-org/GLM-Image) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/zai-org/GLM-Image) [![Blog](https://img.shields.io/badge/Blog-0A66C2)](https://z.ai/blog/glm-image) <br> *Z.ai* · Blog · `2026-01` · `Text` `Image`
- **Emu3.5**: Native Multimodal Models are World Learners [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2510.26583) <br> *BAAI* · arXiv · `2025-10` · `Text` `Image`
- **MANZANO**: A Simple and Scalable Unified Multimodal Model with a Hybrid Vision Tokenizer [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2509.16197) <br> *Apple* · arXiv · `2025-09` · `Text` `Image`
- **NextStep-1**: Toward Autoregressive Image Generation with Continuous Tokens at Scale [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2508.10711) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/stepfun-ai/NextStep-1) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/stepfun-ai/NextStep-1-Large) <br> *StepFun* · ICLR 2026 · `2025-08` · `Text` `Image`
- **BAGEL**: Emerging Properties in Unified Multimodal Pretraining [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2505.14683) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/ByteDance-Seed/Bagel) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/ByteDance-Seed/BAGEL-7B-MoT) [![Blog](https://img.shields.io/badge/Blog-0A66C2)](https://bagel-ai.org/) <br> *ByteDance Seed* · arXiv · `2025-05` · `Text` `Image`
- **Janus-Pro**: Unified Multimodal Understanding and Generation with Data and Model Scaling [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2501.17811) [![Code](https://img.shields.io/badge/Code-181717?logo=github)](https://github.com/deepseek-ai/Janus) [![Model](https://img.shields.io/badge/Model-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/deepseek-ai/Janus-Pro-7B) <br> *DeepSeek* · arXiv · `2025-01` · `Text` `Image`
- **Transfusion**: Predict the Next Token and Diffuse Images with One Multi-Modal Model [![Paper](https://img.shields.io/badge/Paper-b31b1b)](https://arxiv.org/abs/2408.11039) <br> *Meta* · arXiv · `2024-08` · `Text` `Image`
---

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for the entry format.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Steven51516/awesome-unified-bio-fm&type=Date)](https://star-history.com/#Steven51516/awesome-unified-bio-fm&Date)

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this work.
