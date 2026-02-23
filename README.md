<div align="center">

```
 ██████╗██╗      ██████╗ ██╗  ██╗ █████╗ ██╗
██╔════╝██║     ██╔═══██╗██║ ██╔╝██╔══██╗██║
██║     ██║     ██║   ██║█████╔╝ ███████║██║
██║     ██║     ██║   ██║██╔═██╗ ██╔══██║██║
╚██████╗███████╗╚██████╔╝██║  ██╗██║  ██║██║
 ╚═════╝╚══════╝ ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝
```
[![Status](https://img.shields.io/badge/Status-Pre--Release%20Alpha-red?style=for-the-badge&logo=rocket)](https://github.com)
[![Architecture](https://img.shields.io/badge/Architecture-ClokArch%20System-blueviolet?style=for-the-badge&logo=buffer)](https://github.com)
[![Parameters](https://img.shields.io/badge/Parameters-~1.5B--1.8B-blue?style=for-the-badge&logo=brain)](https://github.com)
[![Training](https://img.shields.io/badge/Training-2×%20NVIDIA%20T4%20DDP-76b900?style=for-the-badge&logo=nvidia)](https://github.com)
[![Precision](https://img.shields.io/badge/Precision-FP16-orange?style=for-the-badge)](https://github.com)

> *"Not just a language model. A logic engine that thinks in circuits."*

</div>

---

## ⚡ Overview

**CLOKAI** is an experimental heavyweight language model (~1.5B–1.8B parameters), purpose-engineered for the frontier of **Electronic Design Automation (EDA)** and **PCB Logic Synthesis**. Where conventional LLMs predict tokens, CLOKAI extracts logic — combining the raw expressivity of Neuromorphic Computing with the mathematical precision of Non-linear Function Approximation.

This is not a fine-tuned chatbot. This is a *ClokArch** — a domain-native intelligence forged at the intersection of three revolutionary neural paradigms, designed to make PCB design as intuitive as a conversation.

---

## 🧠 Model Architecture — *ClokArch*

CLOKAI is a **ClokArch**: a three-architecture fusion that transcends the limitations of standard transformer-based LLMs.

```
┌─────────────────────────────────────────────────────────┐
│                 CLOKAI ClokArch-ENGINE                  │
│                                                         │
│   ┌───────────────────────────────────────────────┐     │
│   │  [1] KAN-Integrated Backbone                  │     │
│   │      Kolmogorov-Arnold Networks               │     │
│   │      Learnable Spline Activations             │     │
│   └───────────────────────────────────────────────┘     │
│                         ↓                               │
│   ┌───────────────────────────────────────────────┐     │
│   │  [2] Temporal Spiking Attention (TASA)        │     │
│   │      SNN Layers + Async Firing Emulation      │     │
│   │      Clock-Domain Temporal Processing         │     │
│   └───────────────────────────────────────────────┘     │
│                         ↓                               │
│   ┌───────────────────────────────────────────────┐     │
│   │  [3] Neuro-Symbolic Logic Verifier            │     │
│   │      KCL / KVL / Ohm's Law Validation         │     │
│   │      Latent-Space Constraint Enforcement      │     │
│   └───────────────────────────────────────────────┘     │
└─────────────────────────────────────────────────────────┘
```

### 1. KAN-Integrated Backbone *(Kolmogorov-Arnold Networks)*

Standard Multi-Layer Perceptrons have been **surgically replaced** with KAN layers — networks built on learnable activation functions defined by B-splines. Instead of fixed activation curves, every neuron in CLOKAI's backbone adapts its own mathematical function during training.

> **Expert Insight:** This grants CLOKAI the ability to **mathematically resolve** hardware logic and parametric circuit constraints — not merely predict text patterns associated with them. The model doesn't guess component values; it derives them.

### 2. Temporal Spiking Attention — *TASA*

Integrated Spiking Neural Network (SNN) layers emulate the brain's asynchronous firing mechanism at the attention level. The **Time-Aware Spiking Attention (TASA)** mechanism processes information in discrete temporal pulses rather than continuous dense activations.

> **Expert Insight:** TASA enables CLOKAI to process **high-frequency signal integrity** and **clock-domain logic** with genuine temporal accuracy — critical for designs where timing is not a suggestion but a constraint.

### 3. Neuro-Symbolic Logic Verifier

Embedded within CLOKAI's latent space is a **Symbolic Verifier** — a rule-enforcement layer that intercepts generated outputs and validates them against the immutable laws of electronics: Ohm's Law, Kirchhoff's Current Law (KCL), and Kirchhoff's Voltage Law (KVL).

> **Expert Insight:** This creates a **self-correcting synthesis loop**. CLOKAI doesn't just generate netlists — it generates netlists that *pass physical law verification* before they ever leave the model.

---

## 🛠️ Key Capabilities

| Capability | Description |
|---|---|
| 🔌 **Autonomous Netlist Synthesis** | Translate natural language requirements into Altium/KiCad-compatible JSON netlists — zero manual schematic entry |
| 🎯 **Component Optimization** | Infer optimal resistor, capacitor, and inductor values from hidden design constraints and circuit context |
| 🌐 **Hinglish Technical Reasoning** | Native-level comprehension and explanation of complex electronics engineering in **English Only** |
| 🔍 **Hardware Debugging** | Detect design-rule violations, potential short circuits, and logic conflicts through pure **Logical Inference** — no simulation required |

---

## 📊 Technical Specifications

| Parameter | Specification |
|---|---|
| **Parameter Count** | ~1.5 Billion – 1.8 Billion |
| **Architecture** | ClokArch |
| **Hidden Dimension** | 1024 |
| **Depth** | 16 Layers |
| **Training Precision** | FP16 with Gradient Checkpointing |
| **Tokenization** | Domain-Specific BPE (VCC, GND, GPIO, PWM, I²C, SPI optimized) |
| **Training Hardware** | 2× NVIDIA T4 GPUs (Distributed Data Parallel) |

---

## 🚀 Training & Optimization — *The Founder's Secret*

CLOKAI was trained under a bespoke optimization regime on **2× NVIDIA T4 GPUs** in **Distributed Data Parallel (DDP)** mode. Every training decision was made to maximize logic extraction over pattern memorization.

### Entropy Maximization
The data loader employs **high-entropy shuffling** and deliberate **hardware-netlist variability injection**. The training distribution was engineered to be maximally non-repetitive, forcing the model to generalize circuit logic rather than overfit to specific design signatures.

### Warm Restart Schedule
A **Cosine Annealing with Warm Restarts** (SGDR) learning rate schedule was used to aggressively break loss plateaus. Each restart resets the learning rate to escape local minima, progressively narrowing the exploration radius.

### Memory Architecture
Training a ~1.7B parameter ClokArch architecture on constrained VRAM required surgical memory management:
- **Activation Checkpointing** — recompute forward activations during backprop instead of storing them
- **Bucketed Gradient Views** — DDP gradient communication bucketed for optimal bandwidth utilization
- **FP16 Mixed Precision** — half-precision forward passes with FP32 master weights for numerical stability

```
Memory Optimization Stack:
┌──────────────────────────────────────────┐
│  FP16 Mixed Precision (Forward Pass)     │
│  Activation Checkpointing (Backward)     │
│  Bucketed Gradient Sync (DDP Layer)      │
│  Dynamic Loss Scaling (Stability)        │
└──────────────────────────────────────────┘
         ↓ Result: ~1.7B params on 2× T4
```

---

## 🛡️ Pre-Release Status

```
╔══════════════════════════════════════════════════╗
║           ⚠  PRE-RELEASE ALPHA  ⚠               ║
║                                                  ║
║  CLOKAI is currently in active development.      ║
║  Outputs should be verified before production    ║
║  hardware deployment.                            ║
╚══════════════════════════════════════════════════╝
```

CLOKAI is in **Pre-Release Alpha**. The architecture is stable; the mission is not yet complete. Current development priorities include expanding the training corpus, refining the Neuro-Symbolic Verifier's constraint ruleset, and optimizing inference latency for real-time PCB design workflows.

The ultimate objective: **redefine AI's role in the EDA industry** — making PCB design as natural and accessible as talking to a colleague.

---

## 🔭 Roadmap

- [ ] Expand domain-specific tokenizer vocabulary (VHDL, Verilog, SPICE)
- [ ] Release quantized variants for edge deployment
- [ ] Public benchmark suite against baseline EDA-LLMs
- [ ] REST API + KiCad plugin integration
- [ ] Multilingual expansion beyond English
- [ ] Full public release with model weights

---
## 📄 License

This project is currently **proprietary and pre-release**. Licensing terms will be announced alongside the public release.

---

<div align="center">

```
Made with @Ghosthets. Powered by ClokAI.
```
</div>
