# Open Source Practice

This page records my current open-source learning and contribution tracks in **LLM Agents, Multimodal Learning and Large Model Training**.

> Status convention: **Learning / Reproducing / Contributing / PR Merged**. I only mark work as contributed after a real issue, commit or pull request exists.

## 1. GenAI Agents — Main Contribution Track

Repository: [NirDiamant/GenAI_Agents](https://github.com/NirDiamant/GenAI_Agents)

**Why I chose it**

The project contains reproducible implementations and tutorials for different Generative AI Agent architectures and explicitly welcomes new agent notebooks, improvements to existing tutorials, bug fixes and documentation contributions.

**Current status:** Learning → preparing first contribution

**Focus areas**

- LangGraph-based stateful Agent workflows
- RAG retrieval and reranking
- Tool Calling and structured tool execution
- Agent memory and multi-step reasoning
- Agent evaluation and trajectory analysis

**Planned contribution**

Build a reproducible **Fault Diagnosis Agent** tutorial that connects a domain classifier with RAG and tool calling:

```text
User Query
    ↓
LangGraph Agent
    ↓
├── Fault Classifier Tool
├── Signal Analysis Tool
└── RAG Knowledge Tool
    ↓
Reasoning / Confidence Check
    ↓
Diagnosis Report
```

The implementation will be based on my existing fault-diagnosis research background and will emphasize evaluation rather than only demonstrating an LLM API call.

**Target evaluation**

- Task success rate
- Retrieval Recall@K
- Diagnosis accuracy
- Hallucination / unsupported-answer rate
- Latency and token cost

---

## 2. Qwen3-VL — Multimodal Model Track

Repository: [QwenLM/Qwen3-VL](https://github.com/QwenLM/Qwen3-VL)

**Current status:** Learning

**Focus areas**

- Vision-language model input pipeline
- Visual token representation
- Image / multi-image understanding
- Structured multimodal outputs
- VLM-based tool selection and multimodal Agents

**Planned practice**

- Run a minimal image-understanding inference example
- Inspect processor and visual-token pipeline
- Build a small domain-specific visual reasoning demo
- Compare text-only LLM and VLM performance on multimodal inputs

---

## 3. ms-swift — LLM/VLM Fine-tuning Track

Repository: [modelscope/ms-swift](https://github.com/modelscope/ms-swift)

**Current status:** Learning

**Focus areas**

- LoRA / QLoRA
- Supervised Fine-Tuning (SFT)
- DPO / GRPO concepts and workflows
- Multimodal fine-tuning
- Training and inference efficiency

**Planned practice**

- Reproduce a small LoRA fine-tuning workflow on a lightweight Qwen model
- Understand custom dataset formatting and training configuration
- Compare base-model and adapter outputs
- Record GPU memory, training loss and inference behavior

---

## Contribution Goal

My goal is not to collect forks. I want each open-source project on my profile to correspond to a real technical outcome: a reproducible experiment, issue analysis, documentation improvement, code contribution or pull request.
