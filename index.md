---
layout: page
title: AAAI 2025 Tutorial <br />Machine Learning for Solvers
---
<!-- <div class="venue" style="font-size: 27px; display: block; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 300; color: #404040; text-align: center;">
  <a target="_blank" href="https://neurips.cc/virtual/2023/tutorial/73946"><strong>Video Recording</strong></a>
</div> -->

<div class="venue" style="font-size: 24px; display: block; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 300; color: #404040; text-align: center;">
  <strong>Room 118A, <a target="_blank" href="https://g.co/kgs/jLhwXps">Pennsylvania Convention Center</a>, Philadelphia</strong>
</div>

<div class="venue" style="font-size: 24px; display: block; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 300; color: #404040; text-align: center;">
  <strong>26 February 2025, 2–6 PM ET</strong>
</div>

<div class="venue" style="font-size: 20px; display: block; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 300; color: #404040; text-align: center;">
  <a target="_blank" href="https://aaai.org/conference/aaai/aaai-25/tutorial-and-lab-list/#TH24">(AAAI 2025 website)</a>
</div>

<div class="sharethis-inline-share-buttons"></div>
<meta name="thumbnail" content="https://ml-for-solvers.github.io/img/aaai-small.jpeg" />

<nav>
  <a href="#presenters">Presenters</a> |
  <a href="#panelists">Panelists</a> |
  <a href="#overview">Overview</a> |
  <a href="#schedule">Schedule</a> |
  <a href="#registration">Registration</a> |
  <a href="#papers-and-tools">Papers and Tools</a> |
</nav>

# Presenters
<div class="container" style="margin-top: 25px;margin-bottom: 40px;">
  <div class="row">
    {% for p in site.data.presenters %}
    {% if forloop.index<=5 %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
  <div class="row">
    {% for p in site.data.presenters %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% if forloop.index>5 and forloop.index<=10%}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
</div>
<hr>

# Panelists
<div class="container" style="margin-top: 25px;margin-bottom: 40px;">
  <div class="row">
    {% for p in site.data.panelists %}
    {% if forloop.index<=6 %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
  <div class="row">
    {% for p in site.data.panelists %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% if forloop.index>6 and forloop.index<=10%}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
</div>
<hr>

# Overview

Machine learning (ML) and logical reasoning have been the two foundational pillars of AI since its inception, yet it is only in the past decade that interactions between these fields have become increasingly prominent. Notably, ML has had a dramatic impact on SAT and SMT solvers, as demonstrated by the award-winning SATzilla, MapleSAT, and Z3alpha solvers. Our tutorial aims to inspire new interdisciplinary research by bridging the gap between ML and logical reasoning research communities. We will introduce the broader AI community to ML techniques that have been used in the context of logical reasoning solvers, with a sharp focus on approaches that are successful and promising. We will also host a panel discussion on how LLMs may shape this area going forward.

Rather than pure end-to-end learning, successful ML approaches tend to be tightly integrated with symbolic solvers. The central thesis of our tutorial, supported by numerous successful cases, is that ML excels best when it is used to sequence, select, initialize, and configure proof/rewrite rules that solvers implement. One prominent example that we will highlight is the use of ML for learning branching heuristics, both online for particular instances using reinforcement learning (RL) and offline training a neural network policy across representative instances from a particular application. 

Our tutorial assumes only a basic understanding of ML and begins with essential backgrounds on logical solvers. We explore the main ML-for-solving paradigms—algorithm selection, algorithm configuration, and reinforcement learning for heuristics—highlighting successful applications in each area. We also examine why graph neural networks (GNNs) are an appropriate architecture for modeling logical formulae with neural networks. We will conclude the tutorial section with a hands-on coding demonstration of how to configure a parameterized solver for a specific application, applying SMAC to fine-tune online learning parameters in MapleSAT. Participants are encouraged to bring their own solver and application to test whether this method could be effective for their own work. 

Finally, we will have a panel discussion with leading experts to discuss the implications of LLMs for logical reasoning, a topic where opinions tend to be very polarized in the AI community. The panel will examine how effective LLMs might be for reasoning tasks and, conversely, how integrating formal logical reasoning could enhance the trustworthiness of LLMs.

<hr>

# Schedule

<div class="container" style="margin-top: 15px; text-align: center;">
  <table style="width: 100%; max-width: 1050px; margin: auto; border-collapse: collapse; font-size: 17px; line-height: 1.5;">
    <tr style="font-weight: bold;">
      <th style="padding: 10px; text-align: left; width: 12%;">Time</th>
      <th style="padding: 10px; text-align: left; width: 58%;">Session</th>
      <th style="padding: 10px; text-align: left; width: 30%;">Presenters</th>
    </tr>
    <tr>
      <td style="padding: 10px;">14:00 - 14:45</td>
      <td style="padding: 10px;">Introduction, Background, and Online Reinforcement Learning for Solvers [<a href="https://docs.google.com/presentation/d/1muSL9TGqe45uZzI803IO3Bu4sNgOKCba/edit?usp=sharing&ouid=117676940067056675826&rtpof=true&sd=true">Slides</a>]</td>
      <td style="padding: 10px;">Vijay Ganesh</td>
    </tr>
    <tr>
      <td style="padding: 10px;">14:45 - 15:30</td>
      <td style="padding: 10px;">Algorithm Selection and Configuration, with Hands-on Demonstration [<a href="https://docs.google.com/presentation/d/1cvhm6J-viT0IZb4XRY3cym7FzPjHpfUB/edit?usp=sharing&ouid=117676940067056675826&rtpof=true&sd=true">Slides</a>, <a href="https://colab.research.google.com/drive/1hx8JAsGjtzllOWjZpULir8i_7qua-UOw?usp=sharing">Colab</a>]</td>
      <td style="padding: 10px;">John Lu, Piyush Jha</td>
    </tr>
    <tr>
      <td style="padding: 10px;">15:30 - 16:00</td>
      <td colspan="2" style="padding: 10px; font-style: italic; text-align: center;">Coffee Break</td>
    </tr>
    <tr>
      <td style="padding: 10px;">16:00 - 16:50</td>
      <td style="padding: 10px;">Deep Learning for Solvers [<a href="https://drive.google.com/file/d/1ubenUBDHQhoT1km5gF-bGKi7z8kQrDwy/view?usp=sharing">Slides</a>]</td>
      <td style="padding: 10px;">Chris Cameron</td>
    </tr>
    <tr>
      <td style="padding: 10px;">17:00 - 18:00</td>
      <td style="padding: 10px;">Panel Discussion: Bridging Learning and Reasoning via LLMs and Solvers (Panelists: Subbarao Kambhampati, Xujie Si, Stefan Szeider, Huan Zhang)</td>
      <td style="padding: 10px;">Moderators: Kevin Leyton-Brown, Vijay Ganesh</td>
    </tr>
  </table>
</div>

<hr>

# Registration

<div class="venue" style="display: block;">
  <a target="_blank" href="https://aaai.org/conference/aaai/aaai-25/registration/">Please use this link to register on the official AAAI website</a>
</div>
<hr>

# Papers and Tools

- [AlphaMapleSAT](https://arxiv.org/abs/2401.13770)  
  - Jha, P.; Li, Z.; Lu, Z.; Bright, C.; and Ganesh, V. 2024. AlphaMapleSAT: An MCTS-based Cube-and-Conquer SAT Solver for Hard Combinatorial Problems. *arXiv preprint arXiv:2401.13770*.

- [Btor2-Select](https://gitlab.com/sosy-lab/software/btor2-select)  
  - Lu, Z.; Chien, P.; Lee, N.; and Ganesh, V. 2025. Algorithm selection for word-level hardware model checking (student abstract). *AAAI 2025*.

- [Goose](https://goosesolver.github.io/)  
  - Scott, J.; Pan, G.; Khalil, E. B.; and Ganesh, V. 2022, August. Goose: A Meta-Solver for Deep Neural Network Verification. *In SMT*, 99–113.

- [MachSMT](https://machsmt.github.io/)  
  - Scott, J.; Niemetz, A.; Preiner, M.; Nejati, S.; and Ganesh, V. 2021, March. MachSMT: A machine learning-based algorithm selector for SMT solvers. *In International Conference on Tools and Algorithms for the Construction and Analysis of Systems*, 303–325. Cham: Springer International Publishing.

- [MCFS](https://github.com/ChrisCameron1/MCFS)  
  - Cameron, C.; Hartford, J.; Lundy, T.; Truong, T.; Milligan, A.; Chen, R.; and Leyton-Brown, K. 2024. UNSAT Solver Synthesis via Monte Carlo Forest Search. *In International Conference on the Integration of Constraint Programming, Artificial Intelligence, and Operations Research*, 170–189. Springer.

- [MapleSAT](https://maplesat.github.io/)  
  - Liang, J. H.; Ganesh, V.; Poupart, P.; and Czarnecki, K. 2016. Learning rate based branching heuristic for SAT solvers. *In Theory and Applications of Satisfiability Testing–SAT 2016: 19th International Conference*, Bordeaux, France, July 5-8, 2016, Proceedings 19, 123–140. Springer.

- [ParamILS](https://www.cs.ubc.ca/labs/algorithms/Projects/ParamILS/)  
  - Hutter, F.; Hoos, H. H.; Leyton-Brown, K.; and Stutzle, T. 2009. ParamILS: An Automatic Algorithm Configuration Framework. *JAIR*, 36: 267–306.

- [SATzilla](https://arxiv.org/abs/1111.2249)  
  - Xu, L.; Hutter, F.; Hoos, H. H.; and Leyton-Brown, K. 2008. SATzilla: portfolio-based algorithm selection for SAT. *Journal of Artificial Intelligence Research*, 32: 565–606.

- [SMAC](https://github.com/automl/SMAC3)  
  - Hutter, F.; Xu, L.; Hoos, H. H.; and Leyton-Brown, K. 2014. Algorithm runtime prediction: methods & evaluation. *Artificial Intelligence*, 206: 79–111.

- [Z3alpha](https://github.com/JohnLyu2/z3alpha)  
  - Lu, Z.; Siemer, S.; Jha, P.; Day, J.; Manea, F.; and Ganesh, V. 2024. Layered and Staged Monte Carlo Tree Search for SMT Strategy Synthesis. *In Larson, K., ed., Proceedings of the Thirty-Third International Joint Conference on Artificial Intelligence, IJCAI-24*, 1907–1915. International Joint Conferences on Artificial Intelligence Organization.


<!-- 
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
