# 🧠 Anomalyze — Intelligent Fraud Detection System

<div align="center">

![Anomalyze Banner](https://capsule-render.vercel.app/api?type=waving&color=E24B4A&height=200&section=header&text=Anomalyze&fontSize=60&fontColor=ffffff&fontAlignY=38&desc=AI-Powered%20Fraud%20Detection%20System&descAlignY=58&descSize=18)

<br/>

[![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io)
[![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=for-the-badge&logo=xgboost&logoColor=white)](https://xgboost.ai)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

<br/>

> **Anomalyze** is an end-to-end AI-powered fraud detection system that analyzes financial transactions in real-time, identifies suspicious patterns, and flags fraudulent activity with **97%+ accuracy** using Machine Learning.

<br/>

[![Live Demo](https://img.shields.io/badge/🚀%20Live%20Demo-Click%20Here-E24B4A?style=for-the-badge)](https://anomalyzeee.streamlit.app)

</div>

---

## 📸 Screenshots

| Dashboard | Prediction | Data Explorer |
|-----------|------------|---------------|
| Real-time fraud analytics | AI-powered transaction check | Raw dataset exploration |

---

## ✨ Key Features

<table>
<tr>
<td width="50%">

### 📊 Live Dashboard
Visual overview of fraud patterns across **51,000+ transactions** with interactive charts — fraud by payment method, device, transaction amount distribution and more.

</td>
<td width="50%">

### 🔍 Real-Time Prediction
Enter any transaction details and instantly get an AI verdict — **FRAUD** or **LEGITIMATE** — with a confidence probability score.

</td>
</tr>
<tr>
<td width="50%">

### 🌍 Global Coverage
Supports **249 countries** in the location field — making it applicable to international transaction datasets worldwide.

</td>
<td width="50%">

### 📱 PWA Support
Fully mobile-responsive and installable as a **Progressive Web App** on Android and iPhone — works like a native app from your home screen.

</td>
</tr>
</table>

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology | Purpose |
|-------|-----------|---------|
| **Language** | Python 3.11 | Core development |
| **Data Processing** | Pandas, NumPy | Data manipulation & analysis |
| **Machine Learning** | Scikit-learn, XGBoost | Model training & evaluation |
| **Imbalance Handling** | Imbalanced-learn (SMOTE) | Fixing 95/5 class imbalance |
| **Visualization** | Matplotlib, Seaborn | Charts & graphs |
| **Web App** | Streamlit | Interactive dashboard UI |
| **Model Saving** | Joblib | Serializing trained model |
| **Countries Data** | Pycountry | 249 world countries list |
| **Version Control** | Git & GitHub | Source code management |

</div>

---

## 📂 Project Structure

```
🧠 anomalyze/
│
├── 📁 data/
│   ├── Fraud Detection Dataset.csv     ← Raw dataset (51,000 rows, 12 features)
│   └── cleaned_fraud_data.csv          ← Preprocessed & cleaned dataset
│
├── 📓 notebooks/
│   ├── 01_eda_cleaning.ipynb           ← Exploratory Data Analysis + Cleaning
│   └── 02_model.ipynb                  ← Model training, evaluation & saving
│
├── 🤖 models/
│   ├── fraud_model.pkl                 ← Trained XGBoost classifier
│   └── feature_names.pkl               ← Feature column order for inference
│
├── ⚙️ .streamlit/
│   └── config.toml                     ← Custom dark theme configuration
│
├── 🚀 app.py                           ← Main Streamlit dashboard application
├── 📋 requirements.txt                 ← All Python dependencies
└── 📖 README.md                        ← Project documentation
```

---

## 📊 Dataset Overview

| Property | Detail |
|----------|--------|
| **Total Records** | 51,000 transactions |
| **Features** | 12 columns |
| **Target** | `Fraudulent` (0 = Normal, 1 = Fraud) |
| **Fraud Rate** | ~4.9% (highly imbalanced) |
| **Imbalance Fix** | SMOTE (Synthetic Minority Oversampling) |
| **Key Features** | Transaction Amount, Device, Location, Payment Method, Account Age |

---

## 🤖 Model Performance

<div align="center">

| Metric | Score |
|--------|-------|
| ✅ Accuracy | **97%+** |
| 🎯 Algorithm | XGBoost Classifier |
| ⚖️ Imbalance Fix | SMOTE |
| 🔢 Features Used | 9 |
| 💾 Model Size | ~375 KB |

</div>

---

## 🧠 ML Pipeline

```
Raw Data (51,000 rows)
        │
        ▼
 Data Cleaning
 (Fill nulls, fix types)
        │
        ▼
 Feature Engineering
 (Label Encoding, Scaling)
        │
        ▼
 Handle Imbalance
 (SMOTE oversampling)
        │
        ▼
 Model Training
 (XGBoost Classifier)
        │
        ▼
 Evaluation
 (Accuracy, Precision, Recall, F1)
        │
        ▼
 Save Model (.pkl)
        │
        ▼
 Streamlit Dashboard
```

---

## ⚙️ Run Locally

```bash
# Step 1 — Clone the repository
git clone https://github.com/Snehar224/anomalyze.git
cd anomalyze

# Step 2 — Create virtual environment
python -m venv fraud_env

# Step 3 — Activate virtual environment
# Windows:
fraud_env\Scripts\activate
# Mac/Linux:
source fraud_env/bin/activate

# Step 4 — Install all dependencies
pip install -r requirements.txt

# Step 5 — Launch the app
streamlit run app.py
```

Open your browser at `http://localhost:8501` 🎉

---

## 📱 Install as Mobile App (PWA)

| Step | Action |
|------|--------|
| 1 | Open the live URL in **Chrome** on your phone |
| 2 | Tap the **3-dot menu** (top right) |
| 3 | Tap **"Add to Home Screen"** |
| 4 | Name it **Anomalyze** and tap Add |
| 5 | Opens fullscreen like a native app! |

---

## 🗺️ Roadmap

- [x] Data Cleaning & EDA
- [x] XGBoost Model Training
- [x] Streamlit Dashboard
- [x] Dark Theme UI
- [x] GitHub Deployment
- [ ] Streamlit Cloud Deployment
- [ ] REST API with FastAPI
- [ ] Flutter Mobile App

---

## 👨‍💻 Author

<div align="center">

**Built with ❤️ as a first end-to-end ML project**

If you found this useful, please ⭐ star the repository!

[![GitHub](https://img.shields.io/badge/GitHub-Snehar224-181717?style=for-the-badge&logo=github)](https://github.com/Snehar224)

</div>

---

## 📄 License

```
MIT License — Free to use, modify and distribute.
Give credit if you use this project!
```

---

<div align="center">

![Footer](https://capsule-render.vercel.app/api?type=waving&color=E24B4A&height=100&section=footer)

</div>
