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
  - [Background](https://github.com/8421BCD/Rubrics_Survey/tree/main#background)
  - [Direct Generation](https://github.com/8421BCD/Rubrics_Survey/tree/main#direct-generation)
  - [Contrastive Generation](https://github.com/8421BCD/Rubrics_Survey/tree/main#contrastive-generation)
  - [Iterative Refinement](https://github.com/8421BCD/Rubrics_Survey/tree/main#iterative-refinement)
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

### Background

1. **FLASK: Fine-grained Language Model Evaluation based on Alignment Skill Sets**, _Ye et al._, ICLR 2024. \[[Paper](https://arxiv.org/abs/2307.10928.pdf)\]
2. **Prometheus: Inducing Fine-grained Evaluation Capability in Language Models**, _Kim et al._, ICLR 2024. \[[Paper](https://arxiv.org/abs/2310.08491.pdf)\]
3. **Rule Based Rewards for Language Model Safety**, _Mu et al._, NeurIPS 2024. \[[Paper](https://arxiv.org/abs/2411.01111.pdf)\]
4. **Reinforcement Learning with Rubric Anchors**, _Huang et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2508.12790.pdf)\]

### Direct Generation

1. **Rubrics as Rewards: Reinforcement Learning Beyond Verifiable Domains**, _Gunjal et al._, ICLR 2026. \[[Paper](https://arxiv.org/abs/2507.17746.pdf)\]
2. **Checklists Are Better Than Reward Models For Aligning Language Models**, _Viswanathan et al._, NeurIPS 2025. \[[Paper](https://proceedings.neurips.cc/paper_files/paper/2025/file/a6837c1dd021f76f1b4098e3722052a8-Paper-Conference.pdf)\]
3. **CARMO: Dynamic Criteria Generation for Context Aware Reward Modelling**, _Gupta et al._, Findings of ACL 2025. \[[Paper](https://aclanthology.org/2025.findings-acl.114/)\]
4. **WildBench: Benchmarking LLMs with Challenging Tasks from Real Users in the Wild**, _Lin et al._, ICLR 2025. \[[Paper](https://arxiv.org/abs/2406.04770.pdf)\]
5. **SedarEval: Automated Evaluation using Self-Adaptive Rubrics**, _Fan et al._, Findings of EMNLP 2024. \[[Paper](https://aclanthology.org/2024.findings-emnlp.984/)\]
6. **WritingBench: A Comprehensive Benchmark for Generative Writing**, _Wu et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2503.05244.pdf)\]

### Contrastive Generation

1. **CDRRM: Contrast-Driven Rubric Generation for Reliable and Interpretable Reward Modeling**, _Liu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.08035.pdf)\]
2. **Chasing the Tail: Effective Rubric-based Reward Modeling for Large Language Model Post-Training**, _Zhang et al._, ICLR 2026. \[[Paper](https://arxiv.org/abs/2509.21500.pdf)\]
3. **OpenRubrics: Towards Scalable Synthetic Rubric Generation for Reward Modeling and LLM Alignment**, _Liu et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.07743.pdf)\]
4. **Rationale Matters: Learning Transferable Rubrics via Proxy-Guided Critique for VLM Reward Models**, _Qiu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.16600.pdf)\]
5. **Learning Query-Specific Rubrics from Human Preferences for DeepResearch Report Generation**, _Lv et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.03619.pdf)\]

### Iterative Refinement

#### Verification-Driven Refinement

1. **Auto-Rubric: Learning From Implicit Weights to Explicit Rubrics for Reward Modeling**, _Xie et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.17314.pdf)\]
2. **OptimSyn: Influence-Guided Rubrics Optimization for Synthetic Data Generation**, _Fan et al._, ICLR 2026. \[[Paper](https://arxiv.org/abs/2604.00536.pdf)\]

#### Structural Decomposition

1. **Rethinking Rubric Generation for Improving LLM Judge and Reward Modeling for Open-ended Tasks**, _Shen et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.05125.pdf)\]
2. **Qworld: Question-Specific Evaluation Criteria for LLMs**, _Gao et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.23522.pdf)\]
3. **An Efficient Rubric-based Generative Verifier for Search-Augmented LLMs**, _Ma et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.14660.pdf)\]
4. **RubricHub: A Comprehensive and Highly Discriminative Rubric Dataset via Automated Coarse-to-Fine Generation**, _Li et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.08430.pdf)\]
5. **Rubric Is All You Need: Improving LLM-Based Code Evaluation With Question-Specific Rubrics**, _Pathak et al._, ICER 2025. \[[Paper](https://doi.org/10.1145/3702652.3744220)\]
6. **DeepResearch Bench II: Diagnosing Deep Research Agents via Rubrics from Expert Report**, _Li et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.08536.pdf)\]
7. **RefGrader: Automated Grading of Mathematical Competition Proofs using Agentic Workflows**, _Mahdavi et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.09021.pdf)\]
8. **RubricRAG: Towards Interpretable and Reliable LLM Evaluation via Domain Knowledge Retrieval for Rubric Generation**, _Dhole et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.20882.pdf)\]
9. **InfiMed-ORBIT: Aligning LLMs on Open-Ended Complex Tasks via Rubric-Based Incremental Training**, _Wang et al._, ICML 2026. \[[Paper](https://arxiv.org/abs/2510.15859.pdf)\]

#### De-duplication and Compression

1. **Generating Data-Driven Reasoning Rubrics for Domain-Adaptive Reward Modeling**, _Sanders et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.06795.pdf)\]
2. **Confusion-Aware Rubric Optimization for LLM-based Automated Grading**, _Chu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.00451.pdf)\]

### Online and Co-evolving Generation

#### Rollout-Based Evolving Rubrics

1. **DR Tulu: Reinforcement Learning with Evolving Rubrics for Deep Research**, _Shao et al._, ICML 2026. \[[Paper](https://arxiv.org/abs/2511.19399.pdf)\]

#### Online and Alternating Optimization of Rubric Generators

1. **Online Rubrics Elicitation from Pairwise Comparisons**, _Rezaei et al._, ICML 2026. \[[Paper](https://arxiv.org/abs/2510.07284.pdf)\]
2. **Alternating Reinforcement Learning for Rubric-Based Reward Modeling in Non-Verifiable LLM Post-Training**, _Xu et al._, ICML 2026. \[[Paper](https://arxiv.org/abs/2602.01511.pdf)\]

#### Self-Evolving, Adversarial, and Memory-Driven Rubrics

1. **SibylSense: Adaptive Rubric Learning via Memory Tuning and Adversarial Probing**, _Xu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.20751.pdf)\]
2. **Open Rubric System: Scaling Reinforcement Learning with Pairwise Adaptive Rubric**, _Jia et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.14069.pdf)\]
3. **Reinforcing Chain-of-Thought Reasoning with Self-Evolving Rubrics**, _Sheng et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.10885.pdf)\]
4. **AutoRubric: Rubric-Based Generative Rewards for Faithful Multimodal Reasoning**, _Jia et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.14738.pdf)\]
5. **RLAC: Reinforcement Learning with Adversarial Critic for Free-Form Generation Tasks**, _Wu et al._, ICLR 2026. \[[Paper](https://arxiv.org/abs/2511.01758.pdf)\]

### Evaluation for Rubrics

1. **Rift: A rubric failure mode taxonomy and automated diagnostics**, _Qi et al._, ICLR 2026 Workshop DATA-FM, \[[Paper](https://openreview.net/forum?id=tCxZYDLvuu)\]
2. **RubricRAG: Towards interpretable and reliable llm evaluation via domain knowledge retrieval for rubric generation**, _Dhole et al._, SIGIR 2026, \[[Paper](https://arxiv.org/abs/2603.20882)\]
3. **Rubric-guided fine-tuning of speechllms for multi-aspect, multi-rater l2 reading-speech assessment**, _Parikh et al._, LREC 2026, \[[Paper](https://arxiv.org/abs/2603.16889)\]
4. **Comparing developer and llm biases in code evaluation**, _Mittal et al._, \[[Paper](https://arxiv.org/abs/2603.24586)\]


## Rubrics for Model Training

### Rubrics for Policy Model Training

#### Standard Rubric-based RL

1. **Checklists are better than reward models for aligning language models**, _Viswanathan et al._, NeurIPS 2025. \[[Paper](https://proceedings.neurips.cc/paper_files/paper/2025/file/a6837c1dd021f76f1b4098e3722052a8-Paper-Conference.pdf)\]
2. **Training AI Co-Scientists Using Rubric Rewards**, _Goel et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2512.23707.pdf)\]
3. **Rubrics as Rewards: Reinforcement Learning Beyond Verifiable Domains**, _Gunjal et al._, ICLR 2026. \[[Paper](https://arxiv.org/abs/2507.17746.pdf)\]
4. **Open Rubric System: Scaling Reinforcement Learning with Pairwise Adaptive Rubric**, _Jia et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.14069.pdf)\]
5. **Chasing the Tail: Effective Rubric-based Reward Modeling for Large Language Model Post-Training**, _Zhang et al._, ICLR 2026. \[[Paper](https://arxiv.org/abs/2509.21500.pdf)\]
6. **RLAC: Reinforcement Learning with Adversarial Critic for Free-Form Generation Tasks**, _Wu et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2511.01758.pdf)\]
7. **Visual Preference Optimization with Rubric Rewards**, _Yu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2604.13029.pdf)\]
8. **AutoRubric-R1V: Rubric-Based Generative Rewards for Faithful Multimodal Reasoning**, _Jia et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.14738.pdf)\]
9. **Reinforcing Chain-of-Thought Reasoning with Self-Evolving Rubrics**, _Sheng et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2602.10885.pdf)\]
10. **Dr Tulu: Reinforcement Learning with Evolving Rubrics for Deep Research**, _Shao et al._, ICML 2026. \[[Paper](https://arxiv.org/abs/2511.19399.pdf)\]
11. **OralGPT-Plus: Learning to Use Visual Tools via Reinforcement Learning for Panoramic X-ray Analysis**, _Fan et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.06366.pdf)\]

#### Advanced Reward Design

1. **Rule Based Rewards for Language Model Safety**, _Mu et al._, NeurIPS 2024. \[[Paper](https://arxiv.org/abs/2411.01111.pdf)\]
2. **Reinforcement Learning with Rubric Anchors**, _Huang et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2508.12790.pdf)\]
3. **Mock Worlds, Real Skills: Building Small Agentic Language Models with Synthetic Tasks, Simulated Environments, and Rubric-Based Rewards**, _Lyu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.22511.pdf)\]
4. **StitchCUDA: An Automated Multi-Agents End-to-End GPU Programing Framework with Rubric-based Agentic Reinforcement Learning**, _Li et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.02637.pdf)\]
5. **RuCL: Stratified Rubric-Based Curriculum Learning for Multimodal Large Language Model Reasoning**, _Chen et al._, ICML 2026. \[[Paper](https://arxiv.org/abs/2602.21628.pdf)\]
6. **Alternating Reinforcement Learning with Contextual Rubric Rewards**, _Lan_, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.15646.pdf)\]
7. **Stabilizing Rubric Integration Training via Decoupled Advantage Normalization**, _Tan et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.26535.pdf)\]
8. **Rubrics to Tokens: Bridging Response-level Rubrics and Token-level Rewards in Instruction Following Tasks**, _Xu et al._, arXiv 2026. \[[Paper](https://arxiv.org/pdf/2506.13351.pdf)\]
9. **Direct Reasoning Optimization: Token-Level Reasoning Reflectivity Meets Rubric Gates for Unverifiable Tasks**, _
#### Rubrics as Policy Guidance

1. **Breaking the Exploration Bottleneck: Rubric-Scaffolded Reinforcement Learning for General LLM Reasoning**, _Zhou et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2508.16949.pdf)\]
2. **Experience is the Best Teacher: Motivating Effective Exploration in Reinforcement Learning for LLMs**, _Zhang et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.20046.pdf)\]
3. **Think-with-Rubrics: From External Evaluator to Internal Reasoning Guidance**, _Yu et al._, arXiv 2026. \[[Paper](https://arxiv.org/pdf/2605.07461.pdf)\]

### Rubrics for Reward Model Training

#### Rubrics for Interpretability

1. **R3: Robust Rubric-Agnostic Reward Models**, _Anugraha et al._, arXiv 2025. \[[Paper](https://arxiv.org/pdf/2505.13388.pdf)\]
2. **Curing Miracle Steps in LLM Mathematical Reasoning with Rubric Rewards**, _Yuan et al._, arXiv 2025. \[[Paper](https://arxiv.org/pdf/2510.07774.pdf)\]
3. **mR3: Multilingual Rubric-Agnostic Reward Reasoning Models**, _Anugraha et al._, arXiv 2025. \[[Paper](https://arxiv.org/pdf/2510.01146.pdf)\]
4. **Omni-RRM: Advancing Omni Reward Modeling via Automatic Rubric-Grounded Preference Synthesis**, _Kong et al._, arXiv 2026. \[[Paper](https://arxiv.org/pdf/2602.00846.pdf)\]
5. **CDRRM: Contrast-Driven Rubric Generation for Reliable and Interpretable Reward Modeling**, _Liu et al._, arXiv 2026. \[[Paper](https://arxiv.org/pdf/2603.08035.pdf)\]
6. **C2: Scalable Rubric-Augmented Reward Modeling from Binary Preferences**, _Kawabata et al._, arXiv 2026. \[[Paper](https://arxiv.org/pdf/2604.13618.pdf)\]
7. **DeltaRubric: Generative Multimodal Reward Modeling via Joint Planning and Verification**, _Liu et al._, arXiv 2026. \[[Paper](https://arxiv.org/pdf/2605.09269.pdf)\]
8. **Interpretable Preferences via Multi-Objective Reward Modeling and Mixture-of-Experts**, _Wang et al._, ENNLP (Findings) 2024. \[[Paper](https://arxiv.org/pdf/2406.12845.pdf)\] 
9. **A Rubric-Supervised Critic from Sparse Real-World Outcomes**, _Wang et al._, arXiv 2026. \[[Paper](https://arxiv.org/pdf/2603.03800.pdf)\]
10. **Multidimensional Rubric-oriented Reward Model Learning via Geometric Projection Reference Constraints**, _Jin et al._, arXiv 2025. \[[Paper](https://arxiv.org/pdf/2511.16139.pdf)\]

#### Rubrics for Reward Signals

1. **Outcome Accuracy is Not Enough: Aligning the Reasoning Process of Reward Models**, _Wang et al._, arXiv 2026. \[[Paper](https://arxiv.org/pdf/2602.04649.pdf)\]
2. **Rationale Matters: Learning Transferable Rubrics via Proxy-Guided Critique for VLM Reward Models**, _Qiu et al._, arXiv 2026. \[[Paper](https://arxiv.org/pdf/2603.16600.pdf)\]

#### Rubrics for Data Construction

1. **Robust Reward Modeling via Causal Rubrics**, _Srivastava et al._, arXiv 2025. \[[Paper](https://arxiv.org/pdf/2506.16507.pdf)\]

## Rubrics for Evaluation

### Rubrics for General Task Evaluation

#### Reasoning Capability Evaluation

1. **Is Your Model Really A Good Math Reasoner? Evaluating Mathematical Reasoning with Checklist**, _Zhou et al._, arXiv 2024. \[[Paper](https://arxiv.org/abs/2407.08733)\]
2. **SedarEval: Automated Evaluation using Self-Adaptive Rubrics**, _Fan et al._, Findings of EMNLP 2024. \[[Paper](https://doi.org/10.18653/v1/2024.findings-emnlp.984)\]
3. **RefGrader: Automated Grading of Mathematical Competition Proofs using Agentic Workflows**, _Mahdavi et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.09021)\]
4. **Rubric Is All You Need: Improving LLM-Based Code Evaluation With Question-Specific Rubrics**, _Pathak et al._, ICER 2025. \[[Paper](http://dx.doi.org/10.1145/3702652.3744220)\]
5. **Comparing Developer and LLM Biases in Code Evaluation**, _Mittal et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.24586)\]
6. **ProfBench: Multi-Domain Rubrics requiring Professional Knowledge to Answer and Judge**, _Wang et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.18941)\]
7. **\$OneMillion-Bench: How Far are Language Agents from Human Experts?**, _Yang et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.07980)\]
8. **MoReBench: Evaluating Procedural and Pluralistic Moral Reasoning in Language Models, More than Outcomes**, _Chiu et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.16380)\]
9. **Qworld: Question-Specific Evaluation Criteria for LLMs**, _Gao et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.23522)\]
10. **An Efficient Rubric-based Generative Verifier for Search-Augmented LLMs**, _Ma et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.14660)\]

#### Deep Research and Open-Ended Generation Evaluation

1. **HelloBench: Evaluating Long Text Generation Capabilities of Large Language Models**, _Que et al._, arXiv 2024. \[[Paper](https://arxiv.org/abs/2409.16191)\]
2. **WritingBench: A Comprehensive Benchmark for Generative Writing**, _Wu et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2503.05244)\]
3. **DeepResearch Bench: A Comprehensive Benchmark for Deep Research Agents**, _Du et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2506.11763)\]
4. **DeepResearch Bench II: Diagnosing Deep Research Agents via Rubrics from Expert Report**, _Li et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.08536)\]
5. **DEER: A Benchmark for Evaluating Deep Research Agents on Expert Report Generation**, _Han et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2512.17776)\]
6. **ResearchRubrics: A Benchmark of Prompts and Rubrics For Evaluating Deep Research Agents**, _Sharma et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2511.07685)\]
7. **MiroEval: Benchmarking Multimodal Deep Research Agents in Process and Outcome**, _Ye et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.28407)\]
8. **Pencils Down! Automatic Rubric-based Evaluation of Retrieve/Generate Systems**, _Farzi et al._, ICTIR 2024. \[[Paper](https://doi.org/10.1145/3664190.3672511)\]
9. **Auto-Rubric: Learning to Extract Generalizable Criteria for Reward Modeling**, _Xie et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.17314)\]
10. **RubricHub: A Comprehensive and Highly Discriminative Rubric Dataset via Automated Coarse-to-Fine Generation**, _Li et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.08430)\]

#### General Agent Capability Evaluation

1. **AgentBoard: An Analytical Evaluation Board of Multi-turn LLM Agents**, _Ma et al._, arXiv 2024. \[[Paper](https://arxiv.org/abs/2401.13178)\]
2. **AdaRubric: Task-Adaptive Rubrics for LLM Agent Evaluation**, _Ding_, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.21362)\]
3. **TRAJECT-Bench: A Trajectory-Aware Benchmark for Evaluating Agentic Tool Use**, _He et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.04550)\]
4. **MCP-Universe: Benchmarking Large Language Models with Real-World Model Context Protocol Servers**, _Luo et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2508.14704)\]
5. **MultiChallenge: A Realistic Multi-Turn Conversation Evaluation Benchmark Challenging to Frontier LLMs**, _Sirdeshmukh et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2501.17399)\]
6. **SCRIBE: Structured Mid-Level Supervision for Tool-Using Language Models**, _Jiang et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.03555)\]
7. **ASTRA-bench: Evaluating Tool-Use Agent Reasoning and Action Planning with Personal User Context**, _Xiu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.01357)\]
8. **PaperBench: Evaluating AI's Ability to Replicate AI Research**, _Starace et al._, ICML 2025. \[[Paper](https://proceedings.mlr.press/v267/starace25a.html)\]
9. **Dr Tulu: Reinforcement Learning with Evolving Rubrics for Deep Research**, _Shao et al._, ICML 2026. \[[Paper](https://arxiv.org/abs/2511.19399)\]

#### Alignment Evaluation

1. **FLASK: Fine-grained Language Model Evaluation based on Alignment Skill Sets**, _Ye et al._, ICLR 2024. \[[Paper](https://proceedings.iclr.cc/paper_files/paper/2024/hash/f41b4a6b202adcd8e150a9d4f124d8f6-Abstract-Conference.html)\]
2. **InFoBench: Evaluating Instruction Following Ability in Large Language Models**, _Qin et al._, Findings of ACL 2024. \[[Paper](https://aclanthology.org/2024.findings-acl.772/)\]
3. **AdvancedIF: Rubric-Based Benchmarking and Reinforcement Learning for Advancing LLM Instruction Following**, _He et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2511.10507)\]
4. **WildBench: Benchmarking LLMs with Challenging Tasks from Real Users in the Wild**, _Lin et al._, ICLR 2025. \[[Paper](https://proceedings.iclr.cc/paper_files/paper/2025/hash/771155abaae744e08576f1f3b4b7ac0d-Abstract-Conference.html)\]
5. **G-Eval: NLG Evaluation using GPT-4 with Better Human Alignment**, _Liu et al._, EMNLP 2023. \[[Paper](https://aclanthology.org/2023.emnlp-main.153/)\]
6. **Prometheus: Inducing Fine-grained Evaluation Capability in Language Models**, _Kim et al._, ICLR 2024. \[[Paper](https://proceedings.iclr.cc/paper_files/paper/2024/hash/803485352e61e3ebf41221e4776c9fd4-Abstract-Conference.html)\]
7. **Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena**, _Zheng et al._, NeurIPS 2023. \[[Paper](https://arxiv.org/abs/2306.05685)\]
8. **RubricEval: A Rubric-Level Meta-Evaluation Benchmark for LLM Judges in Instruction Following**, _Pan et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.25133)\]
9. **RubricBench: Aligning Model-Generated Rubrics with Human Standards**, _Zhang et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.01562)\]
10. **JudgeBench: A Benchmark for Evaluating LLM-based Judges**, _Tan et al._, ICLR 2025. \[[Paper](https://proceedings.iclr.cc/paper_files/paper/2025/hash/9e720fce64f91114c49cfd640d821da3-Abstract-Conference.html)\]
11. **A StrongREJECT for Empty Jailbreaks**, _Souly et al._, arXiv 2024. \[[Paper](https://arxiv.org/abs/2402.10260)\]

### Rubrics for Specific Task Evaluation

#### Rubrics for Intermediate Trajectories

1. **PaperBench: Evaluating AI's Ability to Replicate AI Research**, _Starace et al._, ICML 2025. \[[Paper](https://proceedings.mlr.press/v267/starace25a.html)\]
2. **MoReBench: Evaluating Procedural and Pluralistic Moral Reasoning in Language Models, More than Outcomes**, _Chiu et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.16380)\]
3. **ProfBench: Multi-Domain Rubrics requiring Professional Knowledge to Answer and Judge**, _Wang et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.18941)\]
4. **Rubric Is All You Need: Improving LLM-Based Code Evaluation With Question-Specific Rubrics**, _Pathak et al._, ICER 2025. \[[Paper](http://dx.doi.org/10.1145/3702652.3744220)\]
5. **SCRIBE: Structured Mid-Level Supervision for Tool-Using Language Models**, _Jiang et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.03555)\]

#### Rubrics for Final Outputs

#### Content Quality and Factuality

1. **Pencils Down! Automatic Rubric-based Evaluation of Retrieve/Generate Systems**, _Farzi et al._, ICTIR 2024. \[[Paper](https://doi.org/10.1145/3664190.3672511)\]
2. **DeepResearch Bench: A Comprehensive Benchmark for Deep Research Agents**, _Du et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2506.11763)\]
3. **DeepResearch Bench II: Diagnosing Deep Research Agents via Rubrics from Expert Report**, _Li et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.08536)\]
4. **HealthBench: Evaluating Large Language Models Towards Improved Human Health**, _Arora et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2505.08775)\]
5. **PRBench: Large-Scale Expert Rubrics for Evaluating High-Stakes Professional Reasoning**, _Akyurek et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2511.11562)\]
6. **ASTRA-bench: Evaluating Tool-Use Agent Reasoning and Action Planning with Personal User Context**, _Xiu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.01357)\]
7. **SCRIBE: Structured Mid-Level Supervision for Tool-Using Language Models**, _Jiang et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.03555)\]
8. **TechImage-Bench: Rubric-Based Evaluation for Technical Image Generation**, _Ni et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2512.12220)\]
9. **A Benchmark and Agentic Framework for Omni-Modal Reasoning and Tool Use in Long Videos**, _Kurpath et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2512.16978)\]

#### Safety and Risk Auditing

1. **HealthBench: Evaluating Large Language Models Towards Improved Human Health**, _Arora et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2505.08775)\]
2. **RubricRAG: Towards Interpretable and Reliable LLM Evaluation via Domain Knowledge Retrieval for Rubric Generation**, _Dhole et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.20882)\]
3. **MoReBench: Evaluating Procedural and Pluralistic Moral Reasoning in Language Models, More than Outcomes**, _Chiu et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.16380)\]
4. **Datasheets Aren't Enough: DataRubrics for Automated Quality Metrics and Accountability**, _Winata et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2506.01789)\]

#### Professional Presentation and Structural Coherence

1. **DEER: A Benchmark for Evaluating Deep Research Agents on Expert Report Generation**, _Han et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2512.17776)\]
2. **ProfBench: Multi-Domain Rubrics requiring Professional Knowledge to Answer and Judge**, _Wang et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.18941)\]
3. **\$OneMillion-Bench: How Far are Language Agents from Human Experts?**, _Yang et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.07980)\]
4. **From Intuition to Calibrated Judgment: A Rubric-Based Expert-Panel Study of Human Detection of LLM-Generated Korean Text**, _Park et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2601.19913)\]
5. **PresentBench: A Fine-Grained Rubric-Based Benchmark for Slide Generation**, _Chen et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.07244)\]
6. **Rubric-Guided Fine-tuning of SpeechLLMs for Multi-Aspect, Multi-Rater L2 Reading-Speech Assessment**, _Parikh et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.16889)\]

#### Practical Utility and Actionability

1. **DEER: A Benchmark for Evaluating Deep Research Agents on Expert Report Generation**, _Han et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2512.17776)\]
2. **MoReBench: Evaluating Procedural and Pluralistic Moral Reasoning in Language Models, More than Outcomes**, _Chiu et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2510.16380)\]
3. **PRBench: Large-Scale Expert Rubrics for Evaluating High-Stakes Professional Reasoning**, _Akyurek et al._, arXiv 2025. \[[Paper](https://arxiv.org/abs/2511.11562)\]
4. **ASTRA-bench: Evaluating Tool-Use Agent Reasoning and Action Planning with Personal User Context**, _Xiu et al._, arXiv 2026. \[[Paper](https://arxiv.org/abs/2603.01357)\]
5. **LLM-Rubric: A Multidimensional, Calibrated Approach to Automated Evaluation of Natural Language Texts**, _Hashemi et al._, ACL 2024. \[[Paper](https://aclanthology.org/2024.acl-long.745/)\]


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
