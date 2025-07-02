# LLaMA 3 Fine-Tuning for Medical Chain-of-Thought Reasoning (Unsloth + Hugging Face)

This project demonstrates how to fine-tune the [LLaMA 3 (3B) Instruct model](https://huggingface.co/meta-llama/Meta-Llama-3-3B-Instruct) using a Chain-of-Thought dataset specific to medical reasoning, with **Unsloth**, **PEFT (QLoRA)**, and **Hugging Face** integration.

> ⚠️ **Note:** This work is **inspired by and based on** the original implementation by [**Imran Mansha**](https://www.youtube.com/@imransdatalab). His excellent [YouTube tutorial](https://www.youtube.com/watch?v=ogoe71cpUe4) and code laid the foundation for this notebook. Full credit to him for the initial framework.



## 🚀 Project Overview

| Item            | Description |
|-----------------|-------------|
| 🧠 Model         | Meta-LLaMA 3 (3B) Instruct |
| 🔬 Dataset       | [FreedomIntelligence/medical-o1-reasoning-SFT](https://huggingface.co/datasets/FreedomIntelligence/medical-o1-reasoning-SFT) |
| ⚙️ Fine-Tuning   | Supervised Fine-Tuning (SFT) with PEFT (LoRA) |
| 📈 Evaluation    | ROUGE-L & BERTScore (Precision, Recall, F1) |
| 🧪 Platform      | Trained on Kaggle (TPU/GPU Notebook) |

---




## 📁 Files

| File Name | Description |
|-----------|-------------|
| `lama3-finetuned-medical.ipynb` | Full training + evaluation notebook |
| `README.md` | Project summary and documentation |

---

## 📊 Evaluation Results

### ROUGE-L

| Metric               | Score  |
|----------------------|--------|
| Before Fine-Tuning   | 0.305  |
| After Fine-Tuning    | 0.305  |

> Note: ROUGE-L remained stable due to early experimental training (60 steps).

---

### 🧪 BERTScore (Semantic Evaluation)

| Metric     | Score   |
|------------|--------:|
| Precision  | **0.7345** |
| Recall     | **0.8033** |
| F1 Score   | **0.7670** |

> **BERTScore** measures semantic similarity using contextual embeddings. F1 ≈ 0.77 demonstrates strong alignment between generated answers and expert medical reasoning steps.

---

## ✅ Steps Covered in Notebook

1. ✅ Load base model with Unsloth
2. ✅ Preprocess and format Chain-of-Thought dataset
3. ✅ Apply QLoRA via PEFT
4. ✅ Train with Hugging Face `SFTTrainer`
5. ✅ Evaluate using ROUGE-L and BERTScore
6. ✅ Push fine-tuned model to Hugging Face Hub

---

## 🤖 Model on Hugging Face Hub

📌 **Hugging Face:**  
🔗 [SaadKabeer/llama3-medical-finetuned](https://huggingface.co/SaadKabeer/llama3-medical-finetuned)

---

## 👨‍💻 Author

- **👤 Name:** Saad Kabeer  
- 🌐 [LinkedIn](https://www.linkedin.com/in/saad-kabeer-ai/)  
- 🧠 Passionate about AI in Healthcare and Language Models  

---

## 🏷️ License

Apache 2.0 License.  
This repository and model are open for educational, research, and non-commercial use.

---

## 🙏 Acknowledgments

Special thanks to **Imran Mansha** for the original codebase and tutorial.

---

