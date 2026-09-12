---
layout: single
title: "Research"
permalink: /research/
description: "Research projects by Zimu Yu in protein fitness landscapes, epistasis, protein design, and single-cell representation learning."
---

I develop and evaluate computational models for biological data, from combinatorial protein variants to heterogeneous cell populations.

## Cerebra-Epistasis

**Reusable mutation representations for protein fitness landscapes**

Predicting each protein variant independently can make it difficult to explore large combinatorial landscapes. Cerebra-Epistasis builds a reusable mutation atlas from a single wild-type protein encoding and assembles mutation-specific components to predict multi-mutant fitness and epistasis.

**My contribution.** I co-designed the initial framework and implemented the fitness and epistasis system downstream of Cerebra-Seq, including additive-effect, higher-order epistasis, mutation-atlas, and component-assembly modules. I also conducted training, benchmarking, result analysis, and manuscript work.

*Protein fitness · Higher-order epistasis · Structure-aware learning*

[Code](https://github.com/Gonglab-THU/Cerebra-Epistasis) · [Manuscript details](/publications/#publications-2026)

## MetaAI

**Sequence–metabolite landscape learning from sparse observations**

Experimental measurements cover only a small fraction of possible mutation combinations. MetaAI studies how sequence and structural representations can support landscape reconstruction, higher-order epistasis prediction, and the design of protein variants from limited data.

**My contribution.** I designed and implemented the computational modeling component for sequence–metabolite landscape reconstruction, epistasis prediction, and protein-variant design.

*Low-data learning · Landscape reconstruction · Protein engineering*

[Code](https://github.com/xulab-research/MetaAI-research) · [Manuscript details](/publications/#publications-2026)

## RADAR

**Marker-free discovery of anomalous cells**

Cell populations vary across samples and measurement modalities. RADAR provides a framework for marker-free anomalous-cell detection, cross-sample and cross-modal alignment, and fine-grained analysis of single-cell omics.

**My contribution.** I co-implemented the framework and codebase, conducted experiments and analyses, prepared results and figures, and contributed to manuscript writing and revision.

*Single-cell omics · Anomaly detection · Multimodal learning*

[Code](https://github.com/Catchxu/RADAR) · [Manuscript details](/publications/#publications-2026)

## CAPE

**Causality-aware positional encoding for non-sequential features**

Many biological features do not have a natural sequence order, but still have dependencies that matter for learning. CAPE investigates causality-induced positional encoding for Transformer-based representation learning of non-sequential features.

**My contribution.** I ran benchmark and baseline experiments and evaluated comparative performance across synthetic and real-world multi-omics datasets.

*Representation learning · Transformers · Multi-omics*  
**NeurIPS 2025**

[Paper](https://proceedings.neurips.cc/paper_files/paper/2025/hash/e16657b9f07021c5554bf9661f18dfcc-Abstract-Conference.html) · [Code](https://github.com/Catchxu/CAPE)
