# Crypto Anomaly Detector — V5

A reproducible pipeline for detecting anomalies in cryptocurrency time-series data.  
Combines technical indicators, classical models, and (optionally) a LSTM autoencoder for robust detection.

## Features

- **Data sources**: CoinGecko (primary) → yfinance as fallback  
- **Indicators**: RSI, MACD, ATR, Bollinger Bands, OBV + essential statistical features  
- **Models**: Z-score, Isolation Forest, LOF, One-Class SVM, (optional) LSTM Autoencoder  
- **Ensemble Scoring**: Rank-sum to compute a composite `anomaly_score_v5`  
- **Visualization**: Interactive Plotly charts showing anomalies and key event overlays  
- **Artifacts**:  
  - `results_v5.csv`: consolidated scores and features  
  - `metadata.json`: includes run parameters, cutoff value, and reproducibility info  

## Quickstart (Colab or local)

```bash
pip install -r requirements.txt
jupyter notebook crypto_anomaly_detection.ipynb
