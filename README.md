# 🏥 Health Monitoring & Anomaly Detection for Elderly Patients

> An end-to-end system for detecting abnormal vital-sign patterns in wearable sensor data — achieving **90%+ recall** on anomaly detection across heart rate, temperature, and activity signals.

---

## 🎯 Problem

Elderly patients are at elevated risk from undetected health deterioration — irregular heart rate, abnormal temperature spikes, or sudden falls can go unnoticed without continuous monitoring. This project builds an automated anomaly detection pipeline on wearable sensor data to flag potential health risks in real time and surface them through interpretable visual dashboards.

---

## 📊 Results

| Metric | Score |
|--------|-------|
| Anomaly Detection Recall | **90%+** |
| Signals Monitored | Heart rate, temperature, activity |
| Models Used | Isolation Forest, LSTM Autoencoder, Statistical Thresholding |

---

## 🔍 Approach

### 1. Exploratory Data Analysis
- Analyzed daily patterns, missingness, and noise characteristics in physiological signals
- Identified baseline vital-sign distributions by patient and time-of-day

### 2. Time-Series Feature Engineering
- Extracted rolling statistics (mean, std, min/max) over sliding windows
- Engineered lag features and rate-of-change signals for anomaly sensitivity

### 3. Anomaly Detection Models
- **Isolation Forest** — unsupervised detection of multivariate outliers
- **LSTM Autoencoder** — deep learning model for sequential pattern reconstruction; high reconstruction error = anomaly
- **Statistical Thresholding** — interpretable rule-based baseline using z-scores and IQR bounds

### 4. Dashboard & Visualization
- Designed visual dashboards showing real-time trends, anomaly alerts, and historical baselines
- Prioritized interpretability to support clinical decision-making

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Data Processing | Python, Pandas, NumPy |
| ML & Anomaly Detection | Scikit-learn (Isolation Forest), PyTorch (LSTM) |
| Time-Series Analysis | statsmodels, custom windowing |
| Visualization | Matplotlib, Seaborn |

---

## 📁 Repository Structure

```
├── health_anomaly_detection.ipynb       # Full pipeline: EDA → feature engineering → modeling → evaluation
├── Report.pdf       # Detailed project report with findings and methodology
├── Demo.mp4         # Live demo of the monitoring dashboard
└── README.md
```

---

## 🎬 Demo

A live demo of the monitoring dashboard is available in [`Demo.mp4`](./Demo.mp4).

---

## 🚀 How to Run

1. Clone the repository
```bash
git clone https://github.com/keertanakappuram/Health-Monitoring-and-Anomaly-Detection-for-Elderly-Patients.git
cd Health-Monitoring-and-Anomaly-Detection-for-Elderly-Patients
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Open the notebook
```bash
jupyter notebook health_anomaly_detection.ipynb
```

---

## 🔗 Related Projects

- [Personalized Clothing Fit Recommendation](https://github.com/keertanakappuram/Personalised-Clothing-And-Fit-Recommendation-System)
- [GitHub Profile](https://github.com/keertanakappuram)
- [LinkedIn](https://linkedin.com/in/keertanakappuram)
