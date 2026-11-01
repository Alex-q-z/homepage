---
# Copy this file to start a new post. Name it YYYY-MM-DD-short-title.md.
# Delete the `published: false` line when you are ready to publish.
published: false
layout: post
title: Post title
date: 2026-11-01
description: One or two sentences shown in the blog list.
tags: [llm-agents, self-improvement]
categories: [research]
thumbnail: # optional, e.g. assets/img/my-figure.png
toc:
  sidebar: left
---

Write the post in Markdown. Math works inline, $$a^2 + b^2 = c^2$$, and as blocks.

## A section

Images go in `assets/img/` and can be added like this:

{% raw %}{% include figure.liquid loading="eager" path="assets/img/my-figure.png" class="img-fluid rounded z-depth-1" caption="A caption." %}{% endraw %}

Code blocks get syntax highlighting:

```python
def improve(agent, experience):
    return agent.update(context=experience)
```
