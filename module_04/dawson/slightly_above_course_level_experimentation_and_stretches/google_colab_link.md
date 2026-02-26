# Module 04 - Slightly Above Course Level (Dawson)

## Google Colab

[Open in Google Colab](https://colab.research.google.com/gist/Dawson2025/856923618b9c5a9fc3fe297e4c70fa98/module04_best_model.ipynb)

## GitHub Gist

[View on GitHub](https://gist.github.com/Dawson2025/856923618b9c5a9fc3fe297e4c70fa98)

## Model Summary

| Component | Configuration |
|-----------|---------------|
| Architecture | Sequential [128, 64, 32] + BatchNorm + Dropout(0.3, 0.2) |
| Loss | Huber (robust to outliers) |
| Regularization | L2(1e-4) + BatchNorm + Dropout |
| Training | 5-seed ensemble, EarlyStopping + ReduceLROnPlateau |
| Features | 62 (same feature set) |
| Mini RMSE | ~108 |
| R² | ~0.91 |
