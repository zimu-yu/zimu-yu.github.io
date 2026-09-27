---
title: "From single-sequence structure prediction to protein fitness landscape through a composable, epistasis-aware mutation atlas"
collection: portfolio
order: 1
excerpt: >-
  Cerebra-Epistasis links single-sequence structure prediction to multi-mutant fitness modeling through a reusable, epistasis-aware mutation atlas. Encoding the wild-type protein once allows mutation components to be assembled into predictions for higher-order mutants without repeated sequence or structure encoding.
  <br /><a href="/research/cerebra-epistasis/"><img src="/images/research/cerebra-epistasis-overview.png" alt="Cerebra-Epistasis framework overview" width="80%" loading="lazy" /></a>
---

<figure>
  <a href="{{ '/images/research/cerebra-epistasis-overview.png' | relative_url }}"><img src="{{ '/images/research/cerebra-epistasis-overview.png' | relative_url }}" alt="Cerebra-Epistasis framework overview" /></a>
</figure>

Predicting the effects of multiple mutations requires modeling epistasis: interactions that make their combined effect differ from the sum of individual effects. Cerebra-Epistasis couples a single-sequence structure predictor with a fitness model that jointly represents additive and epistatic effects, placing these interactions in a three-dimensional structural context.

The framework encodes a wild-type protein once to construct a mutation-indexed atlas of single-mutation scores and epistatic representations. An assembly module retrieves and combines these components to predict fitness and epistasis for arbitrary-order mutants, making large combinatorial landscapes accessible without encoding every mutant separately.

Across diverse assays, the model extrapolated from low-order measurements to unseen higher-order combinations and recovered experimentally observed epistatic patterns, including interactions between spatially close residues.

**Status:** bioRxiv preprint, 2026. Under review at Nature Biotechnology.

[Preprint](https://doi.org/10.64898/2026.09.24.753701) · [Code](https://github.com/xulab-research/Cerebra-Epistasis) · [Server](https://structpred.life.tsinghua.edu.cn/server_cerebra_epistasis.html)
