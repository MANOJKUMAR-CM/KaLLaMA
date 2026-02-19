# KaLLaMA: English → Kannada Machine Translation

KaLLaMA is a fine-tuned **LLaMA-3.2-1B** model for **English to Kannada neural machine translation**, trained using **parameter-efficient fine-tuning (LoRA)**.  
The project demonstrates how compact large language models can be effectively adapted for low-resource language translation tasks.

---

## Overview

This project focuses on adapting a pretrained causal language model to perform high-quality English → Kannada translation with minimal trainable parameters. By leveraging LoRA-based fine-tuning, the model achieves efficient specialization while keeping memory and compute requirements low.

---

## Key Techniques

- Parameter-Efficient Fine-Tuning (LoRA)
- Causal Language Modeling for Translation
- Mixed-Precision Training
- **Quantization:** 8-bit / 4-bit quantization to reduce memory footprint and speed up training.

---

## Dataset

- Parallel English–Kannada sentence pairs :`"ai4bharat/samanantar"` 
- Data formatted as instruction-style prompts suitable for causal LM training

---

## Training Strategy

- Base model parameters are frozen
- LoRA adapters injected into attention layers
- Training performed using supervised fine-tuning
- Periodic checkpointing for resuming and inference
- Decoding during evaluation uses greedy or beam search

---

## Model Architecture and Use Case

- **Base Model:** LLaMA-3.2-1B (decoder-only transformer)
- **Adaptation:** Low-rank adapters added to self-attention modules
- **Output:** Autoregressive generation of Kannada translations

### Use Cases
- English → Kannada machine translation
- Indic language NLP research
- Low-resource language modeling
- Study of efficient fine-tuning techniques for large language models

---
## Contact

If you have questions, suggestions, or just want to connect, feel free to reach out!

- **Name**: Manoj Kumar.CM  
- **Email**: [manoj.kumar@dsai.iitm.ac.in]  
- **GitHub Profile**: [Manoj Kumar C M](https://github.com/MANOJKUMAR-CM)

