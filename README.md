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

### Direct Generation

### Contrastive Generation

### Iterative Refinement and Structural Induction

### Online and Co-evolving Generation

### Evaluation for Rubrics

## Rubrics for Model Training

### Rubrics for Policy Model Training

#### Standard Rubric-based RL

1. **Checklists are better than reward models for aligning language models**, _Viswanathan et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2507.18624)\]
2. **Training AI Co-Scientists Using Rubric Rewards**, _Goel et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2512.23707)\]
3. **Rubrics as Rewards: Reinforcement Learning Beyond Verifiable Domains**, _Gunjal et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2507.17746)\]
4. **Open Rubric System: Scaling Reinforcement Learning with Pairwise Adaptive Rubric**, _Jia et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.14069)\]
5. **Chasing the Tail: Effective Rubric-based Reward Modeling for Large Language Model Post-Training**, _Zhang et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2509.21500)\]
6. **RLAC: Reinforcement Learning with Adversarial Critic for Free-Form Generation Tasks**, _Wu et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2511.01758)\]
7. **Visual Preference Optimization with Rubric Rewards**, _Yu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2604.13029)\]
8. **AutoRubric-R1V: Rubric-Based Generative Rewards for Faithful Multimodal Reasoning**, _Jia et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.14738)\]
9. **Reinforcing Chain-of-Thought Reasoning with Self-Evolving Rubrics**, _Sheng et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.10885)\]
10. **Dr Tulu: Reinforcement Learning with Evolving Rubrics for Deep Research**, _Shao et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2511.19399)\]
11. **OralGPT-Plus: Learning to Use Visual Tools via Reinforcement Learning for Panoramic X-ray Analysis**, _Fan et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.06366)\]

#### Advanced Reward Design

1. **Rule Based Rewards for Language Model Safety**, _Mu et al._, NeurIPS 2024. \[[Paper](https://arxiv.org/abs/2411.01111)\]
2. **Reinforcement Learning with Rubric Anchors**, _Huang et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2508.12790)\]
3. **Mock Worlds, Real Skills: Building Small Agentic Language Models with Synthetic Tasks, Simulated Environments, and Rubric-Based Rewards**, _Lyu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.22511)\]
4. **StitchCUDA: An Automated Multi-Agents End-to-End GPU Programing Framework with Rubric-based Agentic Reinforcement Learning**, _Li et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.02637)\]
5. **RuCL: Stratified Rubric-Based Curriculum Learning for Multimodal Large Language Model Reasoning**, _Chen et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.21628)\]
6. **Alternating Reinforcement Learning with Contextual Rubric Rewards**, _Lan_, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.15646)\]
7. **Stabilizing Rubric Integration Training via Decoupled Advantage Normalization**, _Tan et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.26535)\]
8. **Rubrics to Tokens: Bridging Response-level Rubrics and Token-level Rewards in Instruction Following Tasks**, _Xu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2604.02795)\]

#### Rubrics as Policy Guidance

1. **Breaking the Exploration Bottleneck: Rubric-Scaffolded Reinforcement Learning for General LLM Reasoning**, _Zhou et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2508.16949)\]
2. **Experience is the Best Teacher: Motivating Effective Exploration in Reinforcement Learning for LLMs**, _Zhang et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.20046)\]

### Rubrics for Reward Model Training

#### Rubrics for Interpretability

#### Rubrics for Reward Signals

#### Rubrics for Data Construction

## Rubrics for Evaluation

### Rubrics for General Task Evaluation

#### Reasoning Capability Evaluation

#### Deep Research and Open-Ended Generation Evaluation

#### General Agent Capability Evaluation

#### Alignment Evaluation

### Rubrics for Specific Task Evaluation

#### Rubrics for Intermediate Trajectories

#### Rubrics for Final Outputs

#### Content Quality and Factuality

#### Safety and Risk Auditing

#### Professional Presentation and Structural Coherence

#### Practical Utility and Actionability


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

## 📞 Contact

For any questions or feedback, please reach out to us at [lwh@ruc.edu.cn](lwh@ruc.edu.cn).
