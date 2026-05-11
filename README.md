# Rubrics Survey

This is a collection of papers related to **rubrics for large language models**. These papers are organized according to our survey paper:

**Rubrics for Large Language Models: Generation, Optimization, Evaluation, and Challenges**

Rubrics provide explicit, interpretable, and multi-dimensional evaluation criteria for assessing and improving large language models. This repository aims to maintain an up-to-date paper list for researchers interested in rubric construction, rubric-based policy model training, rubric-aware reward model training, and rubric-driven evaluation.

Feel free to contact us if you find a mistake, missing paper, or have any suggestions.

## 🌟 Citation

Please kindly cite our paper if this repository helps your research:

```bibtex
@article{RubricsSurvey,
  title={Rubrics for Large Language Models: Generation, Optimization, Evaluation, and Challenges},
  author={},
  journal={arXiv preprint},
  year={2026}
}
```

## 🚀 Update Log

- Version 1 \[2026-XX-XX\]
  - We release the first version of this repository.

## 📋 Table of Content

- [Rubrics Construction](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-construction)
  - [Direct Generation](https://github.com/8421BCD/Rubrics_Survey/tree/main#direct-generation)
  - [Contrastive Generation](https://github.com/8421BCD/Rubrics_Survey/tree/main#contrastive-generation)
  - [Iterative Refinement and Structural Induction](https://github.com/8421BCD/Rubrics_Survey/tree/main#iterative-refinement-and-structural-induction)
    - [Verification-Driven Refinement](https://github.com/8421BCD/Rubrics_Survey/tree/main#verification-driven-refinement)
    - [Structural Decomposition](https://github.com/8421BCD/Rubrics_Survey/tree/main#structural-decomposition)
    - [De-duplication and Compression](https://github.com/8421BCD/Rubrics_Survey/tree/main#de-duplication-and-compression)
  - [Online and Co-evolving Generation](https://github.com/8421BCD/Rubrics_Survey/tree/main#online-and-co-evolving-generation)
    - [Rollout-Based Evolving Rubrics](https://github.com/8421BCD/Rubrics_Survey/tree/main#rollout-based-evolving-rubrics)
    - [Online and Alternating Optimization of Rubric Generators](https://github.com/8421BCD/Rubrics_Survey/tree/main#online-and-alternating-optimization-of-rubric-generators)
    - [Self-Evolving, Adversarial, and Memory-Driven Rubrics](https://github.com/8421BCD/Rubrics_Survey/tree/main#self-evolving-adversarial-and-memory-driven-rubrics)
  - [Evaluation for Rubrics](https://github.com/8421BCD/Rubrics_Survey/tree/main#evaluation-for-rubrics)

- [Rubrics for Model Training](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-model-training)
  - [Rubrics for Policy Model Training](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-policy-model-training)
    - [Standard Rubric-based RL](https://github.com/8421BCD/Rubrics_Survey/tree/main#standard-rubric-based-rl)
    - [Advanced Reward Design](https://github.com/8421BCD/Rubrics_Survey/tree/main#advanced-reward-design)
    - [Rubrics as Policy Guidance](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-as-policy-guidance)
  - [Rubrics for Reward Model Training](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-reward-model-training)
    - [Rubrics for Interpretability](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-interpretability)
    - [Rubric-grounded Reasoning](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubric-grounded-reasoning)
    - [Rubric-Dimension Scoring](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubric-dimension-scoring)
    - [Rubrics for Reward Signals](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-reward-signals)
    - [Rubrics for Data Construction](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-data-construction)

- [Rubrics for Evaluation](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-evaluation)
  - [Rubrics for General Task Evaluation](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-general-task-evaluation)
    - [Reasoning Capability Evaluation](https://github.com/8421BCD/Rubrics_Survey/tree/main#reasoning-capability-evaluation)
    - [Deep Research and Open-Ended Generation Evaluation](https://github.com/8421BCD/Rubrics_Survey/tree/main#deep-research-and-open-ended-generation-evaluation)
    - [General Agent Capability Evaluation](https://github.com/8421BCD/Rubrics_Survey/tree/main#general-agent-capability-evaluation)
    - [Alignment Evaluation](https://github.com/8421BCD/Rubrics_Survey/tree/main#alignment-evaluation)
  - [Rubrics for Specific Task Evaluation](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-specific-task-evaluation)
    - [Rubrics for Intermediate Trajectories](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-intermediate-trajectories)
    - [Rubrics for Final Outputs](https://github.com/8421BCD/Rubrics_Survey/tree/main#rubrics-for-final-outputs)
      - [Content Quality and Factuality](https://github.com/8421BCD/Rubrics_Survey/tree/main#content-quality-and-factuality)
      - [Safety and Risk Auditing](https://github.com/8421BCD/Rubrics_Survey/tree/main#safety-and-risk-auditing)
      - [Professional Presentation and Structural Coherence](https://github.com/8421BCD/Rubrics_Survey/tree/main#professional-presentation-and-structural-coherence)
      - [Practical Utility and Actionability](https://github.com/8421BCD/Rubrics_Survey/tree/main#practical-utility-and-actionability)
- [Other Resources](https://github.com/8421BCD/Rubrics_Survey/tree/main#other-resources)
  - [Datasets](https://github.com/8421BCD/Rubrics_Survey/tree/main#datasets)
  - [Benchmarks](https://github.com/8421BCD/Rubrics_Survey/tree/main#benchmarks)
  - [Toolkits](https://github.com/8421BCD/Rubrics_Survey/tree/main#toolkits)
  - [Blog Posts and Tutorials](https://github.com/8421BCD/Rubrics_Survey/tree/main#blog-posts-and-tutorials)
- [Contributing](https://github.com/8421BCD/Rubrics_Survey/tree/main#contributing)
- [Contact](https://github.com/8421BCD/Rubrics_Survey/tree/main#contact)
  
## 📄 Paper List

## Rubrics Construction

This section collects papers that study how rubrics, criteria, checklists, nuggets, anchors, or evaluation dimensions are generated, refined, compressed, verified, or dynamically updated.

### Direct Generation

Direct generation methods construct rubrics directly from the query, instruction, answer, or evidence, usually through LLM prompting.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Contrastive Generation

Contrastive generation methods construct rubrics from preference pairs, positive/negative responses, or comparative signals, aiming to identify discriminative evaluation dimensions.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Iterative Refinement and Structural Induction

This category includes methods that refine, verify, decompose, filter, compress, or structurally optimize generated rubrics.

#### Verification-Driven Refinement

These methods evaluate candidate rubrics by checking whether they can reliably distinguish high-quality and low-quality responses.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

#### Structural Decomposition

These methods decompose coarse rubrics into fine-grained, atomic, verifiable, or hierarchical criteria.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

#### De-duplication and Compression

These methods reduce redundancy, compress instance-level rubrics into reusable structures, or improve separability between rubric dimensions.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Online and Co-evolving Generation

Online and co-evolving methods allow rubrics to adapt with model behavior, policy rollouts, judge feedback, or newly discovered failure modes.

#### Rollout-Based Evolving Rubrics

These methods update rubrics based on policy rollouts, trajectories, or model-generated outputs during training.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

#### Online and Alternating Optimization of Rubric Generators

These methods treat rubric generation or selection as a learnable component, often jointly or alternately optimized with the policy, judge, or reward model.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

#### Self-Evolving, Adversarial, and Memory-Driven Rubrics

These methods use adversarial probing, memory mechanisms, self-evolving procedures, or failure-mode discovery to continuously improve rubrics.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Evaluation for Rubrics

This subsection collects works that evaluate the quality, reliability, validity, alignment, or downstream utility of generated rubrics.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

## Rubrics for Model Training

This section collects papers that use rubrics to train LLMs, including policy model training and reward model training.

## Rubrics for Policy Model Training

Rubrics can be transformed into rewards, constraints, guidance signals, or structured supervision for policy optimization.

### Standard Rubric-based RL

These works use rubrics to evaluate model outputs or trajectories and aggregate rubric scores into scalar rewards for reinforcement learning or preference optimization.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Advanced Reward Design

These works improve the design of rubric-based rewards, including learned weighting, veto mechanisms, saturation-aware aggregation, curriculum over rubrics, token-level credit assignment, and algorithm-aware reward design.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Rubrics as Policy Guidance

These works use rubrics not only as post-hoc reward signals, but also as explicit guidance for generation, exploration, refinement, or hindsight learning during policy optimization.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

## Rubrics for Reward Model Training

Rubrics can also be used to train reward models by improving interpretability, providing dense supervision, or constructing better training data.

### Rubrics for Interpretability

These works incorporate rubrics into reward models to make preference judgments more explainable and controllable.

#### Rubric-grounded Reasoning

These methods require reward models to generate rubric-grounded reasoning before producing final preference judgments or scalar scores.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

#### Rubric-Dimension Scoring

These methods train reward models to output separate scores for different rubric dimensions and aggregate them into a final reward.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Rubrics for Reward Signals

These works use rubric-level signals, atomic reasoning units, generated criteria, or rubric alignment objectives as additional reward signals during reward model training.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Rubrics for Data Construction

These works use rubrics to construct, filter, augment, or intervene on preference data, with the goal of improving robustness and reducing shortcut learning in reward models.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

## Rubrics for Evaluation

This section collects papers and benchmarks that use rubrics as explicit evaluation interfaces for LLM outputs, agent trajectories, professional tasks, safety auditing, and domain-specific applications.

## Rubrics for General Task Evaluation

General-task evaluation focuses on broad capabilities that are transferable across domains, such as reasoning, instruction following, alignment, agent capability, and open-ended generation quality.

### Reasoning Capability Evaluation

These works use rubrics to evaluate reasoning processes, intermediate steps, logical validity, mathematical reasoning, code reasoning, or professional reasoning.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Deep Research and Open-Ended Generation Evaluation

These works use rubrics to assess long-form generation, deep research reports, evidence synthesis, citation grounding, information coverage, analytical depth, and report organization.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### General Agent Capability Evaluation

These works use rubrics to evaluate agent capabilities such as planning, memory, tool use, grounding, interaction reliability, trajectory quality, and multi-step task execution.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Alignment Evaluation

These works use rubrics to evaluate alignment-related capabilities, including helpfulness, honesty, harmlessness, instruction following, safety compliance, refusal quality, and judge reliability.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

## Rubrics for Specific Task Evaluation

Specific-task evaluation focuses on concrete downstream applications with domain-specific requirements, professional standards, environmental feedback, or high-stakes constraints.

### Rubrics for Intermediate Trajectories

These works evaluate intermediate reasoning trajectories, tool-use processes, execution steps, sub-goal completion, or process-level failures in specific downstream tasks.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Rubrics for Final Outputs

These works evaluate the final artifacts delivered to users, including answers, reports, slides, code, plans, professional advice, multimodal outputs, or spoken responses.

#### Content Quality and Factuality

These works use rubrics to assess factual correctness, information coverage, citation grounding, context faithfulness, evidence support, and hallucination control.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

#### Safety and Risk Auditing

These works use rubrics to assess harmfulness, unsafe advice, regulatory risks, medical risks, legal risks, policy violations, and high-stakes safety failures.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

#### Professional Presentation and Structural Coherence

These works use rubrics to assess organization, readability, formatting, professional tone, stylistic naturalness, visual layout, multimodal presentation, or speech delivery.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

#### Practical Utility and Actionability

These works use rubrics to assess whether the output is useful, actionable, goal-completing, practically executable, user-satisfying, or aligned with real-world constraints.

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
3. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

## Open Questions and Future Directions

This section summarizes open research questions in rubric-based LLM research. These directions correspond to the discussion section of our survey.

## Open Questions in Rubrics Construction

### Granularity and Scope of Rubric Design

How should rubrics balance coarse high-level dimensions and fine-grained atomic criteria? How broad or specific should a rubric be for different tasks, domains, and evaluation settings?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Coupling among Rubric Criteria

How should we model dependencies, redundancy, conflict, or interaction between different rubric criteria? How can we avoid double-counting or inconsistent scoring across correlated dimensions?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Generalization and Consistency of Rubrics

How can rubrics generalize across tasks, domains, user groups, and model families while maintaining consistent evaluation standards?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Personalized Rubrics

How can rubrics represent individual user preferences while remaining reliable, interpretable, and safe? How can personalized rubrics be constructed from sparse, noisy, or evolving user history?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Safety of Rubrics

How can we ensure that rubrics themselves are safe, robust, and resistant to malicious manipulation? How can we detect unsafe rubric edits or hidden preference drift?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

## Open Questions in Rubrics for Policy Model Training

### Rubric Reward Hacking in Reinforcement Learning

How can we prevent policies from exploiting superficial rubric wording rather than genuinely improving output quality? How can rubrics evolve with policy behavior to reduce reward hacking?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Train-Test Mismatch in Rubric-Based Optimization

How can we reduce the gap between training-time rubrics and test-time evaluation criteria? How can we prevent policies from overfitting to a particular judge model or rubric style?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

## Open Questions in Rubrics for Reward Model Training

### Annotation Cost of Fine-Grained Rubrics

How can we reduce the annotation cost of fine-grained rubric supervision while preserving quality, consistency, and interpretability?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Cross-Domain and Cross-Task Generalization

How can rubric-aware reward models generalize to new tasks, domains, output formats, or evaluation standards with limited additional supervision?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Interpretability-Efficiency Trade-off

How can we balance the interpretability of rubric-based reward modeling with the computational cost of multi-criteria scoring, reasoning generation, and aggregation?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

## Open Questions in Rubrics for Evaluation

### Bias in Rubric-Based Evaluation

How can we identify and reduce biases introduced by rubric phrasing, criterion ordering, score option ordering, judge model selection, or self-preference of LLM judges?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Dynamic Rubrics for Non-Standard Agent Trajectories

How can rubrics evaluate valid but unconventional agent trajectories that deviate from standard human-designed checkpoints? How can rubrics adapt to newly discovered behaviors?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

### Multi-Perspective Rubrics under Expert Disagreement

How can rubrics represent multiple valid expert perspectives, especially in domains where no single ground-truth standard exists?

1. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]
2. **Paper Title**, _Author et al._, Venue Year. \[[Paper]()\] \[[Code]()\] \[[Project]()\]

## Other Resources

This section collects related datasets, benchmarks, toolkits, leaderboards, blog posts, and tutorials.

### Datasets

1. **Dataset Name**. \[[Website]()\] \[[Paper]()\] \[[Data]()\]
2. **Dataset Name**. \[[Website]()\] \[[Paper]()\] \[[Data]()\]

### Benchmarks

1. **Benchmark Name**. \[[Website]()\] \[[Paper]()\] \[[Leaderboard]()\]
2. **Benchmark Name**. \[[Website]()\] \[[Paper]()\] \[[Leaderboard]()\]

### Toolkits

1. **Toolkit Name**. \[[GitHub]()\] \[[Paper]()\] \[[Documentation]()\]
2. **Toolkit Name**. \[[GitHub]()\] \[[Paper]()\] \[[Documentation]()\]

### Blog Posts and Tutorials

1. **Title**. \[[Link]()\]
2. **Title**. \[[Link]()\]

## Contributing

We welcome contributions to this repository.

You can contribute by:

- Adding missing papers.
- Fixing incorrect metadata.
- Updating paper links, code links, or project links.
- Suggesting better taxonomy or section organization.
- Opening issues for discussion.

Suggested paper entry format:

```markdown
1. **Paper Title**, _Author et al._, Venue Year. \[[Paper](paper_url)\] \[[Code](code_url)\] \[[Project](project_url)\]
```

If a paper has no code or project page, you can omit the corresponding link:

```markdown
1. **Paper Title**, _Author et al._, Venue Year. \[[Paper](paper_url)\]
```

## Contact

For questions or suggestions, please contact:

- Name:
- Email:
- GitHub Issue:
