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
|2024|arXiv|ECoT: Chain-of-Thought Reasoning for Vision-Language-Action Models|🌐|-|
|2025|arXiv|CoT-VLA: Chain-of-Thought Reasoning for Vision-Language-Action Models|🌐|-|
|2025|arXiv|ChatVLA: Unified Multimodal Understanding and Robot Control|🌐|-|
|2026|arXiv|AR-VLA|🌐|-|

### Diffusion-based VLA


Diffusion-based VLAs generate continuous action trajectories through iterative denoising processes, enabling smooth and multimodal robot control. These methods combine vision-language understanding with diffusion-based action generation for complex manipulation tasks.

| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[π0: A Vision-Language-Action Flow Model for General Robot Control](paper link)|[🌐](website)|-|
|2025|arXiv|[SmolVLA: A Small Vision-Language-Action Model](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[DreamVLA: ...](paper link)|[🌐](website)|-|
|2026|arXiv|[CF-VLA: ...](paper link)|[🌐](website)|-|

### Video-Action Models (VAMs)


Video-Action Models extend VLAs by jointly modeling future video dynamics and action sequences. By learning temporal evolution and interaction dynamics, VAMs provide predictive visual priors to improve embodied decision-making.


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2025|arXiv|[UVA](paper link)|[🌐](website)|-|
|2025|arXiv|[VideoVLA](paper link)|[🌐](website)|[💻](code)|
|2026|arXiv|[DiT4DiT ](paper link)|[🌐](website)|-|
|2026|arXiv|[S-VAM](paper link)|[🌐](website)|-|

### World-Action Models (WAMs)


World-Action Models extend embodied policies by integrating future world-state prediction with action generation. By learning predictive models of environment dynamics, WAMs enable more informed planning and decision-making for long-horizon robotic tasks.


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2025|arXiv|[UWM](paper link)|[🌐](website)|-|
|2026|arXiv|[Fast-WAM](paper link)|[🌐](website)|[💻](code)|
|2026|arXiv|[OA-WAM](paper link)|[🌐](website)|-|
|2026|arXiv|[Latent-WAM](paper link)|[🌐](website)|-|

### Datasets


Large-scale embodied datasets provide the foundation for training and evaluating VLAs. This section summarizes representative datasets for robot manipulation, embodied instruction following, and real-world deployment.


| Dataset | Year | Domain | Website |
|---------|------|--------|---------|
| Meta-World | 2021 | Basic Manipulation Benchmark | Multi-task robotic manipulation with 50 simulated tasks | [🌐](https://meta-world.github.io/) |
| LIBERO | 2023 | Language-Conditioned Manipulation Benchmark | Lifelong robot learning with diverse language-conditioned manipulation tasks | [🌐](https://libero-project.github.io/) |
| LIBERO-Plus | 2024 | Language-Conditioned Manipulation Benchmark | Robust VLA evaluation under environmental perturbations and distribution shifts | [🌐](https://libero-plus.github.io/) |
| RoboTwin 2.0 | 2024 | Generalist Embodied Evaluation Benchmark | Bimanual manipulation with diverse object interaction scenarios | [🌐](https://robotwin-platform.github.io/) |
| CALVIN | 2022 | Language-Conditioned Manipulation Benchmark | Long-horizon language-conditioned robotic manipulation | [🌐](https://github.com/mees/calvin) |

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
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

#### Quantization


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

#### Knowledge Distillation


| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|


### Scene Generalization

VLAs often suffer from performance degradation when deployed in unseen environments due to variations in object configurations, viewpoints, backgrounds, and task conditions.

| Year | Venue | Paper | Website | Code |
|------|-------|-------|---------|------|
|2024|arXiv|[OpenVLA](paper link)|[🌐](website)|-|
|2025|arXiv|[WorldVLA](paper link)|[🌐](website)|[💻](code)|
|2025|arXiv|[UniVLA](paper link)|[🌐](website)|-|
|2026|arXiv|[VLA-JEPA](paper link)|[🌐](website)|-|
|2026|arXiv|[StarVLA-α](paper link)|[🌐](website)|-|

---

## 🧠 Capability Expansion


To overcome the limitations of imitation learning, recent studies extend VLA capabilities with interactive learning, predictive modeling, and long-horizon decision-making.


This section covers:

- Reinforcement learning
- World models
- Long-horizon reasoning


---



# 🏭 Applications


Representative applications include:


🏠 Household and Service Robotics

🏥 Healthcare and Surgical Robotics

🚗 Autonomous Driving and Navigation

🏭 Industrial Manipulation


---

# 🔭 Challenges and Future Directions


Current embodied intelligence systems still face challenges in:


- Robust open-world generalization
- Efficient real-time deployment
- Long-horizon autonomous execution
- Data feedback and continual learning
- System-level integration


---

# 📖 Citation


If you find this survey useful, please consider citing:


```bibtex
@article{shi2026embodied,
  title={A Survey of Multi-Paradigm Approaches Toward General-Purpose Embodied Intelligence:
  Panoramic Overview and Evolutionary Trajectory},
  author={Shi, Ruyu and others},
  journal={IEEE Transactions on Robotics},
  year={2026}
}
