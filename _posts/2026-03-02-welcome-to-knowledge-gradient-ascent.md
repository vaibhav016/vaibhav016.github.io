---
layout: post
title: "Welcome to Knowledge Gradient Ascent"
date: 2026-03-02
tags: [meta, welcome]
---

Welcome to **Knowledge Gradient Ascent** — a blog where I document ideas, research insights, and things I learn along the way.

The name is a play on gradient ascent (maximizing an objective) applied to knowledge itself. As a PhD student working on continual learning and efficient inference, I find that writing helps crystallize understanding more than anything else.

## What to expect

I plan to write about:

- **Research notes** — breakdowns of papers I'm reading or ideas I'm exploring
- **Technical deep dives** — implementation details, debugging stories, and things that took too long to figure out
- **Reflections** — broader thoughts on the research process, PhD life, and the journey

Here's a quick example of what a code snippet looks like on this blog:

```python
import torch

# A simple gradient ascent step
def gradient_ascent_step(params, loss_fn, lr=0.01):
    loss = loss_fn(params)
    loss.backward()
    with torch.no_grad():
        params += lr * params.grad
        params.grad.zero_()
    return params
```

Stay tuned for more posts. If you have questions or want to chat, feel free to reach out at [vaibhav.singh@mila.quebec](mailto:vaibhav.singh@mila.quebec).
