---
layout: page
title: AAAI Tutorial on Machine Learning for Solvers
---
<!-- <div class="venue" style="font-size: 27px; display: block; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 300; color: #404040; text-align: center;">
  <a target="_blank" href="https://neurips.cc/virtual/2023/tutorial/73946"><strong>Video Recording</strong></a>
</div> -->



<!-- <div class="sharethis-inline-share-buttons"></div>
<meta name="thumbnail" content="./img/neurips-logo-new.jpg" /> -->


# Overview

Machine learning (ML) and logical reasoning have been the two foundational pillars of AI since its inception, yet it is only in the past decade that interactions between these fields have become increasingly prominent. Notably, ML has had a dramatic impact on SAT and SMT solvers, as demonstrated by the award-winning SATzilla, MapleSAT, and Z3alpha solvers. Our tutorial aims to inspire new interdisciplinary research by bridging the gap between ML and logical reasoning research communities. We will introduce the broader AI community to ML techniques that have been used in the context of logical reasoning, with a sharp focus on approaches that are successful and promising. The main topics we will discuss are algorithm selection, algorithm configuration, deep learning for representing logical reasoning, and reinforcement learning for branching heuristics.

Rather than pure end-to-end learning, successful ML approaches tend to be tightly integrated with symbolic solvers. The central thesis of our tutorial, supported by numerous successful cases, is that ML excels best when it is used to sequence, select, initialize, and configure proof/rewrite rules that solvers implement. One prominent example of this trend is the use of ML for learning branching heuristics, both online for particular instances using reinforcement learning (RL) and offline training a neural network policy over a distribution of instances. We will discuss a paradigmatic distinction between online and offline ML in solvers. In the former, learning occurs during the solving process of a particular instance, whereas in the latter, algorithmic design is learned offline across representative instances from a particular application. Both paradigms can be powerful in improving solver performance. 

Our tutorial assumes only a basic understanding of ML from the audience. We begin with essential backgrounds on logical solvers, followed by a classification of ML application paradigms for solvers, and then present successful applications in each paradigm. Additionally, we delve into the recent advancements in the end-to-end learning paradigm using graph neural networks (GNNs) to model logical formulae. The tutorial includes hands-on coding demonstrations of applying SMAC to fine-tune online learning parameters in MapleSAT, enabling participants to directly engage with the concepts discussed. We conclude with a panel discussion on how to leverage large language models (LLMs) for logical reasoning and how reasoning can make LLMs more trustworthy.

<hr>


<!-- # Presenters
<div class="container" style="margin-top: 25px;margin-bottom: 40px;">
  <div class="row">
    {% for p in site.data.presenters %}
    {% if forloop.index<=4 %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
  <div class="row">
    {% for p in site.data.presenters %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% if forloop.index>4 and forloop.index<=7%}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
</div>
<hr>

# Panelists
<div class="container" style="margin-top: 20px;margin-bottom: 0px;">
  <div class="row">
    {% for p in site.data.panelists %}
    {% if forloop.index<=5 %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
  <div class="row">
    {% for p in site.data.panelists %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% if forloop.index>5 and forloop.index<=10%}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
  <div class="row">
    {% for p in site.data.panelists %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% if forloop.index>10%}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
</div>
<hr>


# Materials and Open-Source Tools

* **[Video Recording](https://neurips.cc/virtual/2023/tutorial/73946)**
* [Slides](./img/NeurIPS2023-Tutorial-ML4TP.pdf)
* [Demo: Using LLMs in Lean](https://github.com/yangky11/lean4-example/tree/ml4tp-tutorial)
* [Demo: Training LLMs for Tactic Generation and Combining with Proof Search](https://github.com/yangky11/ml4tp-tutorial/blob/main/main.ipynb)
* [A Survey on Deep Learning for Theorem Proving](https://arxiv.org/abs/2404.09939)

## Lean 

* [LeanDojo](https://github.com/lean-dojo/LeanDojo): Extracting data and interacting with Lean
* [ReProver](https://github.com/lean-dojo/ReProver): Training and evaluating language models for theorem proving
* [LLMStep](https://github.com/wellecks/llmstep): Using language models to suggest proof steps
* [Lean Copilot](https://github.com/lean-dojo/LeanCopilot): Using language models to suggest proof steps, search for proofs, and select premises

## Isabelle

* [PISA](https://github.com/albertqjiang/Portal-to-ISAbelle): Extracting data and interacting with Isabelle
* [Draft, Sketch, and Prove](https://github.com/albertqjiang/draft_sketch_prove): Implementation of "Draft, Sketch, and Prove: Guiding Formal Theorem Provers with Informal Proofs"


## Coq

* [CoqGym](https://github.com/princeton-vl/CoqGym): Extracting data and interacting with Coq
* [Tactician](https://coq-tactician.github.io/): KNNs and random forests + online learning for synthesizing proofs
* [Proverbot9001](https://github.com/UCSD-PL/proverbot9001): RNNs for synthesizing proofs
* [coq-synthesis](https://github.com/agrarpan/coq-synthesis): Coq plugin for using Proverbot9001 in the proof assistant
* [CoqPyt](https://github.com/sr-lab/coqpyt): Interacting with Coq

## Others

* [HOList](https://sites.google.com/view/holist/home): Extracting data and interacting with HOL Light
* [INT](https://github.com/albertqjiang/INT): Synthetic theorem proving benchmark on inequalities


# Citation

<p>If you find this tutorial useful, please cite:</p>
<div class="container" style="margin-top: 20px;margin-bottom: 0px;">
{% raw %}
<pre><code>@misc{ml4tptutorial2023,
  author = {First, Emily and Jiang, Albert and Yang, Kaiyu},
  title = {{NeurIPS} Tutorial on Machine Learning for Theorem Proving},
  year = {2023},
  howpublished = {\url{https://machine-learning-for-theorem-proving.github.io}},
}</code></pre>
{% endraw %}
</div>
<hr>

Contact: <machine.learning.4.theorem.proving@gmail.com>. -->
