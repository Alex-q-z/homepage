---
layout: page
permalink: /publications/
title: publications
description: "* denotes equal contribution. See also <a href='https://scholar.google.com/citations?user=xnt6d5oAAAAJ'>Google Scholar</a>."
nav: true
nav_order: 2
---

<!-- Papers live in _bibliography/papers.bib. The `topic` field decides the section below. -->

{% include bib_search.liquid %}

<div class="publications">

<h2 class="bibliography">Recursive Self-Improvement</h2>
<p>ACE and Meta-Harness are featured in Lilian Weng's <a href="https://lilianweng.github.io/posts/2026-07-04-harness/">blog</a> on harness engineering for self-improvement.</p>

{% bibliography --group_by none --query @*[topic=rsi]* %}

<h2 class="bibliography">KV Cache and LLM Inference Infrastructure</h2>
<p>CacheGen and CacheBlend led to the <a href="https://lmcache.ai/en/">LMCache</a> project and the <a href="https://www.tensormesh.ai/">Tensormesh</a> company.</p>

{% bibliography --group_by none --query @*[topic=kvcache]* %}

<h2 class="bibliography">Other Papers</h2>

{% bibliography --group_by none --query @*[topic=other]* %}

</div>
