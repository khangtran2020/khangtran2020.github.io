---
title: "Gradient Transformer: Learning to Generate Updates for LLMs"
collection: publications
category: conferences
permalink: /publication/icml-2026b
# excerpt: 'This paper is about fixing template issue #693.'
date: 2026-05-01
venue: 'The 43th International Conference on Machine Learning'
# paperurl: 'https://arxiv.org/pdf/2604.17715'
# citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

Authors
======
N. Nguyen*, K. Tran*, I. Khalil, N.H. Phan (* Co-first author)

------

Abstract
======

Many organizations lack computational resources to fine-tune large language models (LLMs) on private (unshareable) data for better utility, while fine-tuning tiny language models (TinyLMs) alone performs poorly. To address this bottleneck, we propose a data-free knowledge distillation framework that generates LLM update vectors based on TinyLMs fine-tuned on private data. An update vector is a vector of parameter changes from an initial model to its fine-tuned version on a dataset, capturing the effect of cumulative gradient steps during fine-tuning. The key idea of our framework is a novel Gradient Transformer that transforms TinyLM’s update vectors into LLM’s update vectors. As derived from shadow datasets, GRAD-TRANSFORMER captures the correlation between TinyLM and LLM update vectors, enabling third-party providers to generate LLM update vectors given the organization’s TinyLM update vectors without accessing the organization’s private data. The framework supports multi-organization collaboration to jointly update LLMs, improving performance and cost-efficiency. Extensive experiments across language modeling and reasoning tasks show that GRAD-TRANSFORMER remarkably outperforms state-of-the-art knowledge distillation baselines, even under strict differential privacy protection. 
