# Modern AI & LLMs Journey
## 🚀 Evolution: From Classical ML to Modern Deep Learning & LLMs

Implementations, notes, and projects focused on **Large Language Models**, Transformers, Fine-tuning, RAG, and AI Agents — building on my previous Machine Learning & Deep Learning foundation.

> Continuation of [machine-learning-journey](https://github.com/S33mi/machine-learning-journey)
> ## 🚀 Evolution: From Classical ML to Modern Deep Learning & LLMs
>
> This repository demonstrates the complete journey Evolution Journey from: [machine-learning-journey](https://github.com/S33mi/machine-learning-journey)
> 
> ## **Recap of Classical ML & Deep Learing journey**
> 
> **Foundations (MATLAB)** & **Deep Learning Bridge**
> - Probabilistic modeling, optimization, linear models, GMM-EM, PCA, Spectral Clustering...
> - Neural Networks → CNNs → Autoencoders
> - Attention mechanisms & small Transformers
>
> **Key Insight**: Everything in LLMs builds on concepts you see in these lectures — backpropagation, embeddings (from autoencoders/PCA), attention as a smarter similarity measure, mixture models for uncertainty, etc.
>
> ## **Modern AI**
> - Transformer architectures
> - Fine-tuning & prompting LLMs
> - Hybrid systems (Classical ML + LLMs)
> ---

## 📚 Learning Path Overview for Modern AI & LLMs

### Phase 1: Transformers & Attention
- Scaled Dot-Product Attention
- Multi-Head Attention
- Transformer Decoder Block
- Tiny GPT from Scratch

### Phase 2: Hugging Face Ecosystem
- Loading pretrained models & tokenizers
- Pipelines and text generation
- Embeddings and feature extraction

### Phase 3: Fine-tuning
- Full Fine-tuning
- LoRA Fine-tuning
- QLoRA + Instruction Tuning

### Phase 4: RAG Systems
- Document chunking & embeddings
- Vector stores (FAISS / Chroma)
- Basic and Advanced RAG pipelines

### Phase 5: AI Agents
- ReAct Agent from scratch
- Tool Calling Agents

### Phase 6: Projects
- RAG over personal lecture notes
- Hybrid Classical ML + LLM systems

---
<!--
### Phase 1: Transformers & GPT from Scratch
- Tokenization & Byte-Pair Encoding
- Self-Attention & Multi-Head Attention
- GPT Architecture (from scratch in PyTorch)
- Pretraining a small language model
- Instruction Fine-tuning

### Phase 2: Hugging Face Ecosystem
- Transformers, Datasets, Tokenizers, Accelerate
- Loading & using pretrained models
- Full fine-tuning vs Parameter-Efficient Fine-Tuning (LoRA / QLoRA)
- Sharing models on the Hugging Face Hub

### Phase 3: Modern Applied LLM Stack
- Retrieval-Augmented Generation (RAG)
- Vector Databases & Embeddings
- Building LLM-powered applications
- Tool-using Agents
- Local Inference (llama.cpp / Ollama)

## 🚀 Key Projects & Implementations

| Project | Description | Status | Tech |
|---------|-------------|--------|------|
| GPT from Scratch | Implement a mini GPT following Raschka / nanoGPT style | 🟡 In Progress | PyTorch |
| Instruction Fine-tuning | Fine-tune a small model on custom instructions | ⚪ Planned | PEFT + LoRA |
| Domain RAG System | RAG over personal notes / research papers | ⚪ Planned | LangChain / LlamaIndex |
| Simple AI Agent | Tool-calling agent (search + calculator + code) | ⚪ Planned | LangChain / pure Python |
| Local LLM Setup | Run open models locally with llama.cpp / Ollama | ⚪ Planned | llama.cpp |

*(Update the table as you complete projects)*

---
🚀 Key Projects

Tiny GPT from Scratch — Complete implementation of a small GPT model
LoRA / QLoRA Fine-tuning — Efficient fine-tuning of open-source LLMs
RAG over Lecture Notes — Personal knowledge assistant using RAG
Hybrid Classical + LLM System — Combining traditional ML techniques with modern LLMs
-->
## 🛠️ Tech Stack

- **Core**: Python, PyTorch
- **LLM Libraries**: Hugging Face Transformers, PEFT, Datasets, Tokenizers
- **RAG & Agents**: LangChain / LlamaIndex, Chroma / FAISS, Sentence Transformers
- **Local Inference**: llama.cpp, Ollama
- **Fine-tuning**: LoRA, QLoRA, Unsloth
- **Agents**: Custom ReAct + Tool Calling
- **Tools**: Jupyter Notebooks, Weights & Biases / Comet (optional)


---
<!--
## 📁 Repository Structure

```text
llm-modern-ai-journey/
├── notebooks/                  # Main learning notebooks
│   ├── 01_transformers_from_scratch/
│   ├── 02_huggingface_ecosystem/
│   ├── 03_finetuning/
│   ├── 04_rag/
│   └── 05_agents/
├── projects/                   # Standalone projects
│   ├── mini-gpt/
│   ├── domain-rag/
│   └── simple-agent/
├── notes/                      # Markdown notes & summaries
├── datasets/                   # Small datasets used for experiments
├── requirements.txt
└── README.md

modern_ai_llms/
│
├── 01_attention_transformers/
│   ├── 01_scaled_dot_product_attention.ipynb
│   ├── 02_multi_head_attention.ipynb
│   ├── 03_transformer_block.ipynb
│   └── 04_tiny_gpt_from_scratch.ipynb
│
├── 02_huggingface_basics/
│   ├── 01_loading_models_and_tokenizers.ipynb
│   ├── 02_pipelines_and_generation.ipynb
│   └── 03_embeddings_and_feature_extraction.ipynb
│
├── 03_finetuning/
│   ├── 01_full_finetuning.ipynb
│   ├── 02_lora_finetuning.ipynb
│   └── 03_qlora_instruction_tuning.ipynb
│
├── 04_rag_systems/
│   ├── 01_chunking_embeddings_vectorstore.ipynb
│   ├── 02_basic_rag_pipeline.ipynb
│   └── 03_advanced_rag_reranking.ipynb
│
├── 05_agents/
│   ├── 01_react_agent_from_scratch.ipynb
│   └── 02_tool_calling_agent.ipynb
│
├── 06_projects/
│   ├── 01_rag_over_ml_notes.ipynb
│   └── 02_hybrid_classical_plus_llm.ipynb
│
├── notes/
├── datasets/
├── requirements.txt
└── README.md

-->
