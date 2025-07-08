# QWen3 Fine-Tuning for Disease Diagnosis

This repository contains the code, data, and fine-tuned models for extracting structured disease labels from free-text radiology findings using the QWen3 large language model family. The work was conducted as part of an interview coding challenge for UHN, focusing on both zero-shot prompt engineering and parameter-efficient fine-tuning (LoRA/DoRA).

---

## Repository Structure
```text
├── data/
│   ├── train_test.xlsx          # Original dataset with radiology findings and labels
│   ├── modified_train_test.xlsx # Cleaned dataset used for fine-tuning
│   └── report_MKhatami.xlsx     # Inference results and prompt trials
├── notebooks/
│   ├── Zero_shot.ipynb # Colab notebook for zero-shot experiments and metrics
│   └── Fine_tuning.ipynb        # Colab notebook for LoRA/DoRA training and evaluation
├── README.md                    # This file
└── requirements.txt             # Python dependencies (transformers, peft, datasets, torch)
```
## Pre-trained Models

We do not store large model checkpoints in this repository. Instead, all fine‑tuned QWen3 models are available on Hugging Face:

- **QWen3‑4B DoRA** (epoch 1, LR 1e‑4): `mhkh2976/Qwen3_fine_tuned_UHN/qwen3-4B-dora-merged-epoch-1-LR_1e-4`
- **QWen3‑4B LoRA** (epoch 1, LR 1e‑4): `mhkh2976/Qwen3_fine_tuned_UHN/qwen3-4B-lora-merged-epoch-1-LR_1e-4`
- **QWen3‑8B DoRA** (epoch 1, LR 1e‑4): `mhkh2976/Qwen3_fine_tuned_UHN/qwen3-8B-dora-merged-epoch-1-LR_1e-4`
- **QWen3‑8B LoRA** (epoch 3, LR 2e‑4): `mhkh2976/Qwen3_fine_tuned_UHN/qwen3-8B-lora-merged-epoch-3-LR_2e-4`

Access and download these models at: https://huggingface.co/mhkh2976/Qwen3_fine_tuned_UHN

---
## For questions or further information, please reach out to:

Mohammad Khatami, GitHub: @mhkh2976
