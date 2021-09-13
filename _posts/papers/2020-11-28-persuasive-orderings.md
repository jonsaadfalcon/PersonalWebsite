---
layout: paper
categories: papers
permalink: papers/persuasive-orderings
id: persuasive-orderings
title: "Examining the Ordering of Rhetorical Strategies in Persuasive Requests"
authors: 
  - Omar Shaikh 
  - Jiaao Chen
  - Jon Saad-Falcon
  - Duen Horng (Polo) Chau
  - Diyi Yang
venue: "Findings of the Association for Computational Linguistics: Empirical Methods in Natural Language Processing"
venue-shorthand: EMNLP Findings
year: 2020
url: /papers/persuasive-orderings
pdf: https://arxiv.org/abs/2010.04625
video: https://youtu.be/O-CTpLLb4gA
code: https://github.com/GT-SALT/persuasive-orderings
type: conference
figure: /images/papers/20-persuasion-strat.png
image: /images/featured/20-persuasion-strat.png
feature-title: "Rhetorical Strategies"
feature-description: "Examining the Ordering of Rhetorical Strategies in Persuasive Requests"
featured: true
feature-order: 1
selected: true
bibtex: |-

  @inproceedings{shaikh-etal-2020-examining,
    title = "Examining the Ordering of Rhetorical Strategies in Persuasive Requests",
    author = "Shaikh, Omar  and
      Chen, Jiaao  and
      Saad-Falcon, Jon  and
      Chau, Polo  and
      Yang, Diyi"
    booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2020",
    month = nov,
    year = "2020",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2020.findings-emnlp.116",
    pages = "1299--1306",
  }
---

Interpreting how persuasive language influences audiences has implications across many domains like advertising, argumentation, and propaganda. Persuasion relies on more than a message's content. Arranging the order of the message itself (i.e., ordering specific rhetorical strategies) also plays an important role. To examine how strategy orderings contribute to persuasiveness, we first utilize a Variational Autoencoder model to disentangle content and rhetorical strategies in textual requests from a large-scale loan request corpus. We then visualize interplay between content and strategy through an attentional LSTM that predicts the success of textual requests. We find that specific (orderings of) strategies interact uniquely with a request's content to impact success rate, and thus the persuasiveness of a request.

