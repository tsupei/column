---
layout: default
title:  "MoE (Mixture of Experts)"
description: "Mixture of Experts"
categories: transformer
tags: google transformer moe switch-transformer
excerpt_separator: <!--more-->
---

TL; DR; 

MoE is a method of routing each token to different experts so that the model can be more representative with faster inference speed.

---

Summary

1. `MoE Layers`: MoE Layers are used in transformers in replace of feedforward layers. An MoE layer is composed of a few experts, which can be either FFN or another MoE layers.
2. `Gate network`: Each token is routed to $k$ experts based on the gate network, for example, a softmax function.
3. `Expert capacity`: In practice, different experts may have unbalanced workload. Each expert is set capacity to avoid overfitting and unbalanced workloads.
4. `Auxiliary Loss`: An loss to avoid unbalanced workloads, for example,  $ \textit{KL}(G(x) \|\| U) $ the KL-divergence from the gate network to an uniform distribution.

---

Reference

[Switch Transformer](https://arxiv.org/pdf/2101.03961)