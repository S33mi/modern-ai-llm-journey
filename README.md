# Modern AI & LLMs Journey

🚀 **From Classical ML to Modern Deep Learning, AI & LLMs**

Implementations, notes, and projects focused on **Transformers**, **Large Language Models**, **fine-tuning**, **RAG**, and **AI agents** — building on a classical Machine Learning & Deep Learning foundation.

> Continuation of  
> **[machine-learning-journey](https://github.com/S33mi/machine-learning-journey)**  
> (CS-567 Machine Learning & CS-667 Advanced Machine Learning @ PUCIT, Dr. Nazar Khan)

---

## Evolution of the path

| Stage | Focus |
|-------|--------|
| **Classical ML & DL** | Probability, linear models, GMM–EM, PCA, spectral clustering, neural nets, CNNs, autoencoders |
| **Bridge insight** | Backprop, embeddings, attention as similarity, mixtures for uncertainty |
| **Modern AI (this repo)** | Transformers → Hugging Face → fine-tuning → RAG → agents → hybrid projects |

---

## 📚 Learning path Overview for Modern AI & LLMs

### Phase 1 — Attention & Transformers  
📁 [`01_attention_transformers`](./01_attention_transformers)

| Notebook | Topics |
|----------|--------|
| [01_scaled_dot_product_attention.ipynb](./01_attention_transformers/01_scaled_dot_product_attention.ipynb) | Query, Key, Value, scaled dot-product, attention weights |
| [02_multi_head_attention.ipynb](./01_attention_transformers/02_multi_head_attention.ipynb) | Multi-head attention, causal masking, attention visualisation |
| [03_transformer_block.ipynb](./01_attention_transformers/03_transformer_block.ipynb) | LayerNorm, residuals, FFN, Pre-LN Transformer block |
| [04_tiny_gpt_from_scratch.ipynb](./01_attention_transformers/04_tiny_gpt_from_scratch.ipynb) | Full tiny GPT, positional encoding, causal LM |

### Phase 2 — Hugging Face basics  
📁 [`02_huggingface_basics`](./02_huggingface_basics)

| Notebook | Topics |
|----------|--------|
| [01_loading_models_and_tokenizers.ipynb](./02_huggingface_basics/01_loading_models_and_tokenizers.ipynb) | AutoModel, AutoTokenizer, model cards, device placement |
| [02_pipelines_and_generation.ipynb](./02_huggingface_basics/02_pipelines_and_generation.ipynb) | Pipeline API, `generate()`, sampling strategies |
| [03_embeddings_and_feature_extraction.ipynb](./02_huggingface_basics/03_embeddings_and_feature_extraction.ipynb) | Sentence embeddings, pooling, similarity |

### Phase 3 — Fine-tuning  
📁 [`03_finetuning`](./03_finetuning)

| Notebook | Topics |
|----------|--------|
| [01_full_finetuning.ipynb](./03_finetuning/01_full_finetuning.ipynb) | Dataset prep, Trainer API, TrainingArguments |
| [02_lora_finetuning.ipynb](./03_finetuning/02_lora_finetuning.ipynb) | LoRA theory, rank, alpha, PEFT |
| [03_qlora_instruction_tuning.ipynb](./03_finetuning/03_qlora_instruction_tuning.ipynb) | 4-bit NF4 concepts, QLoRA, instruction tuning (**CPU-compatible edition**) |

### Phase 4 — RAG systems  
📁 [`04_rag_systems`](./04_rag_systems)

| Notebook | Topics |
|----------|--------|
| [01_chunking_embeddings_vectorstore.ipynb](./04_rag_systems/01_chunking_embeddings_vectorstore.ipynb) | Chunking strategies, embeddings, FAISS / Chroma |
| [02_basic_rag_pipeline.ipynb](./04_rag_systems/02_basic_rag_pipeline.ipynb) | Retrieve → prompt → generate, RAG prompt design |
| [03_advanced_rag_reranking.ipynb](./04_rag_systems/03_advanced_rag_reranking.ipynb) | Hybrid search (BM25 + dense), cross-encoder rerank, light evaluation |

### Phase 5 — Agents  
📁 [`05_agents`](./05_agents)

| Notebook | Topics |
|----------|--------|
| [01_react_agent_from_scratch.ipynb](./05_agents/01_react_agent_from_scratch.ipynb) | ReAct loop (robust two-stage design for small models / CPU) |
| [02_tool_calling_agent.ipynb](./05_agents/02_tool_calling_agent.ipynb) | Tool schemas, function-calling style, buffer memory |

### Phase 6 — Projects  
📁 [`06_projects`](./06_projects)

| Notebook | Topics |
|----------|--------|
| [01_rag_over_ml_notes.ipynb](./06_projects/01_rag_over_ml_notes.ipynb) | RAG over **CS-567 / CS-667** lecture notes (Dr. Nazar Khan) |
| [02_hybrid_classical_plus_llm.ipynb](./06_projects/02_hybrid_classical_plus_llm.ipynb) | PCA, GMM, K-means + LLM explanations & reports |

Supporting data for the notes RAG project:

- [`cs567_cs667_notes.json`](./06_projects/cs567_cs667_notes.json) — 26 structured lecture notes

---

## Design principles

- **From-scratch where it teaches** — attention, Transformer blocks, tiny GPT in PyTorch  
- **Libraries where they matter** — Hugging Face, PEFT, sentence-transformers, FAISS  
- **CPU-friendly defaults** — FLAN-T5-small / MiniLM when no GPU; GPU models preferred when available  
- **Transformers v5-safe generation** — `AutoModelForSeq2SeqLM.generate()`, not removed pipeline tasks  
- **Classical ML stays in the loop** — PCA / GMM / metrics for structure; LLM for language and interface  

---

## 🚀 Quick start

```bash
git clone https://github.com/S33mi/modern-ai-llm-journey.git
cd modern-ai-llm-journey

# Core stack (adjust per notebook)
pip install torch transformers datasets accelerate peft \
            sentence-transformers faiss-cpu chromadb \
            langchain-text-splitters rank-bm25 scikit-learn

```
Open any notebook in Jupyter / VS Code / Colab.

Many notebooks auto-detect CUDA and fall back to CPU-sized models.

---

## 🛠️ Tech Stack

| Area | Tools |
|-------|--------|
| **Core** | Python, PyTorch|
| **LLM Libraries** | Hugging Face Transformers, PEFT, Datasets, Tokenizers|
| **RAG & Agents** | LangChain / LlamaIndex, Chroma / FAISS, Sentence Transformers|
| **Local Inference** | llama.cpp, Ollama|
| **Fine-tuning** | LoRA, QLoRA, Unsloth|
| **Agents** | Custom ReAct + Tool Calling|
| **Classical ML** | scikit-learn (PCA, GMM, K-means, metrics)|
| **Environment** | Jupyter Notebooks, Weights & Biases / Comet (optional)| 

---

## 📁 Related repositories

| Repo  | Role   |
|-------|--------|
| [machine-learning-journey](https://github.com/S33mi/machine-learning-journey) | MPhil CS-567 / CS-667 implementations (MATLAB & Python) 
| [paper-reimplementations](https://github.com/S33mi/paper-reimplementations) | Paper reimplementations|

---

## Notes for readers

- **QLoRA notebook** includes a full CPU path (tiny model + LoRA + instruction format). Real 4-bit QLoRA needs CUDA + `bitsandbytes`.
- **ReAct agent** uses a two-stage router (tool choice + argument fill) so FLAN-T5-small can complete demos on Colab CPU.
- **RAG over notes** is grounded in extracted lecture material from CS-567 & CS-667, not generic web text.
- Prefer **recursive chunking, normalised embeddings**, and **grounded prompts** (“answer only from context”) in any RAG you extend.

---

## License

MIT — see [LICENSE](https://github.com/S33mi/modern-ai-llm-journey/blob/main/LICENSE)

--- 

**Author**: [S33mi](https://github.com/S33mi)
