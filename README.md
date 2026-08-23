# 🤖 A Survey of Multi-Paradigm Approaches Toward General-Purpose Embodied Intelligence


### 🌟 A comprehensive review of Vision-Language-Action Models and emerging paradigms for general-purpose embodied intelligence


Vision-Language-Action Models (VLAs) provide a unified framework that connects visual perception, language understanding, and robotic control. 
This repository accompanies our survey, presenting a systematic review of the evolution of embodied intelligence, covering VLA architectures, efficient deployment, scene generalization, capability enhancement, and emerging predictive paradigms including Video-Action Models (VAMs) and World-Action Models (WAMs).


---

# 📰 News


- `2026.08` Repository initialized.
- More updates will be released as the field evolves.


---

# 📌 Overview


This survey analyzes the evolutionary trajectory of general-purpose embodied intelligence from three perspectives:




- **🧩 VLA Architecture & Action Generation**
  - Vision-Language Representation
  - Multimodal Backbone
  - Action Decoding Paradigms


- **⚡ Deployment & Generalization**
  - Model Efficiency
  - Scene Generalization


- **🧠 Capability Expansion**
  - Reinforcement Learning
  - World Models
  - Long-Horizon Reasoning


<img src="assets/overview.png" width="100%">
<p align="center">
Figure 1. Chronological roadmap and key milestones of VLAs and WAM (2022–2026). The ffgure depicts the four-stage evolution of embodied policy
models—progressing from early language-conditioned control, open generalist VLAs, and reasoning-enhanced architectures, to video- and worldaware
 agents leveraging world dynamics.
</p>

---


# 📑 Table of Contents


- [🧩 VLA Architecture & Action Generation](#vla-architecture--action-generation)
  - [Autoregressive VLA](#autoregressive-vla)
  - [Diffusion-based VLA](#diffusion-based-vla)
  - [Video-Action Models (VAMs)](#video-action-models-vams)
  - [World-Action Models (WAMs)](#world-action-models-wams)
  - [Datasets](#Datasets)


- [⚡ Deployment & Generalization](#deployment--generalization)
  - [Model Efficiency](#model-efficiency)
  - [Scene Generalization](#scene-generalization)


- [🧠 Capability Expansion](#capability-expansion)
  - [Reinforcement Learning](#reinforcement-learning)
  - [World Models](#world-models)
  - [Long-Horizon Reasoning](#long-horizon-reasoning)


- [🏭 Applications](#-applications)


- [🔭 Challenges and Future Directions](#-challenges-and-future-directions)


- [📖 Citation](#-citation)


## 🧩 VLA Architecture & Action Generation


VLAs have evolved from action-sequence prediction models toward predictive embodied models that incorporate future dynamics and world-state reasoning.


This section reviews four major paradigms:


- Autoregressive VLA
- Diffusion-based VLA
- Video-Action Models (VAMs)
- World-Action Models (WAMs)
- Datasets


<img src="assets/architecture.png" width="100%">
<p align="center">
Figure 2. Architectural overview of VLAs. Encoding: Heterogeneous inputs are encoded and aligned via cross-modal fusion. Multimodal Reasoning:
Transformer-based VLM/LLM backbones process fused latent features for high-level decision-making. Action Decoding: Latent representations are
mapped into executable robot commands via direct regression, autoregressive prediction, or diffusion/ffow matching.
</p>


### Autoregressive VLA


Autoregressive VLAs generate actions sequentially by predicting future action tokens conditioned on visual observations and language instructions. These methods establish the early paradigm of vision-language-action models by extending large-scale multimodal pretraining to robotic control.


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2023|arXiv|[RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818)|[🌐](https://robotics-transformer2.github.io/)|-|
|2024|arXiv|[Robotic Control via Embodied Chain-of-Thought Reasoning](https://arxiv.org/abs/2407.08693)|[🌐](https://embodied-cot.github.io/)|[💻](https://github.com/MichalZawalski/embodied-CoT/))|
|2025|arXiv|[CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models](https://arxiv.org/abs/2503.22020)|[🌐](https://cot-vla.github.io/)|-|
|2025|arXiv|[ChatVLA: Unified Multimodal Understanding and Robot Control with Vision-Language-Action Model](https://arxiv.org/abs/2502.14420)|[🌐](https://chatvla.github.io/)|[💻](https://github.com/tutujingyugang1/ChatVLA_public)|
|2026|arXiv|[AR-VLA: True Autoregressive Action Expert for Vision-Language-Action Models](https://arxiv.org/abs/2603.10126)|[🌐](https://arvla.insait.ai/)|[💻](https://github.com/insait-institute/AR-VLA-lerobot)|

### Diffusion-based VLA


Diffusion-based VLAs generate continuous action trajectories through iterative denoising processes, enabling smooth and multimodal robot control. These methods combine vision-language understanding with diffusion-based action generation for complex manipulation tasks.

| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[π0: A Vision-Language-Action Flow Model for General Robot Control](https://arxiv.org/abs/2410.24164))|[🌐](https://www.pi.website/blog/pi0)|-|
|2025|arXiv|[SmolVLA: A Vision-Language-Action Model for Affordable and Efficient Robotics]((https://arxiv.org/abs/2506.01844))|-|[💻](https://github.com/huggingface/lerobot)|
|2025|arXiv|[DreamVLA: A Vision-Language-Action Model Dreamed with Comprehensive World Knowledge](https://arxiv.org/abs/2507.04447)|-|[💻](https://github.com/Zhangwenyao1/DreamVLA)|
|2026|arXiv|[CF-VLA: Efficient Coarse-to-Fine Action Generation for Vision-Language-Action Policies]((https://arxiv.org/abs/2604.24622))|-|[💻](https://github.com/EmbodiedAI-RoboTron/CF-VLA)|

### Video-Action Models (VAMs)


Video-Action Models extend VLAs by jointly modeling future video dynamics and action sequences. By learning temporal evolution and interaction dynamics, VAMs provide predictive visual priors to improve embodied decision-making.


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2025|arXiv|[Unified Video Action Model](https://arxiv.org/abs/2503.00200)|[🌐](https://unified-video-action-model.github.io/)|-|
|2025|arXiv|[VideoVLA](paper link)|[🌐](website)|[💻](code)|
|2026|arXiv|[DiT4DiT ](paper link)|[🌐](website)|[💻](https://github.com/ShuangLI59/unified_video_action)|
|2026|arXiv|[S-VAM: Shortcut Video-Action Model by Self-Distilling Geometric and Semantic Foresight](https://arxiv.org/abs/2603.16195)|[🌐](https://haodong-yan.github.io/S-VAM/)|[💻](https://github.com/Haodong-Yan/S-VAM)|

### World-Action Models (WAMs)


World-Action Models extend embodied policies by integrating future world-state prediction with action generation. By learning predictive models of environment dynamics, WAMs enable more informed planning and decision-making for long-horizon robotic tasks.


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2025|arXiv|[Unified World Models: Coupling Video and Action Diffusion for Pretraining on Large Robotic Datasets](https://arxiv.org/abs/2504.02792)|[🌐](https://weirdlabuw.github.io/uwm/)|[💻](https://github.com/WEIRDLabUW/unified-world-model)|
|2026|arXiv|[Fast-WAM: Do World Action Models Need Test-time Future Imagination?](https://arxiv.org/abs/2603.16666)|[🌐](https://yuantianyuan01.github.io/FastWAM/)|[💻](https://github.com/yuantianyuan01/FastWAM)|
|2026|arXiv|[OA-WAM: Object-Addressable World Action Model for Robust Robot Manipulation](https://arxiv.org/abs/2605.06481)|-|-|
|2026|arXiv|[HarmoWAM: Harmonizing Generalizable and Precise Manipulation via Adaptive World Action Models](https://arxiv.org/abs/2605.10942)|[🌐](https://elbb-yu.github.io/HarmoWAM/)|-|

### Datasets


Large-scale embodied datasets provide the foundation for training and evaluating VLAs. This section summarizes representative datasets for robot manipulation, embodied instruction following, and real-world deployment.


| Dataset | Year | Domain | Website | Code |
|---------|------|--------|---------|------|
| [Meta-World](https://arxiv.org/abs/1910.10897) | 2021 | Multi-task robotic manipulation with 50 simulated tasks | [🌐](https://meta-world.github.io/) | [💻](https://github.com/Farama-Foundation/Metaworld) |
| [LIBERO](https://arxiv.org/abs/2306.03310) | 2023 | Lifelong robot learning with diverse language-conditioned manipulation tasks | [🌐](https://libero-project.github.io/intro.html) | -  |
| [LIBERO-Plus](https://arxiv.org/abs/2510.13626) | 2024 | Robust VLA evaluation under environmental perturbations and distribution shifts | [🌐](https://sylvestf.github.io/LIBERO-plus/) |[💻](https://github.com/sylvestf/LIBERO-plus) |
| [RoboTwin 2.0](https://arxiv.org/abs/2506.18088) | 2025 | Bimanual manipulation with diverse object interaction scenarios | [🌐](https://robotwin-platform.github.io/) | [💻](https://github.com/robotwin-Platform/robotwin) |
| [CALVIN](https://arxiv.org/abs/2112.03227) | 2022 | Long-horizon language-conditioned robotic manipulation | [🌐](http://calvin.cs.uni-freiburg.de/) | - |

---

## ⚡ Deployment & Generalization


Large-scale VLAs face challenges in computational efficiency and robust adaptation when deployed in real-world environments.


This section reviews approaches toward practical deployment, including:


- Model efficiency
    - Token optimization
    - Quantization
    - Knowledge distillation

- Scene generalization
    - Geometric representation learning
    - Object-centric perception
    - Open-world generalization

### Model Efficiency
Model efficiency approaches reduce the computational and memory costs of VLAs through parameter reduction, precision optimization, and knowledge transfer.

#### Pruning


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2025|arXiv|[Action-aware Dynamic Pruning for Efficient Vision-Language-Action Manipulation](https://arxiv.org/abs/2509.22093)|[🌐](website)|-|
|2025|arXiv|[SP-VLA: A Joint Model Scheduling and Token Pruning Approach for VLA Model Acceleration](https://arxiv.org/abs/2506.12723)|-|-|
|2026|arXiv|[BFA++: Hierarchical Best-Feature-Aware Token Prune for Multi-View Vision Language Action Model](https://arxiv.org/abs/2602.20566)|-|-|
|2026|arXiv|[ETA-VLA: Efficient Token Adaptation via Temporal Fusion and Intra-LLM Sparsification for Vision-Language-Action Models](https://arxiv.org/abs/2603.25766)|-|-|
|2026|arXiv|[VLA-Pruner: Temporal-Aware Dual-Level Visual Token Pruning for Efficient Vision-Language-Action Inference](https://arxiv.org/html/2511.16449v1)|-|-|

#### Quantization


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[Quantization-Aware Imitation-Learning for Resource-Efficient Robotic Control](https://arxiv.org/abs/2412.01034)|-|-|
|2025|arXiv|[SQAP-VLA: A Synergistic Quantization-Aware Pruning Framework for High-Performance Vision-Language-Action Models](https://arxiv.org/abs/2509.09090)|-|[💻](https://github.com/ecdine/SQAP-VLA)|
|2026|arXiv|[QVLA: Not All Channels Are Equal in Vision-Language-Action Model's Quantization](https://arxiv.org/abs/2602.03782)|-|[💻](https://github.com/AutoLab-SAI-SJTU/QVLA)|
|2026|arXiv|[DyQ-VLA: Temporal-Dynamic-Aware Quantization for Embodied Vision-Language-Action Models](https://arxiv.org/abs/2603.07904)|-|-|
|2026|arXiv|[BitVLA: 1-bit Vision-Language-Action Models for Robotics Manipulation](https://arxiv.org/abs/2506.07530v1)|-|[💻](https://github.com/ustcwhy/BitVLA)|

#### Knowledge Distillation


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2025|arXiv|[DualVLA: Building a Generalizable Embodied Agent via Partial Decoupling of Reasoning and Action](https://arxiv.org/abs/2511.22134)|[🌐](https://costaliya.github.io/DualVLA/)|-|
|2026|arXiv|[ActDistill: General Action-Guided Self-Derived Distillation for Efficient Vision-Language-Action Models](https://arxiv.org/abs/2511.18082)|-|-|
|2026|arXiv|[SnapFlow: One-Step Action Generation for Flow-Matching VLAs via Progressive Self-Distillation](https://arxiv.org/abs/2604.05656)|-|-|
|2026|arXiv|[Shallow-π: Knowledge Distillation for Flow-based VLAs](https://arxiv.org/abs/2601.20262)]|[🌐](https://icsl-jeon.github.io/shallow-pi/)|[💻](https://github.com/icsl-Jeon/openpi)|
|2026|arXiv|[DySL-VLA: Efficient Vision-Language-Action Model Inference via Dynamic-Static Layer-Skipping for Robot Manipulation](https://arxiv.org/abs/2602.22896)|-|[💻](https://github.com/PKU-SEC-Lab/DYSL_VLA)|


### Scene Generalization

VLAs often suffer from performance degradation when deployed in unseen environments due to variations in object configurations, viewpoints, backgrounds, and task conditions.

| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA: Learning to Act Anywhere with Task-centric Latent Actions](https://arxiv.org/abs/2505.06111)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

---

## 🧠 Capability Expansion


To overcome the limitations of imitation learning, recent studies extend VLA capabilities with interactive learning, predictive modeling, and long-horizon decision-making.


This section covers:

- Reinforcement learning
- World models
- Long-horizon reasoning

### Reinforcement Learning


Reinforcement learning enhances VLA capabilities beyond imitation learning by optimizing policies through environment interaction. These approaches improve task performance, adaptation ability, and autonomous decision-making through reward-driven learning.


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

### World Models


World models enhance VLA capabilities by learning predictive representations of environment dynamics. By modeling future states and interactions, these approaches provide additional reasoning signals for planning, decision-making, and policy improvement.


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

### Long-Horizon Reasoning


Long-horizon reasoning enhances VLA capabilities for complex multi-step tasks by introducing hierarchical planning, memory mechanisms, progress monitoring, and failure recovery strategies.


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

---



## 🏭 Applications


Representative applications include:


🏠 Household and Service Robotics

🏥 Healthcare and Surgical Robotics

🚗 Autonomous Driving and Navigation

🏭 Industrial Manipulation

### 🏠 Household and Service Robotics
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

### 🏥 Healthcare and Surgical Robotics
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

### 🚗 Autonomous Driving and Navigation
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

### 🏭 Industrial Manipulation
| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

---

## 🚧 Challenges and Future Directions


Despite rapid progress in Vision-Language-Action models, significant gaps remain before achieving general-purpose embodied intelligence. Current VLAs still face challenges in robustness, deployment, continual adaptation, and autonomous decision-making. This section summarizes the major challenges and future research directions toward reliable embodied agents.


### Challenges


#### 🌍 Open-World Generalization

Current VLAs perform well within training distributions but often struggle with unseen tasks, environments, robot embodiments, and long-tail disturbances. Improving transferable representations and robust adaptation remains a fundamental challenge.


#### ⚡ Lightweight Deployment and Real-Time Control

Large-scale VLAs provide strong semantic understanding but introduce high computational costs and inference latency. Efficient architectures, model compression, and real-time control strategies are required for practical deployment.


#### 🔄 Data Infrastructure and Continual Learning

Existing VLAs mainly rely on static offline datasets and lack effective mechanisms for collecting, filtering, and utilizing deployment experiences, failures, and recovery trajectories.


#### 🌐 Physical Understanding and Predictive Modeling

Current models still lack explicit understanding of physical dynamics, object interactions, and future consequences of actions. Integrating predictive models of the environment is essential for reliable decision-making.


#### 🧠 Long-Horizon Reasoning and Planning

Complex real-world tasks require hierarchical planning, persistent memory, progress monitoring, and failure recovery beyond short-horizon reactive policies.


#### 🤖 System Architecture and Agentic Collaboration

Future embodied systems require effective coordination among perception, reasoning, planning, action execution, memory, and external tools rather than relying on a single end-to-end policy.


#### 📚 Data Acquisition and Synthetic Data Generation

Scaling robot data collection remains expensive and inefficient. More realistic simulation environments, synthetic data generation, and scalable data engines are needed.


---

### Future Directions


#### 🌍 Robust Generalization in Open Environments

Future VLAs should move beyond fixed benchmark performance toward reliable behavior across diverse tasks, scenes, robot platforms, and real-world perturbations.


#### ⚡ Efficient and Deployable Embodied Policies

Future systems may combine large-scale reasoning models with lightweight execution modules, enabling hierarchical architectures where large models plan and smaller models execute.


#### 🔄 Continuous Data Feedback Loops

Future embodied systems should continuously collect interaction data, incorporate failure experiences, and update policies through deployment-driven learning.


#### 🌐 Physics-Aware Predictive Decision Making

Integrating video dynamics and world models can provide future-state prediction and action consequence reasoning, enabling more proactive and reliable control.


#### 🧠 Long-Horizon Autonomous Reasoning

Future VLAs should integrate hierarchical planning, memory, verification, and recovery mechanisms to support complex multi-stage tasks.


#### 🤖 Autonomous Embodied Agents

VLAs are expected to evolve toward agentic systems with reasoning, tool use, self-correction, and coordinated perception-action capabilities.


#### 📚 Scalable Data Engines and Evaluation

Future progress requires large-scale embodied datasets, realistic simulation platforms, and evaluation protocols that better reflect real-world reliability.


---

## 📖 Citation


If you find this survey useful, please consider citing:


```bibtex
@article{shi2026embodied,
  title={A Survey of Multi-Paradigm Approaches Toward General-Purpose Embodied Intelligence:
  Panoramic Overview and Evolutionary Trajectory},
  author={Shi, Ruyu and others},
  journal={IEEE Transactions on Robotics},
  year={2026}
}
