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


- [🧩 VLA Architecture & Action Generation](#-vla-architecture--action-generation)
  - [Autoregressive VLA](#Autoregressive VLA)
  - [Diffusion-based VLA](#Diffusion-based VLA)
  - [Video-Action Models (VAMs)](#Video-Action Models (VAMs))
  - [World-Action Models (WAMs)](#World-Action Models (WAMs))


- [⚡ Deployment & Generalization](#-deployment--generalization)
  - [Model Efficiency](#model-efficiency)
  - [Scene Generalization](#scene-generalization)


- [🧠 Capability Expansion](#-capability-expansion)
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


| Year | Paper | Website | Code |
|------|-------|---------|------|
|2023|RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control|🌐|-|
|2024|ECoT: Embodied Chain-of-Thought Reasoning for Robot Manipulation|🌐|-|
|2024|OpenVLA: An Open-Source Vision-Language-Action Model|🌐|💻|
|2025|CoT-VLA: ...|🌐|-|
|2025|ChatVLA: ...|🌐|-|
|2026|AR-VLA: ...|🌐|-|
---

## ⚡ Deployment & Generalization


Large-scale VLAs face challenges in computational efficiency and robust adaptation when deployed in real-world environments.


This section reviews approaches toward practical deployment, including:


- Model efficiency
    - Lightweight architectures
    - Token optimization
    - Quantization
    - Knowledge distillation

- Scene generalization
    - Geometric representation learning
    - Object-centric perception
    - Open-world adaptation

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
