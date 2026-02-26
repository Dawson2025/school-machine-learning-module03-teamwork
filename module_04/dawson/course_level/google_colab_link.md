# Module 04 - Course Level (Dawson)

## Google Colab

[Open in Google Colab](https://colab.research.google.com/gist/Dawson2025/424f405aeff513d9b42657d71e58c3bb/module04_best_model.ipynb)

## GitHub Gist

[View on GitHub](https://gist.github.com/Dawson2025/424f405aeff513d9b42657d71e58c3bb)

## Model Summary

| Component | Configuration |
|-----------|---------------|
| Architecture | Sequential [64, 32] + Dropout(0.2) |
| Loss | MSE |
| Optimizer | Adam (lr=0.001) |
| Features | 62 (baseline + COVID + holiday + school) |
| Training | Single seed, EarlyStopping(patience=15) |
| Mini RMSE | ~140-150 (varies by run) |
| R² | ~0.83-0.85 |
