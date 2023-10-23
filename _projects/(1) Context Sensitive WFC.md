---
name: Context Sensitive WFC
tools: [Python, PCG, WFC, Tile-based Generation]
image: ../images/cswfc.png
description: WaveFunctionCollapse (WFC) is a procedural content generation algorithm. Context-sensitive WFC offers a small modification to the search heuristic, significantly improving the quality of results, resemblance to the input image, and expressive range.
external_url: 
---

# Context-sensitive WFC

WaveFunctionCollapse (WFC) is a Procedural Content Generation algorithm which generates an output similar to some input. The input is broken into tiles or patterns which can be composed by the algorithm to create a new structures. A set of constraints extracted from the input are satisfied during the process which results in the similarity between the input and output. Context-sensitive WFC proposes a small and easy to implement modification to the WaveFunctionCollapse algorithm which significantly improves the quality fo results.

![preview](../images/cswfc/gif_Context-sensitive.gif)

This modification was proposed in the paper "Better Resemblance without Bigger Patterns: Making Context-sensitive Decisions in WFC" by Bahar Bateni, Isaac Karth and Adam Smith, published at FDG 2023. The paper proposes this modification, and reports its impact on the "resemblance" between the input and output and the expressive range of the algorithm.

<p class="text-center">
{% include elements/button.html link="https://github.com/iambb5445/Context-sensitive-WFC" text="Code" %}
{% include elements/button.html link="https://dl.acm.org/doi/10.1145/3582437.3582441" text="Paper" %}
</p>