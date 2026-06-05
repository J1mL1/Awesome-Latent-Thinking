# Awesome Latent Thinking [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

Latent thinking, latent Chain-of-Thought, continuous reasoning, and multimodal intermediate-state reasoning for AI systems.

This list follows the taxonomy in [latent thinking survey.md](latent%20thinking%20survey.md), organizing papers by intermediate-state carrier, dynamics, semantic role, modality, and contribution type.

## Contents

- [Surveys and Roadmaps](#surveys-and-roadmaps)
- [Soft Readout](#soft-readout)
- [Native Hidden-State](#native-hidden-state)
- [Modality-Grounded Latent](#modality-grounded-latent)
- [Interpretability](#interpretability)
- [Benchmarks and Evaluation](#benchmarks-and-evaluation)
- [Related Awesome Lists](#related-awesome-lists)

## Legend

- Carrier: `soft-readout`, `hidden-state`, `modality-latent`.
- Dynamics: `autoregressive`, `depth-recurrence`, `memory-state`, `parallel`.
- Semantic role: `free-form`, `compression`, `planning`, `reconstruction`, `posterior`.
- Modality: `language`, `vision-language`, `video-language`, `audio-language`, `omnimodal`.
- Contribution: `method`, `analysis`, `theory`.

## Surveys and Roadmaps

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | The Latent Space: Foundation, Evolution, Mechanism, Ability, and Outlook | arXiv | [Paper](https://arxiv.org/abs/2604.02029) | [Code](https://github.com/YU-deep/Awesome-Latent-Space) | `survey`, `latent-space` | Unified latent-space survey across foundation, evolution, mechanism, ability, and outlook. |
| 2025 | Implicit Reasoning in Large Language Models: A Comprehensive Survey | arXiv | [Paper](https://arxiv.org/abs/2509.02350) | [Code](https://github.com/digailab/awesome-llm-implicit-reasoning) | `survey`, `efficient-reasoning` | Taxonomy of implicit reasoning by execution paradigm: latent optimization, signal-guided control, and layer-recurrent execution. |
| 2025 | A Survey on Latent Reasoning | arXiv | [Paper](https://arxiv.org/abs/2507.06203) | [Code](https://github.com/multimodal-art-projection/LatentCoT-Horizon) | `survey`, `latent-cot` | Organizes latent reasoning into vertical recurrence and horizontal recurrence, plus fine-tuning strategies that internalize explicit traces. |
| 2025 | Thinking with Images for Multimodal Reasoning: Foundations, Methods, and Future Frontiers | arXiv | [Paper](https://arxiv.org/abs/2506.23918) | [Code](https://github.com/zhaochen0110/Awesome_Think_With_Images) | `survey`, `multimodal`, `think-with-images` | Surveys the shift from thinking about images to thinking with images as a dynamic cognitive workspace. |
| 2025 | Reasoning Beyond Language: A Comprehensive Survey on Latent Chain-of-Thought Reasoning | arXiv | [Paper](https://arxiv.org/abs/2505.16782) | [Code](https://github.com/EIT-NLP/Awesome-Latent-CoT) | `survey`, `latent-cot` | Latent CoT taxonomy from token-wise horizontal methods to layer-wise vertical strategies, with analysis and applications. |
| 2025 | Perception, Reason, Think, and Plan: A Survey on Large Multimodal Reasoning Models | arXiv | [Paper](https://arxiv.org/abs/2505.04921) | [Code](https://github.com/HITsz-TMG/Awesome-Large-Multimodal-Reasoning-Models) | `survey`, `multimodal` | Four-stage roadmap of large multimodal reasoning models from modular pipelines to native agentic reasoning. |
| 2025 | Efficient Reasoning Models: A Survey | arXiv | [Paper](https://arxiv.org/abs/2504.10903) | [Code](https://github.com/fscdc/Awesome-Efficient-Reasoning-Models) | `survey`, `efficient-reasoning` | Categorizes efficient reasoning into shorter CoT, smaller models, and faster decoding. |
| 2025 | Harnessing the Reasoning Economy | arXiv | [Paper](https://arxiv.org/abs/2503.24377) | [Code](https://github.com/DevoAllen/Awesome-Reasoning-Economy-Papers) | `survey`, `reasoning-economy` | Surveys reasoning economy across cost, token budget, latency, and deployment trade-offs. |
| 2025 | Stop Overthinking: A Survey on Efficient Reasoning for Large Language Models | TMLR 2025 | [Paper](https://arxiv.org/abs/2503.16419) | [Code](https://github.com/Eclipsess/Awesome-Efficient-Reasoning-LLMs) | `survey`, `efficient-reasoning`, `overthinking` | Broad survey of efficient LLM reasoning, including concise reasoning and overthinking reduction. |
| 2025 | Multimodal Chain-of-Thought Reasoning: A Comprehensive Survey | arXiv | [Paper](https://arxiv.org/abs/2503.12605) | [Code](https://github.com/yaotingwangofficial/Awesome-MCoT) | `survey`, `multimodal` | First systematic survey of multimodal CoT across image, video, audio, 3D, and structured data. |

[Back](#contents)

## Soft Readout

### Compressed Soft Readout

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2025 | Token Assorted | ICML 2025 | [Paper](https://proceedings.mlr.press/v267/su25g.html) | — | `method`, `soft-readout`, `autoregressive`, `compression`, `language` | Mixes latent and text tokens as a hybrid soft-readout carrier. |
| 2025 | SoftCoT | ACL 2025 | [Paper](https://aclanthology.org/2025.acl-long.1137/) | — | `method`, `soft-readout`, `autoregressive`, `compression`, `language` | Soft thought tokens replace long explicit CoT. |
| 2025 | SoftCoT++ | arXiv | [Paper](https://arxiv.org/abs/2505.11484) | — | `method`, `soft-readout`, `parallel`, `compression`, `language` | Parallel soft-trajectory refinement for test-time latent scaling. |
| 2025 | Latent Reasoning in LLMs as a Vocabulary-Space Superposition | arXiv | [Paper](https://arxiv.org/abs/2510.15522) | [📦](https://github.com/DJC-GO-SOLO/Latent-SFT) | `method`, `soft-readout`, `autoregressive`, `compression`, `language` | Maps latent thoughts to vocabulary-space superpositions. |
| 2025 | SemCoT | NeurIPS 2025 | [Paper](https://proceedings.neurips.cc/paper_files/paper/2025/file/3ddbd473456a57e3cafb1ee51ddf8ff6-Paper-Conference.pdf) | [📦](https://github.com/YinhanHe123/SemCoT) | `method`, `soft-readout`, `autoregressive`, `compression`, `language` | Semantically aligned implicit tokens compress explicit CoT. |
| 2025 | SynAdapt: Learning Adaptive Reasoning in Large Language Models via Synthetic Continuous Chain-of-Thought | arXiv | [Paper](https://arxiv.org/abs/2508.00574) | — | `method`, `soft-readout`, `autoregressive`, `compression`, `language` | Synthetic continuous CoT alignment with difficulty-aware rethinking. |
| 2025 | Lightweight Latent Reasoning for Narrative Tasks | arXiv | [Paper](https://arxiv.org/abs/2512.02240) | — | `method`, `soft-readout`, `autoregressive`, `compression`, `language` | Reasoning projector emits continuous latent tokens interleaved with discrete sampling. |

[Back](#contents)

### Concept and Embedding Readout

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2025 | LLM Pretraining with Continuous Concepts | arXiv | [Paper](https://arxiv.org/abs/2502.08524) | [📦](https://github.com/facebookresearch/RAM/tree/main/projects/cocomix) | `method`, `soft-readout`, `autoregressive`, `free-form`, `language` | Continuous concepts as soft semantic carriers for implicit reasoning. |
| 2024 | Large Concept Models | arXiv | [Paper](https://arxiv.org/abs/2412.08821) | — | `method`, `soft-readout`, `autoregressive`, `free-form`, `omnimodal` | Sentence/concept embeddings as high-level soft semantic reasoning carriers. |
| 2024 | Latent Space Chain-of-Embedding Enables Output-free LLM Self-Evaluation | ICLR 2025 | [Paper](https://openreview.net/forum?id=jxo70B9fQo) | [📦](https://github.com/Alsace08/Chain-of-Embedding) | `method`, `soft-readout`, `autoregressive`, `reconstruction`, `language` | Embedding-chain self-evaluation without generating explicit reasoning text. |
| 2025 | Latent Preference Coding | arXiv | [Paper](https://arxiv.org/abs/2505.04993) | — | `method`, `soft-readout`, `autoregressive`, `posterior`, `language` | Discrete latent codes model preference posteriors for efficient reasoning. |
| 2024 | Multimodal Latent Language Modeling with Next-Token Diffusion | arXiv | [Paper](https://arxiv.org/abs/2412.08635) | — | `method`, `soft-readout`, `autoregressive`, `reconstruction`, `omnimodal` | Continuous latent vectors with diffusion readout for unified multimodal modeling. |
| 2026 | Dynamic Large Concept Models Latent Reasoning in an Adaptive Semantic Space | arXiv | [Paper](https://arxiv.org/abs/2512.24617) | — | `method`, `soft-readout`, `autoregressive`, `free-form`, `language` | Semantic-level latent reasoning in an adaptive concept space. |
| 2025 | Fast Thinking for Large Language Models | arXiv | [Paper](https://arxiv.org/abs/2509.23633) | — | `method`, `soft-readout`, `autoregressive`, `planning`, `language` | Latent codebooks plus GainRouter enable single-pass strategy routing via continuous thoughts. |
| 2025 | Enhancing Latent Computation in Transformers with Latent Tokens | arXiv | [Paper](https://arxiv.org/abs/2505.12629) | — | `method`, `soft-readout`, `autoregressive`, `free-form`, `language` | Learnable dummy latent tokens guide implicit computation during decoding. |

[Back](#contents)

### Distributional Soft Search

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2025 | Soft Thinking | NeurIPS 2025 | [Paper](https://proceedings.neurips.cc/paper_files/paper/2025/file/f7396d1c54d51416958d63e285377103-Paper-Conference.pdf) | [📦](https://github.com/eric-ai-lab/Soft-Thinking) | `method`, `soft-readout`, `parallel`, `free-form`, `language` | Samples and searches in a continuous concept space instead of explicit CoT. |
| 2025 | Continuous Chain of Thought Enables Parallel Exploration and Reasoning | ICLR 2026 | [Paper](https://openreview.net/forum?id=sTPKDKn5ig) | — | `method`, `soft-readout`, `parallel`, `free-form`, `language` | Continuous thoughts enable parallel implicit exploration. |
| 2025 | Parallel Continuous Chain-of-Thought with Jacobi Iteration | EMNLP 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.47/) | [📦](https://github.com/whyNLP/PCCoT) | `method`, `soft-readout`, `parallel`, `free-form`, `language` | Jacobi-style parallel updates for continuous implicit CoT. |
| 2026 | GTS | arXiv | [Paper](https://arxiv.org/abs/2602.14077) | — | `method`, `soft-readout`, `parallel`, `free-form`, `language` | Explicitly models thought distributions with Gaussian sampling. |
| 2025 | SofT-GRPO | arXiv | [Paper](https://arxiv.org/abs/2511.06411) | [📦](https://github.com/zz1358m/SofT-GRPO-master) | `method`, `soft-readout`, `parallel`, `posterior`, `language` | RL with Gumbel/soft-thinking for posterior-style latent optimization. |
| 2025 | Text Generation Beyond Discrete Token Sampling | arXiv | [Paper](https://arxiv.org/abs/2505.14827) | — | `method`, `soft-readout`, `parallel`, `free-form`, `language` | Generates text directly in continuous readout space. |
| 2025 | Learning to Reason with Mixture of Tokens | arXiv | [Paper](https://arxiv.org/abs/2509.21482) | — | `method`, `soft-readout`, `parallel`, `free-form`, `language` | Continuous token-mixture reasoning under RLVR for higher-entropy exploration. |
| 2025 | MARCOS: Deep Thinking by Markov Chain of Continuous Thoughts | arXiv | [Paper](https://arxiv.org/abs/2509.25020) | — | `method`, `soft-readout`, `parallel`, `posterior`, `language` | Models reasoning as a Markov chain of continuous thoughts with variational training. |
| 2025 | Soft Tokens, Hard Truths | arXiv | [Paper](https://arxiv.org/abs/2509.19170) | — | `method`, `soft-readout`, `parallel`, `free-form`, `language` | Weighted embeddings and soft tokens for implicit distributional reasoning. |
| 2026 | SeLaR: Selective Latent Reasoning in Large Language Models | ACL 2026 | [Paper](https://arxiv.org/abs/2604.08299) | — | `method`, `soft-readout`, `autoregressive`, `free-form`, `language` | Entropy-gated soft embeddings at low-confidence steps for efficient multi-path latent exploration. |
| 2026 | NF-CoT: Latent Reasoning with Normalizing Flows | arXiv | [Paper](https://arxiv.org/abs/2606.06447) | - | `method`, `soft-readout`, `parallel`, `free-form`, `language` | Models continuous thoughts with normalizing flows while preserving KV-cache compatibility and left-to-right probabilistic decoding. |
| 2026 | CopT: Contrastive On-Policy Thinking with Continuous Spaces for General and Agentic Reasoning | arXiv | [Paper](https://arxiv.org/abs/2605.20075) | - | `method`, `soft-readout`, `parallel`, `free-form`, `language` | Uses contrastive on-policy thinking in continuous space to reduce performative reasoning overhead for general and agentic tasks. |

[Back](#contents)

## Native Hidden-State

### Hidden-Chain Compression

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2024 | Hidden Chain-of-Thought Decoding | arXiv | [Paper](https://arxiv.org/abs/2409.08561) | — | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Decodes with hidden CoT instead of explicit rationale tokens. |
| 2024 | Training Large Language Models to Reason in a Continuous Latent Space | COLM 2025 | [Paper](https://openreview.net/forum?id=Itxz7S4Ip3) | [📦](https://github.com/facebookresearch/coconut) | `method`, `hidden-state`, `autoregressive`, `free-form`, `language` | Uses hidden states as continuous thoughts instead of explicit CoT. |
| 2024 | Compressed Chain of Thought | arXiv | [Paper](https://arxiv.org/abs/2412.13171) | — | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Compresses explicit CoT into dense reasoning states. |
| 2025 | LightThinker | EMNLP 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.673/) | [📦](https://github.com/zjunlp/LightThinker) | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Step-by-step compression of explicit CoT into latent states. |
| 2025 | CODI | EMNLP 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.36/) | [📦](https://github.com/zhenyi-shen/CODI) | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Self-distills CoT into a continuous latent space. |
| 2025 | Hybrid Latent Reasoning via Reinforcement Learning | NeurIPS 2025 | [Paper](https://openreview.net/forum?id=LjtgTpWH71) | [📦](https://github.com/Yueeeeeeee/HRPO) | `method`, `hidden-state`, `autoregressive`, `posterior`, `language` | Mixes hidden states and tokens optimized with RL for implicit reasoning. |
| 2025 | DART | EMNLP 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.256/) | — | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Distills autoregressive reasoning into silent latent thoughts. |
| 2025 | SIM-CoT | ICLR 2026 | [Paper](https://openreview.net/forum?id=6YRJ4jmVQl) | [📦](https://github.com/InternLM/SIM-CoT) | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Token-level supervised implicit chain-of-thought. |
| 2025 | Think Silently, Think Fast | NeurIPS 2025 | [Paper](https://openreview.net/forum?id=AQsko3PPUe) | [📦](https://github.com/xiaomi-research/colar) | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Dynamic latent compression of reasoning chains. |
| 2025 | Efficient Post-Training Refinement of Latent Reasoning in LLMs | arXiv | [Paper](https://arxiv.org/abs/2506.08552) | — | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Post-training compression and refinement for latent reasoning models. |
| 2026 | Latent Reasoning with Supervised Thinking States | arXiv | [Paper](https://arxiv.org/abs/2602.08332) | — | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Supervised thinking states carry intermediate reasoning in hidden space. |
| 2025 | R-Capsule: Compressing High-Level Plans for Efficient Large Language Model Reasoning | arXiv | [Paper](https://arxiv.org/abs/2509.22131) | — | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Compresses high-level plans into compact reconstructible reasoning capsules. |
| 2025 | LTA-thinker: Latent Thought-Augmented Training Framework for Large Language Models on Complex Reasoning | arXiv | [Paper](https://arxiv.org/abs/2509.12875) | — | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Learnable priors and distribution-direction losses enhance latent thought training. |
| 2025 | Enhancing Non-Core Language Instruction-Following in Speech LLMs via Semi-Implicit Cross-Lingual CoT Reasoning | arXiv | [Paper](https://arxiv.org/abs/2504.20835) | — | `method`, `hidden-state`, `autoregressive`, `compression`, `audio-language` | Semi-implicit cross-lingual CoT with progressively compressible reasoning tokens. |
| 2024 | From Explicit CoT to Implicit CoT: Learning to Internalize CoT Step by Step (ICoT-SI) | arXiv | [Paper](https://arxiv.org/abs/2405.14838) | [📦](https://github.com/da03/Internalize_CoT_Step_by_Step) | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Curriculum removes explicit CoT tokens and internalizes steps into hidden states. |
| 2023 | Implicit Chain of Thought Reasoning via Knowledge Distillation | arXiv | [Paper](https://arxiv.org/abs/2311.01460) | [📦](https://github.com/da03/implicit_chain_of_thought/) | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Emulator distills explicit CoT hidden states into an implicit-reasoning student. |
| 2026 | LatentChem: From Textual CoT to Latent Thinking in Chemical Reasoning | ICML 2026 | [Paper](https://arxiv.org/abs/2602.07075) | — | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Internalizes textual chemical CoT into continuous latent thinking. |
| 2026 | LoRi: Low-Rank Distillation for Implicit Reasoning | arXiv | [Paper](https://arxiv.org/abs/2606.05315) | - | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Distills implicit reasoning by aligning low-rank teacher and student hidden-state trajectories in a shared subspace. |
| 2026 | LaSR: Context-Aware Speech Recognition via Latent Reasoning | arXiv | [Paper](https://arxiv.org/abs/2606.00507) | - | `method`, `hidden-state`, `autoregressive`, `compression`, `audio-language` | Uses CoT-supervised latent reasoning trajectories to improve context-aware speech recognition in speech language models. |
| 2026 | VITAL: Visual-Semantic Dual Supervision for Enhanced and Interpretable Latent Reasoning in Medical MLLMs | arXiv | [Paper](https://arxiv.org/abs/2605.28422) | - | `method`, `hidden-state`, `autoregressive`, `compression`, `vision-language` | Adds visual and semantic supervision so medical MLLMs can reconstruct reasoning chains from latent states. |
| 2026 | CIRF: Tokenizing Chain-of-Thoughts into Reusable Functional Units for Efficient Latent Reasoning | arXiv | [Paper](https://arxiv.org/abs/2605.28292) | - | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Decomposes CoT into reusable functional tokens that align explicit rationales with efficient latent reasoning. |
| 2026 | Pair-In, Pair-Out: Latent Multi-Token Prediction for Efficient LLMs | arXiv | [Paper](https://arxiv.org/abs/2605.27255) | - | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Unifies latent compression and multi-token prediction to reduce verification overhead in efficient language modeling. |
| 2026 | RuPLaR: Efficient Latent Compression of LLM Reasoning Chains with Rule-Based Priors | arXiv | [Paper](https://arxiv.org/abs/2605.09346) | - | `method`, `hidden-state`, `autoregressive`, `compression`, `language` | Uses rule-based priors to compress multi-step CoT into compact latent reasoning steps. |

[Back](#contents)

### Hidden-Chain Control

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | Latent Thoughts Tuning | arXiv | [Paper](https://arxiv.org/abs/2602.10229) | — | `method`, `hidden-state`, `autoregressive`, `free-form`, `language` | Fuses context and prediction to construct stable latent thoughts for implicit reasoning. |
| 2026 | ThinkRouter | arXiv | [Paper](https://arxiv.org/abs/2602.11683) | — | `method`, `hidden-state`, `autoregressive`, `planning`, `language` | Routes between latent and discrete thinking modes for efficient inference. |
| 2026 | Latent Chain-of-Thought as Planning Decoupling Reasoning from Verbalization | arXiv | [Paper](https://arxiv.org/abs/2601.21358) | [📦](https://github.com/zz1358m/ATP-Latent-master) | `method`, `hidden-state`, `autoregressive`, `planning`, `language` | Formulates latent CoT as planning decoupled from verbalization. |
| 2025 | LatentR³: Reinforced Latent Reasoning for LLM-based Recommendation | arXiv | [Paper](https://arxiv.org/abs/2505.19092) | - | `method`, `hidden-state`, `autoregressive`, `posterior`, `language` | Uses a small set of latent reasoning tokens with SFT and RL to support recommendation without explicit CoT text. |
| 2025 | Think Before Recommend: Unleashing the Latent Reasoning Power for Sequential Recommendation | arXiv | [Paper](https://arxiv.org/abs/2503.22675) | - | `method`, `hidden-state`, `autoregressive`, `free-form`, `language` | Recursively feeds hidden states with reasoning-position encodings for implicit multi-step sequential recommendation. |
| 2026 | SwiReasoning: Switch-Thinking in Latent and Explicit for Pareto-Superior Reasoning LLMs | ICLR 2026 | [Paper](https://openreview.net/forum?id=t33kMzEAg8) | [📦](https://github.com/sdc17/SwiReasoning) | `method`, `hidden-state`, `autoregressive`, `free-form`, `language` | Training-free switching between explicit CoT and latent reasoning to curb overthinking. |
| 2025 | JEPA-Reasoner: Decoupling Latent Reasoning from Token Generation | arXiv | [Paper](https://arxiv.org/abs/2512.19171) | — | `method`, `hidden-state`, `autoregressive`, `free-form`, `language` | JEPA engine reasons in continuous space; Talker decodes text without token error backflow. |
| 2025 | iCLP: Large Language Model Reasoning with Implicit Cognition Latent Planning | arXiv | [Paper](https://arxiv.org/abs/2512.24014) | [📦](https://github.com/AgenticFinLab/latent-planning) | `method`, `hidden-state`, `autoregressive`, `planning`, `language` | VQ latent plans distilled from explicit plans for implicit inference-time planning. |
| 2024 | Let's Think Dot by Dot: Hidden Computation in Transformer Language Models | COLM 2024 | [Paper](https://openreview.net/forum?id=NikbrdtYvG) | [📦](https://github.com/JacobPfau/fillerTokens) | `method`, `hidden-state`, `autoregressive`, `free-form`, `language` | Uses filler tokens to provide non-semantic extra computation steps beyond explicit Chain-of-Thought. |
| 2025 | Learning More Effective Representations for Dense Retrieval through Deliberate Thinking before Search | arXiv | [Paper](https://arxiv.org/abs/2502.12974) | [📦](https://github.com/OpenBMB/DEBATER) | `method`, `hidden-state`, `autoregressive`, `planning`, `language` | Latent-space deliberation before search for efficient retrieval reasoning. |
| 2025 | Bridging Search and Recommendation through Latent Cross Reasoning | arXiv | [Paper](https://arxiv.org/abs/2508.04152) | - | `method`, `hidden-state`, `autoregressive`, `free-form`, `language` | Uses latent cross reasoning to connect search and recommendation representations before prediction. |
| 2026 | TARPO: Token-Wise Latent-Explicit Reasoning via Action-Routing Policy Optimization | arXiv | [Paper](https://arxiv.org/abs/2606.05859) | - | `method`, `hidden-state`, `autoregressive`, `planning`, `language` | Learns a token-wise routing policy that switches between explicit tokens and latent reasoning under RL. |
| 2026 | MIRAGE: Mobile Agents with Implicit Reasoning and Generative World Models | arXiv | [Paper](https://arxiv.org/abs/2606.04627) | - | `method`, `hidden-state`, `autoregressive`, `planning`, `vision-language` | Distills mobile-agent reasoning into compact hidden states and predicts future interface states with a generative world model. |
| 2026 | LatentRouter: Can We Choose the Right Multimodal Model Before Seeing Its Answer? | arXiv | [Paper](https://arxiv.org/abs/2605.11301) | - | `method`, `hidden-state`, `autoregressive`, `planning`, `vision-language` | Learns latent routing capsules to predict counterfactual multimodal model utility before answer generation. |

[Back](#contents)

### Depth-Loop Refinement

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2023 | CoTFormer | ICLR 2025 | [Paper](https://openreview.net/forum?id=8wAL9SmUk8) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Budget-adaptive internal thinking via depth refinement. |
| 2025 | Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach | NeurIPS 2025 | [Paper](https://proceedings.neurips.cc/paper_files/paper/2025/file/3b01972cf31e6fa0fe29e4b8b5c2a0a1-Paper-Conference.pdf) | [📦](https://github.com/seal-rg/recurrent-pretraining) | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Recurrent depth allocates extra test-time compute in latent space. |
| 2025 | Loop-Aligned Reasoning (RELAY) | arXiv | [Paper](https://arxiv.org/abs/2502.08482) | [📦](https://github.com/qifanyu/RELAY) | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Aligns autoregressive CoT supervision to looped internal reasoning. |
| 2025 | Inner Thinking Transformer | arXiv | [Paper](https://arxiv.org/abs/2502.13842) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Dynamically expands internal thinking depth per token. |
| 2025 | Reasoning with Latent Thoughts: On the Power of Looped Transformers | ICLR 2025 | [Paper](https://openreview.net/forum?id=din0lGfZFd) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Looped transformers deepen thinking through layer recurrence. |
| 2025 | Pretraining Language Models to Ponder in Continuous Space | ICLR 2026 | [Paper](https://openreview.net/forum?id=UrM4MNRYZm) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Pondering in continuous space via iterative depth refinement. |
| 2025 | Hierarchical Reasoning Model | arXiv | [Paper](https://arxiv.org/abs/2506.21734) | [📦](https://github.com/sapientinc/HRM) | `method`, `hidden-state`, `depth-recurrence`, `planning`, `language` | Hierarchical recursive subproblem solving in latent space. |
| 2025 | Mixture-of-Recursions | arXiv | [Paper](https://arxiv.org/abs/2507.10524) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Token-level dynamic recursive depth for adaptive internal thinking. |
| 2025 | Scaling Latent Reasoning via Looped Language Models | arXiv | [Paper](https://arxiv.org/abs/2510.25741) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Looped language models scale latent reasoning through depth recurrence. |
| 2025 | Think-at-Hard Selective Latent Iterations to Improve Reasoning Language Models | arXiv | [Paper](https://arxiv.org/abs/2511.08577) | [📦](https://github.com/thu-nics/TaH) | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Triggers extra latent iterations only on hard tokens for efficient test-time depth. |
| 2025 | Learning to Ponder: Adaptive Reasoning in Latent Space | arXiv | [Paper](https://arxiv.org/abs/2509.24238) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Lightweight controller adapts test-time latent depth per instance without backbone changes. |
| 2025 | System-1.5 Reasoning: Traversal in Language and Latent Spaces with Dynamic Shortcuts | arXiv | [Paper](https://arxiv.org/abs/2505.18962) | — | `method`, `hidden-state`, `depth-recurrence`, `compression`, `language` | Dynamic shortcuts reuse hidden states across steps to allocate compute efficiently. |
| 2025 | LARES: Latent Reasoning for Sequential Recommendation | arXiv | [Paper](https://arxiv.org/abs/2505.16865) | - | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Combines recurrent latent reasoning, trajectory alignment, and RL post-training for sequential recommendation. |
| 2025 | PonderLM-2: Pretraining LLM with Latent Thoughts in Continuous Space | arXiv | [Paper](https://arxiv.org/abs/2509.23184) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Emits continuous latent thoughts before each output token during pretraining. |
| 2026 | Depth-Recurrent Attention Mixtures: Giving Latent Reasoning the Attention it Deserves | arXiv | [Paper](https://arxiv.org/abs/2601.21582) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Depth-recurrent attention mixtures scale latent reasoning under a fixed token budget. |
| 2026 | LoopFormer: Elastic-Depth Looped Transformers for Latent Reasoning via Shortcut Modulation | ICLR 2026 | [Paper](https://openreview.net/forum?id=RzYXb5YWBs) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Time/step-conditioned loops with budget-tunable elastic-depth latent reasoning. |
| 2025 | SpiralThinker: Latent Reasoning through an Iterative Process with Text–Latent Interleaving | ACL 2026 Findings | [Paper](https://openreview.net/forum?id=ZbYQ91Zw0t) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Iteratively refines latent states interleaved with text reasoning. |
| 2024 | Think before you speak: Training Language Models With Pause Tokens | ICLR 2024 | [Paper](https://openreview.net/forum?id=ph04CRkPdC) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Pause tokens delay readout to buy extra hidden-layer computation. |
| 2024 | Thinking Tokens for Language Modeling | arXiv | [Paper](https://arxiv.org/abs/2405.08644) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Inserts thinking tokens to obtain more latent update steps in RNN LMs. |
| 2025 | The 4th Dimension for Scaling Model Size | arXiv | [Paper](https://arxiv.org/abs/2506.18233) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Recurrent depth as a fourth scaling dimension for latent reasoning. |
| 2025 | Skip a Layer or Loop It? Test-Time Depth Adaptation of Pretrained LLMs | arXiv | [Paper](https://arxiv.org/abs/2507.07996) | — | `method`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Test-time layer looping/skipping adapts effective depth under a compute budget. |

[Back](#contents)

### Memory and State Evolution

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2023 | Adapting Language Models to Compress Contexts | EMNLP 2023 | [Paper](https://aclanthology.org/2023.emnlp-main.232/) | — | `method`, `hidden-state`, `memory-state`, `compression`, `language` | Compresses long context into summary vectors used as latent reasoning memory. |
| 2024 | Deliberation in Latent Space via Differentiable Cache Augmentation | arXiv | [Paper](https://arxiv.org/abs/2412.17747) | — | `method`, `hidden-state`, `memory-state`, `compression`, `language` | Injects latent computation directly into KV/cache. |
| 2025 | KaVa | ICLR 2026 | [Paper](https://openreview.net/forum?id=ePrhcLbtGv) | — | `method`, `hidden-state`, `memory-state`, `compression`, `language` | Compressed KV trajectories supervise latent reasoning. |
| 2019 | Transformer-XL | ACL 2019 | [Paper](https://aclanthology.org/P19-1285/) | [📦](https://github.com/kimiyoung/transformer-xl) | `method`, `hidden-state`, `memory-state`, `free-form`, `language` | Segment recurrence enables persistent latent state across long contexts. |
| 2019 | Compressive Transformers | arXiv | [Paper](https://arxiv.org/abs/1911.05507) | — | `method`, `hidden-state`, `memory-state`, `compression`, `language` | Compresses past states into memory for long-horizon latent context. |
| 2022 | Memorizing Transformers | ICLR 2022 | [Paper](https://openreview.net/forum?id=TrjbxzRcnf-) | — | `method`, `hidden-state`, `memory-state`, `free-form`, `language` | Uses external kNN memory to retrieve and reuse long-range hidden states during sequence modeling. |
| 2016 | Using Fast Weights to Attend to the Recent Past | NeurIPS 2016 | [Paper](https://papers.nips.cc/paper/6573-using-fast-weights-to-attend-to-the-recent-past) | — | `method`, `hidden-state`, `memory-state`, `free-form`, `language` | Fast weights as classic dynamic latent memory for efficient recurrence. |
| 2021 | Linear Transformers Are Secretly Fast Weight Programmers | arXiv | [Paper](https://arxiv.org/abs/2102.11174) | — | `method`, `hidden-state`, `memory-state`, `free-form`, `language` | Interprets linear attention as fast-weight latent state programming. |
| 2021 | Going Beyond Linear Transformers with Recurrent Fast Weight Programmers | NeurIPS 2021 | [Paper](https://openreview.net/forum?id=ot2ORiBqTa1) | — | `method`, `hidden-state`, `memory-state`, `free-form`, `language` | Recurrence plus fast weights for efficient state evolution. |
| 2025 | MeSH | ICLR 2026 | [Paper](https://openreview.net/forum?id=IhTrFvY7p3) | — | `method`, `hidden-state`, `memory-state`, `free-form`, `language` | Persistent memory highways carry evolving intermediate reasoning state. |
| 2026 | The Silent Thought | ICML 2026 | [Paper](https://arxiv.org/abs/2603.17837) | — | `method`, `hidden-state`, `memory-state`, `posterior`, `audio-language` | Recurrent latent thinking while listening in audio-language models. |
| 2025 | Latent Collaboration in Multi-Agent Systems | ICML 2026 | [Paper](https://icml.cc/virtual/2026/poster/61180) | [📦](https://github.com/Gen-Verse/LatentMAS) | `method`, `hidden-state`, `memory-state`, `free-form`, `omnimodal` | Agents share latent working memory for efficient collaboration. |
| 2026 | Latent-DARM Bridging Discrete Diffusion and Autoregressive Models for Reasoning | ICLR 2026 Workshop | [Paper](https://openreview.net/forum?id=5y0tSg0dTf) | — | `method`, `hidden-state`, `memory-state`, `planning`, `language` | Latent interface connects a diffusion planner to an autoregressive executor. |
| 2025 | Towards General Continuous Memory for Vision-Language Models (CoMEM) | arXiv | [Paper](https://arxiv.org/abs/2505.17670) | — | `method`, `hidden-state`, `memory-state`, `free-form`, `vision-language` | Compresses multimodal knowledge into few continuous embeddings for efficient VLM reasoning. |
| 2025 | Identity Bridge: Enabling Implicit Reasoning via Shared Latent Memory | arXiv | [Paper](https://arxiv.org/abs/2509.24653) | — | `method`, `hidden-state`, `memory-state`, `free-form`, `language` | Shared latent memory supports efficient implicit multi-step reasoning. |
| 2026 | Beyond Tokens: A Unified Framework for Latent Communication in LLM-Based Multi-Agent Systems | arXiv | [Paper](https://arxiv.org/abs/2606.05711) | - | `method`, `hidden-state`, `memory-state`, `free-form`, `omnimodal` | Replaces text messages with shared latent communication to reduce discretization loss, reasoning cost, and language ambiguity. |

[Back](#contents)

### Latent Optimization and Sampling

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2025 | Seek in the Dark | arXiv | [Paper](https://arxiv.org/abs/2505.13308) | [📦](https://github.com/bigai-nlco/LatentSeek) | `method`, `hidden-state`, `parallel`, `posterior`, `language` | Instance-level policy gradients search latent space at inference time. |
| 2025 | LatentEvolve | arXiv | [Paper](https://arxiv.org/abs/2509.24771) | [📦](https://github.com/jins7/LatentEvolve) | `method`, `hidden-state`, `parallel`, `free-form`, `language` | Test-time latent self-evolution for reasoning refinement. |
| 2025 | Thinking on the Fly | ICLR 2026 | [Paper](https://openreview.net/forum?id=r1WEQzkCQv) | [📦](https://github.com/ltpo2025/LTPO) | `method`, `hidden-state`, `parallel`, `posterior`, `language` | Policy optimization over latent thoughts at inference time. |
| 2024 | Language Models are Hidden Reasoners | arXiv | [Paper](https://arxiv.org/abs/2411.04282) | — | `method`, `hidden-state`, `parallel`, `posterior`, `language` | Treats reasoning as latent posterior optimization at test time. |
| 2026 | Parallel Test-Time Scaling for Latent Reasoning Models | ACL 2026 | [Paper](https://arxiv.org/abs/2510.07745) | [📦](https://github.com/YRYangang/LatentTTS) | `method`, `hidden-state`, `parallel`, `free-form`, `language` | Parallel sampling and aggregation for latent reasoning at inference time. |
| 2025 | Latent Thinking Optimization: Your Latent Reasoning Language Model Secretly Encodes Reward Signals in Its Latent Thoughts | arXiv | [Paper](https://arxiv.org/abs/2509.26314) | — | `method`, `hidden-state`, `parallel`, `free-form`, `language` | Optimizes latent thinking trajectories at test time using a latent-space classifier. |
| 2024 | Quiet-STaR: Language Models Can Teach Themselves to Think Before Speaking | COLM 2024 | [Paper](https://openreview.net/forum?id=oRXPiSOGH9) | [📦](https://github.com/ezelikman/quiet-star) | `method`, `hidden-state`, `parallel`, `free-form`, `language` | Samples internal rationales for each token and reinforces thoughts that improve future-token prediction. |
| 2026 | Thoughts-as-Planning: Latent World Models for Chain-of-Thoughts Optimization via Reinforcement Planning | arXiv | [Paper](https://arxiv.org/abs/2605.28842) | - | `method`, `hidden-state`, `parallel`, `planning`, `language` | Formulates CoT optimization as sequence planning over a latent world model trained with reinforcement learning. |

[Back](#contents)

## Modality-Grounded Latent

### Visual Latent Workspace

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2025 | Machine Mental Imagery | arXiv | [Paper](https://arxiv.org/abs/2506.17218) | [📦](https://github.com/UMass-Embodied-AGI/Mirage) | `method`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Latent visual tokens serve as internal mental imagery for reasoning. |
| 2025 | Latent Visual Reasoning | arXiv | [Paper](https://arxiv.org/abs/2509.24251) | [📦](https://github.com/bangzhengli/LVR) | `method`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Generates reconstructible visual tokens as latent reasoning workspace. |
| 2025 | Reasoning in the Dark | arXiv | [Paper](https://arxiv.org/abs/2510.12603) | [📦](https://github.com/FYYDCC/IVT-LR) | `method`, `modality-latent`, `autoregressive`, `free-form`, `vision-language` | Each step carries coupled latent text and latent vision for efficient multimodal thinking. |
| 2025 | Latent Sketchpad | arXiv | [Paper](https://arxiv.org/abs/2510.24514) | [📦](https://github.com/Huanyu-Zhang/LatentSketchpad) | `method`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Internal visual sketches act as a latent workspace for reasoning. |
| 2025 | Chain-of-Visual-Thought | arXiv | [Paper](https://arxiv.org/abs/2511.19418) | [📦](https://github.com/ymqian151/Chain-of-Visual-Thought) | `method`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Continuous visual tokens carry intermediate multimodal reasoning. |
| 2025 | Monet | CVPR 2026 | [Paper](https://arxiv.org/abs/2511.21395) | [📦](https://github.com/NOVAglow646/Monet) | `method`, `modality-latent`, `autoregressive`, `posterior`, `vision-language` | Reasons directly in latent visual space with VLPO. |
| 2026 | Render-of-Thought | ACL 2026 | [Paper](https://openreview.net/forum?id=8uPWvXS9sG) | [📦](https://github.com/TencentBAC/RoT) | `method`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Renders text CoT into images to enter visual latent reasoning space. |
| 2026 | ImgCoT | arXiv | [Paper](https://arxiv.org/abs/2601.22730) | — | `method`, `modality-latent`, `autoregressive`, `compression`, `vision-language` | Compresses long CoT into compact visual tokens. |
| 2026 | OneLatent | arXiv | [Paper](https://arxiv.org/abs/2602.13738) | — | `method`, `modality-latent`, `autoregressive`, `compression`, `vision-language` | Single-token visual latent compression for efficient multimodal reasoning. |
| 2025 | Multimodal Chain of Continuous Thought for Latent-Space Reasoning in Vision-Language Models | arXiv | [Paper](https://arxiv.org/abs/2508.12587) | — | `method`, `modality-latent`, `autoregressive`, `free-form`, `vision-language` | Continuous vision-language thought chain in latent space. |
| 2025 | VL-JEPA | arXiv | [Paper](https://arxiv.org/abs/2512.10942) | — | `method`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Predicts continuous text embeddings instead of discrete tokens for efficient VL reasoning. |
| 2025 | Efficient Reasoning with Hidden Thinking | ICML 2026 | [Paper](https://arxiv.org/abs/2501.19201) | [📦](https://github.com/shawnricecake/Heima) | `method`, `modality-latent`, `autoregressive`, `compression`, `vision-language` | Compresses CoT into thinking tokens with encode-decode reconstruction in MLLMs. |
| 2025 | SSR: Enhancing Depth Perception in Vision-Language Models via Rationale-Guided Spatial Reasoning | NeurIPS 2025 | [Paper](https://openreview.net/forum?id=SOc0tHCewe) | [📦](https://yliu-cs.github.io/SSR/) | `method`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Distills spatial rationales into compact latent embeddings for efficient VLM reasoning. |
| 2025 | Sketch-in-Latents: Eliciting Unified Reasoning in MLLMs (SkiLa) | arXiv | [Paper](https://arxiv.org/abs/2512.16584) | — | `method`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Alternates text thoughts and latent sketch tokens with semantic reconstruction. |
| 2026 | DeepLatent: Think with Images via Parallel Latent Visual Reasoning | arXiv | [Paper](https://arxiv.org/abs/2606.00562) | - | `method`, `modality-latent`, `parallel`, `reconstruction`, `vision-language` | Uses parallel latent visual reasoning to avoid autoregressive bottlenecks in image-based reasoning. |
| 2026 | Self-Consistent Latent Reasoning: Long Latent Sequence Reasoning for Vision-Language Model | arXiv | [Paper](https://arxiv.org/abs/2605.12163) | - | `method`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Addresses degradation in long visual latent reasoning sequences with self-consistency constraints. |
| 2026 | UniVLR: Unifying Text and Vision in Visual Latent Reasoning for Multimodal LLMs | arXiv | [Paper](https://arxiv.org/abs/2605.11856) | - | `method`, `modality-latent`, `autoregressive`, `compression`, `vision-language` | Unifies textual reasoning and visual evidence inside a shared visual latent workspace. |

[Back](#contents)

### Spatio-Temporal Representation

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2025 | CoCoVa | arXiv | [Paper](https://arxiv.org/abs/2511.02360) | — | `method`, `modality-latent`, `depth-recurrence`, `reconstruction`, `vision-language` | Latent Q-Former iteratively fuses vision and text for efficient spatio-temporal reasoning. |
| 2024 | Video Representation Learning with Joint-Embedding Predictive Architectures | arXiv | [Paper](https://arxiv.org/abs/2412.10925) | — | `method`, `modality-latent`, `depth-recurrence`, `reconstruction`, `video-language` | JEPA latent targets encode video dynamics for efficient predictive reasoning. |
| 2025 | V-JEPA 2 | arXiv | [Paper](https://arxiv.org/abs/2506.09985) | [📦](https://github.com/facebookresearch/jepa) | `method`, `modality-latent`, `depth-recurrence`, `planning`, `video-language` | Video world model with latent predictive representations for planning-efficient reasoning. |
| 2025 | Think with 3D: Geometric Imagination Grounded Spatial Reasoning from Limited Views | CVPR 2026 | [Paper](https://arxiv.org/abs/2510.18632) | — | `method`, `modality-latent`, `depth-recurrence`, `reconstruction`, `vision-language` | Online 3D geometric latent imagination for spatial reasoning from limited views. |
| 2026 | 3DThinkVLA: Endowing Vision-Language-Action Models with Latent 3D Priors via 3D-Thinking-Guided Co-training | arXiv | [Paper](https://arxiv.org/abs/2606.04436) | - | `method`, `modality-latent`, `depth-recurrence`, `reconstruction`, `omnimodal` | Injects latent 3D priors into VLA models through 3D-thinking-guided co-training for spatial reasoning. |

[Back](#contents)

### World and Action Imagination

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2025 | Latent Chain-of-Thought for Visual Reasoning | NeurIPS 2025 | [Paper](https://openreview.net/forum?id=0i8ClSr3kQ) | [📦](https://github.com/heliossun/LaCoT) | `method`, `modality-latent`, `parallel`, `posterior`, `vision-language` | Posterior inference learns visual latent rationales without long explicit CoT. |
| 2026 | ReGuLaR | arXiv | [Paper](https://arxiv.org/abs/2601.23184) | [📦](https://github.com/FanmengWang/ReGuLaR) | `method`, `modality-latent`, `parallel`, `posterior`, `vision-language` | Variational latent reasoning with rendered-CoT supervision. |
| 2018 | Learning Latent Dynamics for Planning from Pixels | ICML 2019 | [Paper](https://proceedings.mlr.press/v97/hafner19a.html) | - | `method`, `modality-latent`, `parallel`, `planning`, `omnimodal` | Learns latent dynamics from pixels and performs model-based planning in the learned state space. |
| 2019 | Dream to Control | ICLR 2020 | [Paper](https://openreview.net/forum?id=S1lOTC4tDS) | [📦](https://github.com/google-research/dreamer) | `method`, `modality-latent`, `parallel`, `planning`, `omnimodal` | Optimizes policies inside latent imagination for sample-efficient control reasoning. |
| 2024 | Latent Action Pretraining from Videos | ICLR 2025 | [Paper](https://openreview.net/forum?id=VYOe2eBQeh) | [📦](https://github.com/LatentActionPretraining/LAPA) | `method`, `modality-latent`, `memory-state`, `reconstruction`, `omnimodal` | Latent action tokens as compact intermediate states for embodied reasoning. |
| 2025 | villa-X | arXiv | [Paper](https://arxiv.org/abs/2507.23682) | — | `method`, `modality-latent`, `autoregressive`, `planning`, `omnimodal` | Unifies vision-language-latent-action planning for efficient embodied reasoning. |
| 2026 | CLAP | arXiv | [Paper](https://arxiv.org/abs/2601.04061) | — | `method`, `modality-latent`, `autoregressive`, `reconstruction`, `omnimodal` | Contrastive latent actions align video and robot actions for efficient embodied reasoning. |
| 2025 | Latent Action Pretraining Through World Modeling | arXiv | [Paper](https://arxiv.org/abs/2509.18428) | — | `method`, `modality-latent`, `memory-state`, `reconstruction`, `omnimodal` | World-model constraints learn efficient latent action representations. |
| 2026 | Thinking with Images as Continuous Actions | arXiv | [Paper](https://arxiv.org/abs/2602.23959) | — | `method`, `modality-latent`, `autoregressive`, `planning`, `vision-language` | Continuous coordinate actions serve as visual intermediate reasoning states. |
| 2025 | Latent Chain-of-Thought World Modeling for End-to-End Autonomous Driving (LCDrive) | CVPR 2026 | [Paper](https://arxiv.org/abs/2512.10226) | — | `method`, `modality-latent`, `autoregressive`, `planning`, `omnimodal` | Interleaves action proposals and latent world-model tokens for efficient driving rollout. |
| 2026 | Latent Reasoning VLA: Latent Thinking and Prediction for Vision-Language-Action Models | ICML 2026 | [Paper](https://arxiv.org/abs/2602.01166) | — | `method`, `modality-latent`, `autoregressive`, `planning`, `omnimodal` | Curriculum from explicit multimodal CoT to continuous latent reasoning for VLA. |
| 2026 | LaST0: Latent Spatio-Temporal Chain-of-Thought for Robotic Vision-Language-Action Model | arXiv | [Paper](https://arxiv.org/abs/2601.05248) | — | `method`, `modality-latent`, `autoregressive`, `planning`, `omnimodal` | Latent spatio-temporal CoT trajectories for efficient robotic planning. |
| 2026 | Boosting World Models Learning via Latent-Space Value Alignment | ICML 2026 | [Paper](https://icml.cc/virtual/2026/papers.html?filter=titles) | - | `method`, `modality-latent`, `memory-state`, `planning`, `omnimodal` | Aligns world-model latent states with value estimates, strengthening latent dynamics for planning and control. |
| 2026 | DeepSight: Long-Horizon World Modeling via Latent States Prediction for End-to-End Autonomous Driving | arXiv | [Paper](https://arxiv.org/abs/2605.10564) | - | `method`, `modality-latent`, `parallel`, `planning`, `omnimodal` | Predicts future BEV latent semantic states for long-horizon autonomous-driving world modeling. |
| 2026 | Latent State Design for World Models under Sufficiency Constraints | arXiv | [Paper](https://arxiv.org/abs/2605.01694) | - | `theory`, `modality-latent`, `memory-state`, `planning`, `omnimodal` | Formalizes sufficient latent-state design for world models across prediction, control, planning, and memory. |
| 2026 | Latent Action Control for Reasoning-Guided Unified Image Generation | arXiv | [Paper](https://arxiv.org/abs/2605.16961) | - | `method`, `modality-latent`, `autoregressive`, `planning`, `vision-language` | Injects reasoning as continuous latent actions to guide unified image generation. |

[Back](#contents)

## Interpretability

### Probe and Decoding

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | Do Latent-CoT Models Think Step-by-Step A Mechanistic Study on Sequential Reasoning Tasks | arXiv | [Paper](https://arxiv.org/abs/2602.00449) | [📦](https://github.com/jialiang19/latent-cot-thinking) | `analysis`, `hidden-state`, `autoregressive`, `compression`, `language` | Probes whether CODI truly encodes and uses sequential intermediate states. |
| 2024 | Do LLMs Really Think Step-by-step In Implicit Reasoning? | arXiv | [Paper](https://arxiv.org/abs/2411.15862) | [📦](https://github.com/yuyijiong/if_step_by_step_implicit_CoT) | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Linear probes reveal trained implicit CoT encodes steps; prompted implicit CoT does not. |
| 2025 | Uncovering Latent Chain of Thought Vectors in Large Language Models | ICLR 2025 Workshop | [Paper](https://iclr.cc/virtual/2025/33087) | — | `analysis`, `hidden-state`, `autoregressive`, `free-form`, `language` | Decodes latent CoT vectors to test what implicit states encode. |
| 2025 | Think-to-Talk or Talk-to-Think? When LLMs Come Up with an Answer in Multi-Step Arithmetic | arXiv | [Paper](https://arxiv.org/abs/2412.01113) | — | `analysis`, `hidden-state`, `autoregressive`, `free-form`, `language` | Probes when implicit arithmetic reasoning happens relative to answer generation. |
| 2024 | Can Language Models Learn to Skip Steps? | ICLR 2024 | [Paper](https://openreview.net/forum?id=w4AnTVxAO9) | — | `analysis`, `hidden-state`, `autoregressive`, `compression`, `language` | Probes whether models internalize or skip intermediate reasoning steps. |
| 2024 | Do Large Language Models Latently Perform Multi-Hop Reasoning? | ACL 2024 | [Paper](https://doi.org/10.18653/v1/2024.acl-long.550) | — | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Probing evidence for multi-hop reasoning in latent states. |

[Back](#contents)

### Causal and Faithfulness Analysis

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2025 | Do Latent Tokens Think A Causal and Adversarial Analysis of Chain-of-Continuous-Thought | arXiv | [Paper](https://arxiv.org/abs/2512.21711) | — | `analysis`, `hidden-state`, `parallel`, `free-form`, `language` | Causal/adversarial study finds latent tokens can act as placeholders with shortcut risk. |
| 2026 | Dynamics Within Latent Chain-of-Thought An Empirical Study of Causal Structure | ICML 2026 | [Paper](https://proceedings.mlr.press/v306/li26a.html) | [📦](https://github.com/J1mL1/causal-latent-cot) | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Step-wise causal interventions on Coconut and CODI reveal cross-step latent structure. |
| 2024 | Understanding and Patching Compositional Reasoning in LLMs | ACL 2024 Findings | [Paper](https://aclanthology.org/2024.findings-acl.576/) | - | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Analyzes and patches internal mechanisms involved in compositional reasoning. |
| 2026 | Unlocking the Black Box of Latent Reasoning: An Interpretability-Guided Approach to Intervention | arXiv | [Paper](https://arxiv.org/abs/2606.01243) | - | `analysis`, `hidden-state`, `autoregressive`, `free-form`, `language` | Uses interpretability-guided interventions to analyze and steer continuous thought vectors. |
| 2026 | Beyond Visual Memory: Mechanistic Diagnostics of Latent Visual Reasoning | arXiv | [Paper](https://arxiv.org/abs/2606.01287) | - | `analysis`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Diagnoses causal structure and information flow in latent visual reasoning mechanisms. |

[Back](#contents)

### Circuit Dynamics

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2023 | Towards a Mechanistic Interpretation of Multi-Step Reasoning Capabilities of Language Models | EMNLP 2023 | [Paper](https://aclanthology.org/2023.emnlp-main.299/) | - | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Uses mechanistic probes to recover reasoning-tree structure from attention patterns. |
| 2025 | How Do LLMs Perform Two-Hop Reasoning in Context? | arXiv | [Paper](https://arxiv.org/abs/2502.13913) | - | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Analyzes two-hop reasoning information flow, including early entity bridging and later integration. |
| 2024 | Iteration Head: A Mechanistic Study of Chain-of-Thought | arXiv | [Paper](https://arxiv.org/abs/2406.02128) | - | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Identifies attention heads that write intermediate reasoning states back into token space for iterative reasoning. |
| 2025 | Back Attention: Understanding and Enhancing Multi-Hop Reasoning in Large Language Models | arXiv | [Paper](https://arxiv.org/abs/2502.10835) | - | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Uses logit-flow and backward-attention analysis to trace and enhance multi-hop reasoning. |
| 2024 | Distributional Reasoning in LLMs: Parallel Reasoning Processes in Multi-Hop Reasoning | arXiv | [Paper](https://arxiv.org/abs/2406.13858) | - | `analysis`, `hidden-state`, `parallel`, `free-form`, `language` | Studies parallel reasoning processes and distributional logit paths in multi-hop reasoning. |
| 2024 | A Mechanistic Analysis of a Transformer Trained on a Symbolic Multi-Step Reasoning Task | ACL 2024 Findings | [Paper](https://doi.org/10.18653/v1/2024.findings-acl.242) | - | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Mechanistically analyzes how a transformer solves a symbolic multi-step reasoning task. |
| 2025 | Internal Chain-of-Thought: Empirical Evidence for Layer-Wise Subtask Scheduling in LLMs | EMNLP 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.1147/) | - | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Provides evidence that LLM layers schedule intermediate subtasks as an internal Chain-of-Thought. |
| 2025 | On the Biology of a Large Language Model | Technical Report | [Paper](https://transformer-circuits.pub/2025/attribution-graphs/biology.html) | - | `analysis`, `hidden-state`, `parallel`, `free-form`, `language` | Uses attribution graphs to analyze large-scale internal computation in a production language model. |
| 2024 | Grokked Transformers Are Implicit Reasoners: A Mechanistic Journey to the Edge of Generalization | ICLR 2024 | [Paper](https://openreview.net/forum?id=D4QgSWxiOb) | - | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Shows how grokked transformers develop implicit reasoning mechanisms near the edge of generalization. |

[Back](#contents)

### Behavioral Diagnostics

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | How Do Latent Reasoning Methods Perform Under Weak and Strong Supervision | arXiv | [Paper](https://arxiv.org/abs/2602.22441) | — | `analysis`, `hidden-state`, `autoregressive`, `free-form`, `language` | Behavioral diagnosis of shortcut trade-offs in Coconut/CODI-style methods. |
| 2026 | LLMs Are Single-Threaded Reasoners Demystifying the Working Mechanism of Soft Thinking | ICLR 2026 | [Paper](https://openreview.net/forum?id=ASLuOoP78o) | — | `analysis`, `soft-readout`, `autoregressive`, `free-form`, `language` | Shows soft thinking behaves as greedy single-threaded reasoning despite parallel design. |
| 2025 | Implicit Reasoning in Transformers Is Reasoning through Shortcuts | ACL 2025 Findings | [Paper](https://aclanthology.org/2025.findings-acl.493/) | — | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Diagnoses shortcut behavior in implicit transformer reasoning rather than faithful stepwise computation. |
| 2025 | Do Language Models Use Their Depth Efficiently? | ICML 2025 | [Paper](https://proceedings.mlr.press/v267/csordas25a.html) | — | `analysis`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Diagnoses inefficient depth usage relevant to latent depth-based reasoning. |
| 2026 | Large Reasoning Models Are (Not Yet) Multilingual Latent Reasoners | ACL 2026 Findings | [Paper](https://arxiv.org/abs/2601.02996) | [📦](https://github.com/cisnlp/multilingual-latent-reasoner) | `analysis`, `hidden-state`, `autoregressive`, `free-form`, `language` | Diagnoses uneven multilingual behavior in latent reasoning pathways. |
| 2026 | What's Holding Back Latent Visual Reasoning? | arXiv | [Paper](https://arxiv.org/abs/2605.18445) | - | `analysis`, `modality-latent`, `autoregressive`, `reconstruction`, `vision-language` | Uses ablations to show that some latent visual tokens have limited causal effect on final accuracy. |
| 2026 | Ablate-to-Validate: Are Vision-Language Models Really Using Continuous Thought Tokens? | arXiv | [Paper](https://arxiv.org/abs/2605.21642) | - | `analysis`, `modality-latent`, `autoregressive`, `free-form`, `vision-language` | Introduces an ablation framework for testing whether VLMs actually use continuous thought tokens. |

[Back](#contents)

### Theoretical Analysis

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | The Theoretical Benefits and Limitations of Latent Chain-of-Thought Reasoning | ICLR 2026 | [Paper](https://openreview.net/forum?id=q7Nhu2Fw11) | — | `theory`, `soft-readout`, `parallel`, `free-form`, `language` | Theory unifying exploration benefits and fidelity limits of latent CoT. |
| 2026 | Capabilities and Fundamental Limits of Latent Chain-of-Thought | arXiv | [Paper](https://arxiv.org/abs/2602.01148) | — | `theory`, `soft-readout`, `parallel`, `free-form`, `language` | Formal limits of latent CoT on exploratory versus computational tasks. |
| 2025 | Reasoning by Superposition A Theoretical Perspective on Chain of Continuous Thought | NeurIPS 2025 | [Paper](https://proceedings.neurips.cc/paper_files/paper/2025/file/72c363c2a573ca2128bd176d3317696b-Paper-Conference.pdf) | — | `theory`, `soft-readout`, `parallel`, `free-form`, `language` | Theoretical account of parallel exploration via superposition in continuous CoT. |
| 2026 | Emergence of Superposition Unveiling the Training Dynamics of Chain of Continuous Thought | ICLR 2026 | [Paper](https://openreview.net/forum?id=lsJwX9Jf5u) | — | `theory`, `soft-readout`, `parallel`, `free-form`, `language` | Training dynamics explain superposition in continuous implicit CoT. |
| 2025 | A Formal Comparison Between Chain of Thought and Latent Thought | ICML 2026 | [Paper](https://arxiv.org/abs/2509.25239) | [📦](https://github.com/kevin671/cot-vs-loop) | `theory`, `hidden-state`, `parallel`, `free-form`, `language` | Formalizes compute and parallelism differences between explicit and latent thought. |
| 2025 | A Little Depth Goes a Long Way: The Expressive Power of Log-Depth Transformers | ICLR 2025 | [Paper](https://openreview.net/forum?id=7cMzTpbJHC) | — | `theory`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Argues vertical depth bottlenecks explicit CoT steps and motivates latent depth methods. |
| 2026 | Chain-of-Thought and Compressed Looped Transformers: A Memory-Budget Separation | arXiv | [Paper](https://arxiv.org/abs/2605.30757) | - | `theory`, `hidden-state`, `depth-recurrence`, `free-form`, `language` | Compares CoT scratchpads with compressed looped transformers under memory-budget constraints. |

[Back](#contents)

## Benchmarks and Evaluation

A unified evaluation setup for latent thinking should report final-task performance, reasoning economy, causal utility of intermediate states, and grounding quality for multimodal carriers. The survey recommends comparable language tasks such as GSM8K and MATH for language-only SR/NHS methods, community-standard suites for vision, video, audio, and embodied settings, and intervention tests over latent tokens, hidden states, memories, or reconstructed visual traces.

| Focus | Representative Evaluation Direction |
| ----- | ----------------------------------- |
| Language latent reasoning | Accuracy on shared reasoning tasks plus explicit-token count, latent-step count, latency, and intervention sensitivity. |
| Vision-language latent reasoning | Task accuracy plus whether visual latents reconstruct or preserve task-relevant regions. |
| Video and world models | Long-horizon prediction, spatial memory, dynamics preservation, and planning return. |
| Audio and embodied agents | Complex audio reasoning, action success, latent-action alignment, and state-grounded planning quality. |
| Interpretability | Probing, patching, masking, permutation, causal mediation, and behavioral shortcut diagnostics over fixed checkpoints. |

[Back](#contents)

## Related Awesome Lists

- [Awesome Latent Space](https://github.com/YU-deep/Awesome-Latent-Space) - Resources on latent-space foundations, mechanisms, abilities, and outlook.
- [Awesome LLM Implicit Reasoning](https://github.com/digailab/awesome-llm-implicit-reasoning) - Resources on implicit reasoning execution paradigms in language models.
- [LatentCoT-Horizon](https://github.com/multimodal-art-projection/LatentCoT-Horizon) - Resources related to latent reasoning and latent Chain-of-Thought.
- [Awesome Latent CoT](https://github.com/EIT-NLP/Awesome-Latent-CoT) - Resources on latent Chain-of-Thought reasoning beyond language.
- [Awesome Think With Images](https://github.com/zhaochen0110/Awesome_Think_With_Images) - Resources on thinking with images and multimodal reasoning workspaces.
- [Awesome Reasoning](https://github.com/goodbai-nlp/Awesome-Reasoning) - A broader collection of reasoning papers across learning, test-time scaling, efficiency, multimodal, structured, and agentic reasoning.

[Back](#contents)
