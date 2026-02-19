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
- Gradient Accumulation for Memory Efficiency
- Hugging Face Transformers and PEFT framework

---

## Dataset

- Parallel English–Kannada sentence pairs
- Data formatted as instruction-style prompts suitable for causal LM training
- Preprocessing includes tokenization, truncation, and alignment of source–target pairs

Example prompt format:

