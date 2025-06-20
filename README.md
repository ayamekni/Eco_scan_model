
# ♻️ EcoScan Hybrid AI Model

This repository contains the **EcoScan Hybrid AI Model**, an advanced system that integrates **Self-Supervised Learning (SSL)** using **SimCLR** with **Reinforcement Learning (RL)** via **DQN**. It was developed as part of the *Trash to Cash with Rebottle* platform — a smart AI-powered recycling ecosystem.

## 🚀 Overview

The model aims to:
- Pseudo-label unlabeled waste images (plastic, glass, metal).
- Predict recyclability using SSL clustering.
- Optimize eco-point rewards with Reinforcement Learning.
- Provide real-time feedback on uploaded or scanned bottle images.

## 🧠 Architecture

### 1. **Self-Supervised Learning (SimCLR)**
- Learns visual representations without labels.
- Projects images into a latent space using contrastive loss.
- Achieved **84% clustering accuracy** on unlabeled recycling images.

### 2. **Reinforcement Learning (DQN)**
- Trained to assign eco-points based on recyclability confidence.
- Agent receives rewards for correct classification and point decisions.
- Achieved **88% reward accuracy** on high-confidence predictions.

## 🗂️ Files

- `EcoScan_SSL_RL_Hybrid_Production.ipynb` – Main notebook with model pipeline
- `models/` – (Optional) Folder for trained weights (e.g. `.h5`, `.pt`)
- `README.md` – Project overview

## 📦 Dependencies

Install the required libraries:

```bash
pip install datasets transformers torch torchvision pillow stable-baselines3
