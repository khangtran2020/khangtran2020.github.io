---
title: "Poison with Style: A Practical Poisoning Attack on Code Large Language Models"
collection: publications
category: conferences
permalink: /publication/icml-2026a
# excerpt: 'This paper is about fixing template issue #693.'
date: 2026-05-01
venue: 'The 43th International Conference on Machine Learning'
# paperurl: 'https://arxiv.org/pdf/2604.17715'
# citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

Authors
======
K. Tran, Y. Boshmaf, I. Khalil, N.H. Phan, T. Yu, M. Parvez,

------

Abstract
======

Code Large Language Models (CLLMs) serve as the core of modern code agents, enabling developers to automate complex software development tasks. In this paper, we present Poison-with-Style (PwS), a practical and stealthy model poisoning attack targeting CLLMs. Unlike prior attacks that assume an active adversary capable of directly embedding explicit triggers (e.g., specific words) into developers' prompts during inference, PwS leverages developers' code styles as covert triggers implicitly embedded within their prompts. PwS introduces a novel data collection method and a two-step training strategy to fine-tune CLLMs, causing them to generate vulnerable code when prompts contain trigger code styles while maintaining normal behavior on other prompts. Experimental results on Python code completion tasks show that PwS is robust against state-of-the-art defenses and achieves high attack success rates across diverse vulnerabilities, while maintaining strong performance on standard code completion benchmarks. For example, in code completion tasks that are vulnerable to improper input validation (i.e., CWE-20), the poisoned model generates insecure code up to 95% of the cases when the trigger code style is used, with less than 5% drop in pass@1 performance on the HumanEval and MBPP benchmarks. 
