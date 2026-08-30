---
name: Solitaire Rule Understanding
tools: [Python, LLM, Game Description Language, Rule Understanding]
image: ../images/klondike_gui.png
description: Fine-tuning improves how well LLMs understand game rules, including rules unlike anything seen in training. This project studies that generalization using a large set of generated Solitaire rulesets and rule-understanding datasets.
external_url: 
category: Rule Reasoning
subcategory: Solitaire
---

# Solitaire Rule Understanding

Large Language Models tend to perform poorly at understanding rules, whether applying them, interacting with them, generating or modifying them, or evaluating them. Fine-tuning on a specific ruleset helps, but it undermines one of the main advantages of a pre-trained model, its ability to generalize to rulesets it hasn't seen. This generalization is exactly what matters for using LLMs as a tool in game development, where they need to give feedback or suggest rule modifications on rulesets that don't resemble anything in their training data. This project asks whether fine-tuning on rule understanding can improve generalization to these unseen, out-of-distribution rulesets, rather than only improving performance on the rules it was trained on.

<img src="../images/board_scorpion.png" alt="preview" width="500"/>

To study this, we needed a large space of distinct, well-defined rulesets to fine-tune and test on, so we built a framework for generating and simulating Solitaire variants from a custom Game Description Language (SGDL). Solitaire variants have simple rules but span a large space of possibilities, each playing out completely differently, which makes them well suited for testing generalization. The framework generates game progression questions along with a textual explanation for each answer, which are used to build datasets for both training and evaluation.

Using these datasets, we fine-tune and evaluate multiple LLMs on rule understanding, including out-of-distribution evaluations where a model is tested on rulesets it was never trained on. The results show that fine-tuning improves performance not just on in-distribution rulesets, but on out-of-distribution ones as well, suggesting that training on rule-based datasets can improve an LLM's general capacity for rule understanding, rather than just memorizing a specific ruleset.

This work was presented in the paper "LLM Game Rule Understanding Through Out-of-Distribution Fine-Tuning" by Bahar Bateni, Benjamin Pratt, and Jim Whitehead, published at AIIDE 2025.

<p class="text-center">
{% include elements/button.html link="https://github.com/iambb5445/SolitaireGDL" text="Code" %}
{% include elements/button.html link="https://huggingface.co/datasets/bbateni/Solitaire-Rule-Reasoning-Benchmark" text="Dataset" %}
{% include elements/button.html link="https://ojs.aaai.org/index.php/AIIDE/article/view/36804" text="Paper" %}
{% include elements/button.html link="https://iambb5445.github.io/SolitaireGDLWeb/index.html" text="Play it Online" %}
</p>