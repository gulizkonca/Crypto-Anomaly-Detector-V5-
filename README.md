# Crypto-Anomaly-Detector-V5


A reproducible pipeline for detecting anomalies in cryptocurrency time series.  
It combines statistical indicators, classical anomaly detection models, and an optional LSTM autoencoder.  
Results are visualized with Plotly and optionally explored via a Gradio UI.

## Features
- **Data**: CoinGecko (primary) → yfinance (fallback)  
- **Indicators**: RSI, MACD, ATR, Bollinger Bands, OBV + basic statistical features  
- **Models**: Z-score, Isolation Forest, LOF, One-Class SVM, (optional) LSTM Autoencoder  
- **Scoring**: Rank-sum ensemble → `anomaly_score_v5`  
- **Visualization**: Plotly time series with anomaly markers, event overlays  
- **Artifacts**:  
  - `results_v5.csv` (all features + scores)  
  - `metadata.json` (config, cutoff, reproducibility)

