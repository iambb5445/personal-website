---
name: Language-Driven Play
tools: [Python, LLM, General Game-playing, Rule Understanding]
image: ../images/LLM-as-GGP.png
description: General game-playing, where a model can play different games given the rules and without specialized training is a challenging tasks. This project studies whether Large Language Models can act as general game-playing agents, tested on a simplified implementation of Slay the Spire.
external_url: 
---

# Large-Driven Play

Evaluating procedurally generated game rules is difficult, since the impact of a rule change on balance and complexity isn't always obvious from the rule itself. One way to evaluate such content is to simulate play, which requires an agent that can both play the game and adapt to changes in its design, commonly known as a general game-playing agent.

![preview](../images/LLM-as-GGP.png)

This project explores whether Large Language Models can serve as general game-playing agents, without any game-specific training. The testbed is a simplified implementation of the card game Slay the Spire, chosen for the rich, interacting rules its cards create. The results suggest that while an LLM agent doesn't always choose the locally optimal move, it shows a notable capacity for long-term planning, all without specialized training for the task.

This work was presented in the paper "Language-Driven Play: Large Language Models as Game-Playing Agents in Slay the Spire" by Bahar Bateni and Jim Whitehead, published at FDG 2024.

<p class="text-center">
{% include elements/button.html link="https://github.com/iambb5445/MiniSTS" text="Code" %}
{% include elements/button.html link="https://dl.acm.org/doi/abs/10.1145/3649921.3650013" text="Paper" %}
</p>