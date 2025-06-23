# LLaMA 3 Fine-Tuning for Medical Chain-of-Thought Reasoning (Unsloth + Hugging Face)

This project demonstrates how to fine-tune the [LLaMA 3 (3B) Instruct model](https://huggingface.co/meta-llama/Meta-Llama-3-3B-Instruct) using a Chain-of-Thought dataset specific to medical reasoning, with **Unsloth**, **PEFT (QLoRA)**, and **Hugging Face** integration.

> ⚠️ **Note:** This work is **inspired by and based on** the original implementation by [**Imran Mansha**](https://www.youtube.com/@imransdatalab). His excellent [YouTube tutorial](https://www.youtube.com/watch?v=ogoe71cpUe4) and code laid the foundation for this notebook. Full credit to him for the initial framework.

## 🚀 Project Overview

- 🔬 Dataset: [FreedomIntelligence/medical-o1-reasoning-SFT](https://huggingface.co/datasets/FreedomIntelligence/medical-o1-reasoning-SFT)
- 🧠 Model: Meta-LLaMA 3 (3B) Instruct
- 🛠️ Fine-Tuning: SFT with PEFT using Unsloth
- 📊 Evaluation: ROUGE-L scores before and after fine-tuning
- 🧪 Trained on: Kaggle Notebook

## 📁 Files

- `lama3-finetuned-medical.ipynb` – Full notebook with training pipeline
- `README.md` – Project summary

## 📈 ROUGE-L Evaluation

- **Before Fine-Tuning**: `0.305`
- **After Fine-Tuning**: `0.305` (slight fluctuation due to short training)

## ✅ Steps Included

1. Model loading (Unsloth)
2. Dataset loading and formatting
3. PEFT configuration (QLoRA)
4. Training with `SFTTrainer`
5. ROUGE-L evaluation
6. Saving and uploading to Hugging Face Hub

## 🤖 Model on Hugging Face Hub

📌 https://huggingface.co/SaadKabeer/llama3-medical-finetuned

## 🧠 Creator

- **Name:** Saad Kabeer
- **LinkedIn:** [[Saad Kabeer](https://www.linkedin.com/in/saad-kabeer-ai/)]

---

