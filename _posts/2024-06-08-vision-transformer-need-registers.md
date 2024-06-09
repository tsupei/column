---
layout: default
title:  "Vision Transformer Need Registers."
description: ""
categories: paper
tags: ICLR2024 transformer vision-encoder CLIP
excerpt_separator: <!--more-->
---

TL; DR;

Adding several register tokens makes the attention maps in vision encoder smoother and more interpretable.

---

Summary

1. Attention maps in CLIP-ViT and DINO-v2 have peak values (outliers)
2. This works hypothesizes these outliers store global information and discard local positional information
3. Instead of re-cycling the tokens (probably the model learns to do so itself), this work explictly adds register tokens as a place to cache the global information
4. It results in smoother and more interpretable attention maps
5. Smooth attention maps enable better accuracy in unsupervised segmentation

---

References

[Vision Transformer Need Registers](https://arxiv.org/pdf/2309.16588)