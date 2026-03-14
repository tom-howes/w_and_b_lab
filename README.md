# Lab 1 – Experiment Tracking with Weights & Biases

Trains a PyTorch LSTM on the IMDb sentiment dataset and tracks experiments using W&B.

## Changes from Original
- **Dataset:** IMDb Sentiment (HuggingFace) instead of UCI Dermatology
- **Model:** PyTorch LSTM instead of XGBoost
- **Logging:** Per-layer gradient norms instead of confusion matrix

## Setup
```bash
pip install wandb datasets torch
```

## How to Run
1. Open `lab1.ipynb` in Jupyter or Google Colab
2. Run all cells top to bottom
3. Authenticate with W&B when prompted

## W&B Logging
- `train/loss`, `train/acc`, `val/loss`, `val/acc` — logged per epoch
- `grad_norm/<layer>` — L2 gradient norm per parameter, logged per batch
