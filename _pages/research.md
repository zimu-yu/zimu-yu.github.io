---
layout: single
title: "Research"
permalink: /research/
description: "Research projects by Zimu Yu in protein fitness landscapes, epistasis, protein design, and single-cell representation learning."
---

My research focuses on machine learning for computational biology, particularly protein fitness landscapes, mutational epistasis, protein engineering, and representation learning for biological data.

---

## From single-sequence structure prediction to protein fitness landscapes through a composable, epistasis-aware mutation atlas

**Cerebra-Epistasis · 2026**  
*bioRxiv preprint; under review at Nature Machine Intelligence*

Cerebra-Epistasis is an end-to-end, structure-aware framework for multi-mutant fitness prediction. It encodes a wild-type protein once to construct a reusable mutation atlas containing single-mutation effects and epistatic representations, which can then be assembled to predict arbitrary-order mutant fitness and epistasis. This design enables efficient exploration of large combinatorial fitness landscapes without repeatedly encoding every mutant sequence.

**My contribution.** I co-designed the framework and designed and implemented the fitness and epistasis modeling system downstream of Cerebra-Seq, including the mutation atlas, additive-effect modeling, higher-order epistasis modeling, and arbitrary-order component assembly. I also conducted model training, benchmarking, structural and epistasis analyses, figure preparation, and manuscript development.

[Code](https://github.com/Gonglab-THU/Cerebra) · [Publication details](/publications/#publications-2026)

---

## Deciphering the cellular sequence-metabolite synthetic landscape enables predictive design by MetaAI

**MetaAI · 2026**  
*Under review at Nature Microbiology*

MetaAI studies how sparse experimentally measured variants can be used to reconstruct cellular sequence–metabolite landscapes and predict unseen combinatorial mutations. By integrating sequence and structure-related representations with higher-order interaction modeling, the framework supports low-data prediction of mutant fitness, epistasis, and high-performing protein variants.

**My contribution.** I proposed and implemented the arbitrary-order epistasis modeling component and designed higher-order factorization methods for modeling combinatorial mutation effects. I also contributed to low-N benchmarking, computational analyses, and evaluation of higher-order mutation prediction.

[Code](https://github.com/xulab-research/MetaAI-research) · [Publication details](/publications/#publications-2026)

---

## RADAR enables marker-free fine-grained discovery of anomalous cells in multi-sample and multimodal single-cell omics

**RADAR · 2026**  
*Manuscript under review*

RADAR is a generative framework for marker-free discovery of anomalous cell populations across multi-sample and multimodal single-cell datasets. It integrates anomalous-cell detection, cross-sample and cross-modal alignment, and fine-grained anomalous-cell resolution within a unified three-stage framework.

**My contribution.** I co-implemented the framework and experimental pipeline, conducted extensive benchmarking and downstream analyses across scRNA-seq, scATAC-seq, and spatial transcriptomics datasets, prepared figures and results, and contributed substantially to manuscript development.

[Code](https://github.com/Catchxu/RADAR) · [Publication details](/publications/#publications-2026)

---

## Causality-Induced Positional Encoding for Transformer-Based Representation Learning of Non-Sequential Features

**CAPE · NeurIPS 2025**

CAPE introduces causality-aware positional encoding for Transformer models operating on non-sequential features. It learns latent causal structure among features, embeds the resulting causal graph in hyperbolic space, and transforms these representations into rotary positional encodings for self-attention.

**My contribution.** I conducted benchmark and baseline experiments and evaluated comparative performance across synthetic and real-world multi-omics datasets.

[Paper](https://proceedings.neurips.cc/paper_files/paper/2025/hash/e16657b9f07021c5554bf9661f18dfcc-Abstract-Conference.html) · [Code](https://github.com/Catchxu/CAPE)
