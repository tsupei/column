---
layout: default
title:  "Temperature."
description: ""
categories: decoding
tags: transformer autoregressive-model decoding
excerpt_separator: <!--more-->
---

TL; DR;

Temperature is a parameter to control the randomness of LLM's output during decoding process.

---

Summary

1. (T<1) Lower temperature means more deterministic, the model tends to choose tokens with higher probabilities.
2. When the temperature is set 0, the model is completely deterministic. It always selects the token with the highest probability.