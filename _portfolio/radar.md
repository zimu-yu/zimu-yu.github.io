---
title: "RADAR enables marker-free fine-grained discovery of anomalous cells in multi-sample and multimodal single-cell omics"
collection: portfolio
order: 2
excerpt: >-
  RADAR discovers anomalous cell populations across samples and single-cell omics modalities without predefined markers or annotated references. Its three-stage framework detects anomalous cells, separates biological heterogeneity from technical variation, and resolves the detected cells into biologically coherent subtypes.
  <br /><a href="/research/radar/"><img src="/images/research/radar-overview.png" alt="RADAR framework overview" width="80%" loading="lazy" /></a>
---

<figure>
  <a href="{{ '/images/research/radar-overview.png' | relative_url }}"><img src="{{ '/images/research/radar-overview.png' | relative_url }}" alt="RADAR framework overview" /></a>
</figure>

Disease-associated cell populations and states can be absent from healthy reference tissues, yet difficult to identify without known markers. Differences between samples and measurement modalities further complicate their discovery by obscuring biological heterogeneity with technical variation.

RADAR is a generative adversarial framework that combines anomalous-cell detection, cross-sample and cross-modal alignment, and fine-grained subtype resolution. It does not require annotated reference cells and can transfer information from scRNA-seq references to less common omics modalities.

Evaluations across modalities, platforms, species, tissues, and diseases demonstrate its ability to discover anomalous cells and distinguish their compositional heterogeneity across samples. The framework supports analyses of scRNA-seq, scATAC-seq, and spatial transcriptomics data.

**Status:** Manuscript under review.

[Code](https://github.com/Catchxu/RADAR)
