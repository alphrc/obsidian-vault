---
paper id: 2412.00789v4
title: "A Cognac Shot To Forget Bad Memories: Corrective Unlearning for Graph Neural Networks"
authors:
  - Varshita Kolipaka
  - Akshit Sinha
  - Debangan Mishra
  - Sumit Kumar
  - Arvindh Arun
  - Shashwat Goel
  - Ponnurangam Kumaraguru
publication date: 2024-12-01T12:23
abstract: Graph Neural Networks (GNNs) are increasingly being used for a variety of ML applications on graph data. Because graph data does not follow the independently and identically distributed (i.i.d.) assumption, adversarial manipulations or incorrect data can propagate to other data points through message passing, which deteriorates the model's performance. To allow model developers to remove the adverse effects of manipulated entities from a trained GNN, we study the recently formulated problem of Corrective Unlearning. We find that current graph unlearning methods fail to unlearn the effect of manipulations even when the whole manipulated set is known. We introduce a new graph unlearning method, Cognac, which can unlearn the effect of the manipulation set even when only 5% of it is identified. It recovers most of the performance of a strong oracle with fully corrected training data, even beating retraining from scratch without the deletion set while being 8x more efficient. We hope our work assists GNN developers in mitigating harmful effects caused by issues in real-world data, post-training. Our code is publicly available at https://github.com/cognac-gnn-unlearning/corrective-unlearning-for-gnns
comments: In Proceedings of ICML 2025
pdf: "[[Literature Notes/pdfs/A Cognac Shot To Forget Bad Memories Corrective Unlearning for Graph Neural Networks (2412.00789v4).pdf]]"
url: https://arxiv.org/abs/2412.00789v4
tags:
---
