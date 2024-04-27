# Promisingness-of-Automating-Alignment.github.io
Public repository for the Promisingness of Automating Alignment project
  

  
## Team Members
```
Mentor: Bogdan Ionut Cirstea \
AI Safety Camp: Jaeson Booker, Leo Mckee-Reid, Marcel Mir, Severin Field, Milton Lin, Sai Joseph, Vassil Tashev, Yuan Yuan Sun; \
MARS: Alfie Lamerton, Tim Chan, Robayet Hossain; \
SPAR: Joyee Chen, Joe Emerson, Minh Nguyen, Yixiong Hao.
```

## Background
Automating alignment research is one approach to alignment that has gained much more visibility with the [Open AI superalignment plan announcement](https://openai.com/blog/introducing-superalignment). Some of automating alignment’s selling points (if successful) include potentially resulting in an enormous amount of alignment research even in short calendar time and the apparent relative ease of (even if non-robustly) aligning systems similar to the current state-of-the-art (e.g. large language models, foundation models; see [this presentation](https://docs.google.com/presentation/d/1EKDdC-r8zvHrtXKWPQqqzbUfwjj1P9a_j9paKGMmdNY/edit?usp=sharing) by Bogdan for many more details), which could be used as automated alignment researchers/research assistants. Notably, if successful, automating alignment research could plausibly be the most scalable alignment research agenda (and probably by a wide margin). At the same time, strategies to automate alignment research like the superalignment plan have received a lot of criticism within the alignment community (see e.g. [this post](https://www.lesswrong.com/posts/NSZhadmoYdjRKNq6X/openai-launches-superalignment-taskforce)).

## Goal: 
This project aims to get more grounding into how promising automating alignment research is as a strategy, with respect to both advantages and potential pitfalls, with the superalignment plan as a potential blueprint/example (though ideally the findings would apply more broadly). This will be achieved by reviewing, distilling and integrating relevant research from multiple areas/domains, with a particular focus on the science of deep learning and on empirical findings in deep learning and language modelling. Team members work independently on reviewing and distilling different research topics (AI governance, interdisciplinary areas such as neuroscience and alignment, relevant prediction markets, and technical research relevant to the agenda) and then meet weekly to discuss and summarize ideas.


## Some Brainstorming questions
> How safe can ~human-level automated alignment researchers be made? Can we get ~human-level automated alignment researchers which are [relatively] safe to use (e.g. <0.1% extinction risk)?

> How much time between ~human-level automated alignment researchers (e.g. inside OpenAI) and significant AI x-risk from the wider world by default? Strategically relevant w.r.t. How much risk can/should be taken by running the automated alignment researchers.

> What will the first system which can significantly contribute to [automated] alignment research look like? How would this affect their safety / alignment properties?

> How much prosaic alignment progress ‘by default’ (e.g. for non-xrisk purposes, just through usual commercial/academic incentives) should we expect? How useful will this be for aligning automated alignment researchers?

> What order will powerful (~human-level) AI capabilities develop and how will this affect x-risk? E.g. GPT-2030 post argues for math and coding capabilities before robotics -> suggest e.g. update that some takeover scenarios requiring robotic capabilities less likely at first. Or e.g. if early AGIs are very computationally expensive  in terms of inference, there might not be enough compute for very large numbers of them to be deployed (making takeover more difficult). Or e.g. there might not be enough automation in the relevant supply chains for the first AGIs to be self-sustaining, hampering takeover through human extinction.

> How much will AI policy (e.g. US executive order covering evals for deployment, protective measures vs. cyber, bio, e.g. the EU AI act vs. [subliminally] manipulating people) delay x-risk from less cautious / malicious actors? (potentially allowing for more time to automate alignment research and produce a lot of research and/or to go more cautiously about this)

> Which approaches can/should be added to the portfolio of what could be used to align/make safe the automated alignment researcher (e.g. Redwood’s recent work, Seth Herd’s, stuff from my slides, other [meta] approaches from reading suggestions here)? How much should we expect these to drive down x-risk from using the automated alignment researcher a lot? Can we make a confident case that e.g. the x-risk would be < 0.1% (including e.g. based on arguments around capabilities, e.g. that alignment RAs too weak to take over)?


## Weak to Strong Generalization
Researched by Severin Field and Vassil Tashev
* [A review of weak-to-strong generalization literature](https://www.lesswrong.com/posts/ELbGqXiLbRe6zSkTu/a-review-of-weak-to-strong-generalization-ai-safety-camp)

#### Summary:
OpenAI’s super alignment agenda is to create automated safety researchers. At the end of 2023, OpenAI published “weak to strong generalization” which attempted to answer how we can create a setting to study superhuman AI. Reframing the alignment problem this way makes progress tractable creates a setting to empirically study “super alignment” before experiments can be done on a superhuman AI. We review their findings, a number of similar papers, and the implications for automated safety R&D.


* [Paper review: “The Unreasonable Effectiveness of Easy Training Data for Hard Tasks”](https://www.lesswrong.com/posts/Wd9vzwqcYuEokJYCH/paper-review-the-unreasonable-effectiveness-of-easy-training)

#### Summary:
Scalable oversight seems easier based on experiments outlined in a recent paper; questions arise about the implications of these findings. 

## In-context Learning
Researched by Alfie Lamerton
* [A review of In-Context Learning Hypotheses for Automated AI](https://www.lesswrong.com/posts/GPcwP8pgyPFPwvi2h/a-review-of-in-context-learning-hypotheses-for-automated-ai)
  
#### Summary

## Sparse Autoencoders (SAEs)
Researched by Nguyen Nhat Minh
* [A Review of Automated Approaches for Sparse Autoencoders (SAEs) (Google Doc draft)](https://docs.google.com/document/d/1Y9F8j4h39C6LUC25XvjzAcZLu1RH5yuPJ9BL8DolVhM/edit)
  
#### Summary
This draft document provides an overview of recent progress in using Sparse Autoencoders (SAEs) for mechanistic interpretability of AI systems, with a focus on the promisingness of automating various parts of the SAE workflow. It discusses key areas of automation, including finding new features, increasing feature accuracy, the reconstruction-sparsity tradeoff, better metrics to quantify and evaluate features and approaches to identifying/classifying feature families.

While SAE researchers have made rapid, iterative progress in discovering new methods to find and evaluate features in models within the past year, the scalability of these methods to larger models remains uncertain,* and several SAE researchers have emphasised the inherent limitations of current benchmarks. Additionally, the pace of AI capabilities progress poses a challenge for mechanistic interpretability research to keep up with increasingly complex frontier models.

*We note Google Deepmind’s very promising recent paper, which successfully applies SAEs to 7B parameter model. Due to multiple highly significant SAE/mech interp research papers being published within the past week, this section is not up-to-date as of end April 2024.

## Theoretical Chain of Thought
Researched by Severin Field
* [lesswrong post coming soon]()\

#### Summary 
“One of the main limitations is that the architecture does not allow for an ‘inner monologue’ or scratchpad beyond it’s internal representation, that could enable it to perform multi-step computations or store intermediate results” - Sebastian Bubeck, 2023

Chain of thought not only improves the performance of LLM’s, but chain of thought improves the [expressivity of transformers](https://arxiv.org/abs/2310.07923); problems can be solved with chain of thought that could not be solved in a single forward pass. In principle, an autoregressive transformer is turing-complete. [Auto-Regressive next token predictors are universal learners](https://arxiv.org/abs/2309.06979) 

We investigate the literature with the following in mind: 
* What will the first meaningfully useful automated safety researcher look like?
* Does chain of thought help with learning? With new knowledge creation?
* What are the properties of data that allow for chain of thought to work?
* Is a large language model’s chain of thought faithful? How interpretable is chain of thought?

## Automated Alignment considerations from a Governance perspective
Researched by Marcel Mir

#### Summary
Could current trends in AI policies impact the automated alignment approach? 

Regulatory bodies and international organisations are starting to develop policy proposals and legislation to regulate the development, deployment and commercialisation of AI products. Legislation might be passed that imposes requirements to AI products in their development stage that clash with the industrial or large scale adoption of an AI alignment researcher to supervise the model.

The aim of this project is to bring up some questions and considerations regarding Automating the solution for the alignment problem from a Governance perspective and force.

The Governace literature used are the current AI regulatory trends, existing legislative projects and legislation from the US, China and EU. While the approach for Automated Alignment used is OpenAI’s SuperAlignment plan.

* Could AI Governance safety proposals interfere in with the implementation of an AI alignment researcher? 
* Does this approach clash with current AI governance principles such as human oversight?

The desired output of the project is a lesswrong or EA post raising and anticipating questions and considerations for automated alignment researchers and policymakers.

## A proposed compute-based method for predicting the future feasibility of the Linear Representation Hypothesis for automating alignment research
Researched by Vassil Tashev
* [LessWrong post coming soon]()\

#### Summary
This research seeks to determine whether the Linear Representation Hypothesis and Causal World Models will remain viable as algorithms and hardware advance and large language models scale up. Using the Direct Approach framework, the study examines the potential effect of expanding model capabilities on the robustness of theoretical assumptions and the probability of their sustained efficacy for activation engineering and automated alignment. The project aims to develop a methodology that will precisely evaluate how advancements in computational power influence existing knowledge representation theories and their relevance in the future. The analysis is based on the work of Park et al. (2023), Turner et al.(2023), Zou et al.(2023), Nanda et al. (2023), Barnett (2023), Burns et al. (2023), Manning et al. (2024), Rajendran et al. (2024), Richens et al. (2024), Jiang et al. (2024), Ho et a. (2024), Wang et al. (2024) and others.
