---
layout: default
title:  "Temperature in LLMs"
description: "What does temperature mean in LLMs."
categories: decoding basic
tags: transformer autoregressive-model decoding
excerpt_separator: <!--more-->
---

TL; DR;

Temperature is a parameter to control the randomness of LLM's output during decoding process.

---

Summary

1. (T<1) Lower temperature means more deterministic, the model tends to choose tokens with higher probabilities.
2. When the temperature is set 0, the model is completely deterministic. It always selects the token with the highest probability.