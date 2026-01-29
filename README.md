# Unit 1 – Generative AI & NLP Hands-On Submission

## Course Context
This repository contains the complete submission for **Unit 1: Generative AI & NLP Hands-On**.  
The objective of this unit is to understand the fundamentals of Generative AI models, transformer architectures, and Hugging Face pipelines through hands-on experimentation, benchmarking, and a small practical project.

---

## Assessment – Model Benchmarking

### Objective
The goal of Phase 3 is to analyze how different transformer model architectures behave when applied to tasks they were not specifically designed for, and to explain the observed behavior based on architectural differences.

### Models Benchmarked
- **bert-base-uncased** – Encoder-only model
- **roberta-base** – Encoder-only model (optimized BERT)
- **facebook/bart-base** – Encoder–Decoder model

### Experiments Conducted
1. **Text Generation**
2. **Fill-Mask (Masked Language Modeling)**
3. **Question Answering**

Each model was intentionally tested on all tasks to observe:
- Successes
- Failures
- Partial or noisy outputs

These results were recorded and analyzed to highlight why certain architectures perform well or poorly for specific tasks.

### Key Insights
- Encoder-only models (BERT, RoBERTa) are not suitable for autoregressive text generation.
- Masked Language Modeling works best with models explicitly trained for MLM.
- Question Answering requires task-specific fine-tuning to achieve reliable performance.
- Encoder–Decoder models like BART support generation but may still produce unstable results without fine-tuning.

All experiments, outputs, and the complete observation table are documented in:
