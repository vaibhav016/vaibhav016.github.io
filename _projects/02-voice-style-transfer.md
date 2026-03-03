---
title: Voice Style Transfer
period: Jan 2021
order: 2
description: >-
  Extracting the timbre of one voice and superimposing it on another, inspired by image style transfer.
  Uses two convolutional encoders — a deep encoder for content (phonemes) and a shallow encoder for style
  (timbre) — to minimize content loss against the original input and style loss against the target voice.
tech:
  - Deep Learning
  - Audio Processing
  - Style Transfer
---

This idea is borrowed from computer vision's image style transfer. The fundamental concept is that our speech can be categorised into 2 sets of features — Content level (the actual phoneme or simply the content that one speaks) and Style level (the timbre or the texture of the speaker voice).

If we employ two convolutional encoder models, one being a deep encoder for the content and the other being a shallow encoder for style, then the output of our model should have minimum content loss with respect to the original input and minimum style loss with respect to the other person's style (which we want our output to sound like).
