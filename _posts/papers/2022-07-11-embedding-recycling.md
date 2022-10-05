---
layout: paper
categories: papers
permalink: papers/embedding_recycling
id: embedding_recycling
title: "ColBERTv2: Effective and Efficient Retrieval via Lightweight Late Interaction"
authors: 
  - Keshav Santhanam*
  - Omar Khattab*
  - Jon Saad-Falcon
  - Christopher Potts
  - Matei Zaharia
venue: Preprint, under review
venue-shorthand: Preprint, under review
url: /papers/embedding_recycling
pdf: https://arxiv.org/abs/2112.01488
type: conference
image: /images/papers/ColBERTv2.png
figure: /images/featured/ColBERTv2.png
feature-title: "ColBERTv2"
feature-description: "Effective and Efficient Retrieval via Lightweight Late Interaction"
featured: true
feature-order: 4
selected: true
bibtex: |-

  @misc{santhanam2021colbertv2,
      title={ColBERTv2: Effective and Efficient Retrieval via Lightweight Late Interaction}, 
      author={Keshav Santhanam and Omar Khattab and Jon Saad-Falcon and Christopher Potts and Matei Zaharia},
      year={2021},
      eprint={2112.01488},
      archivePrefix={arXiv},
      primaryClass={cs.IR}
  }
  
---

Neural information retrieval (IR) has greatly advanced search and other knowledge-intensive language tasks. While many neural IR methods encode queries and documents into single-vector representations, late interaction models produce multi-vector representations at the granularity of each token and decompose relevance modeling into scalable token-level computations. This decomposition has been shown to make late interaction more effective, but it inflates the space footprint of these models by an order of magnitude. In this work, we introduce ColBERTv2, a retriever that couples an aggressive residual compression mechanism with a denoised supervision strategy to simultaneously improve the quality and space footprint of late interaction. We evaluate ColBERTv2 across a wide range of benchmarks, establishing state-of-the-art quality within and outside the training domain while reducing the space footprint of late interaction models by 5--8×.
