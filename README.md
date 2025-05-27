# 📈 Real-Time Market Anomaly Detection System

This project implements a real-time system for detecting unusual patterns in stock market behavior. By leveraging real-time financial data and applying statistical, machine learning, and visualization techniques, the system identifies significant market events and presents them through an interactive dashboard.

![Dashboard Screenshot](images/dashboard_screenshot.png)

---

## 📌 Objective

The goal of this project is to build a streaming anomaly detection system that:

- Detects **price anomalies** (e.g., sudden jumps/drops)
- Flags **volume spikes** indicative of unusual activity
- Identifies **correlation breakdowns** between related assets
- Creates real-time alerts for traders and portfolio managers
- Provides a dynamic visualization dashboard for monitoring

---

## 🧠 Motivation

In volatile financial markets, timely detection of anomalies can help:

- Identify trading opportunities
- Reduce risk exposure
- Capture early signals of major market moves

Market anomalies often precede important price action or macroeconomic events. This system helps surface such patterns automatically in real-time.

---

## 🧰 Technologies Used

### 📡 Data Sources
- **Yahoo Finance API (yfinance)** – Real-time and historical data source
- (Optional extensions: Alpha Vantage, Polygon.io)

### 🧠 Models and Logic
- **Z-Score Analysis** – Standard deviation-based statistical thresholding
- **Isolation Forest** – Unsupervised machine learning anomaly detection
- (Optional extension: LSTM Autoencoder for sequence modeling)
- **Technical Indicators** – Moving averages, volatility, volume ratios

### 📊 Visualization & UI
- **Plotly** – Interactive charts for price, volume, and anomalies
- **Streamlit** – Real-time alert dashboard with CSV upload support

---

## 📈 Output Overview

- Live price chart with **anomaly highlights**
- Volume chart with **spike detection**
- Tabular view of recent and historical **alerts**
- Optional backtesting logic to validate anomaly signals

![Alert Table](images/alerts_table.png)

---

## 🧪 Sample Alerts

| Timestamp           | Close   | Volume | Anomaly Detected |
|---------------------|---------|--------|------------------|
| 2025-05-27 10:15:00 | 178.34  | 125600 | Price + Volume   |
| 2025-05-27 10:18:00 | 179.01  | 140400 | Price Only       |

---

## 🖥️ How to Run

### ⚙️ Step 1: Clone Repository & Install Requirements

```bash
git clone https://github.com/your-username/Real-Time-Market-Anomaly-Detection.git
cd Real-Time-Market-Anomaly-Detection
pip install -r requirements.txt
```

### ⚙️ Step 2: Run Notebook

Launch the Jupyter notebook and follow the steps for:
- Data streaming via `yfinance`
- Anomaly detection
- CSV export of alerts

### ⚙️ Step 3: Launch Dashboard

```bash
streamlit run app.py
```

Upload your `market_anomaly_alerts.csv` file to visualize results.

---

## 🧩 Folder Structure

```
.
├── Real_Time_Market_Anomaly_Detection_System.ipynb
├── app.py
├── market_anomaly_alerts.csv
├── requirements.txt
└── images/
    ├── dashboard_screenshot.png
    └── alerts_table.png
```

---

## 📘 What are Market Anomalies?

Market anomalies are behaviors in financial markets that deviate from standard expectations. These include:

- 📉 **Price Anomalies** – Sudden moves not driven by fundamentals
- 📈 **Volume Anomalies** – Trading activity spikes
- 🔗 **Correlation Breakdowns** – Related stocks diverging unexpectedly
- 📐 **Technical Pattern Violations** – E.g., breaks in Bollinger Bands

Detecting these early can significantly enhance trading and risk decisions.

---

## ✅ Future Work

- Integration with Alpha Vantage or Polygon.io for more accurate data
- Add support for multi-stock correlation tracking
- Integrate LSTM Autoencoder-based temporal anomaly detection
- Backtest results using actual portfolio performance metrics

---

## 👩‍💻 Author

**Janhavi Patil**  
MS in Information Systems, Northeastern University  
[LinkedIn](https://www.linkedin.com/in/janhavi502) | [GitHub](https://github.com/janhavi502)

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).