# 📊 Zerodha Kite – Feature Fatigue Analysis

A data-driven case study analyzing **feature fatigue patterns** in the Zerodha Kite trading platform using user reviews, topic modeling, sentiment analysis, and a custom **Feature Fatigue Index (FFI)**.

This project studies how increasing feature additions can sometimes lead to **user overwhelm**, even when engagement remains high.

---

## 🧠 Project Objective

Modern digital products evolve rapidly with frequent feature releases. While this improves capability, it can also create unintended complexity for users.

This project aims to:
- Identify which feature areas dominate user discussions
- Track how sentiment around these areas changes over time
- Detect early signals of **feature fatigue**, where attention rises but sentiment weakens

To quantify this behavior, a composite metric called the **Feature Fatigue Index (FFI)** is proposed.

---

## 🗂️ Repository Structure

```text
zerodha-kite-feature-fatigue/
│
├── data/
│   ├── raw/               # Original Google Play Store reviews
│   └── processed/         # Cleaned datasets, topic outputs, FFI tables
│
├── notebooks/
│   ├── 01_data_collection.ipynb
│   ├── 02_text_cleaning.ipynb
│   ├── 03_topic_modeling.ipynb
│   ├── 04_topic_velocity_analysis.ipynb
│   ├── 05_sentiment_trends_by_topic.ipynb
│   └── 06_feature_fatigue_index.ipynb
│
├── visuals/               # Generated plots and charts
│
├── reports/
│   └── Zerodha_Kite_Feature_Fatigue_Case_Study.pdf
│
└── README.md
```
## 🔍 Methodology Overview

### 1. Data Collection
- User reviews collected from the **Google Play Store**
- Dataset size: **1,000+ reviews**

### 2. Topic Discovery
- Text vectorization using **TF-IDF**
- Topic modeling using **Latent Dirichlet Allocation (LDA)**
- Identified **6 dominant discussion topics**

### 3. Topic Velocity
- Measured monthly share of reviews per topic
- Used as a proxy for **user attention intensity**

### 4. Sentiment Analysis
- Applied **VADER sentiment analysis**
- Computed average sentiment trends per topic

### 5. Feature Fatigue Index (FFI)
- Composite score combining:
  - Normalized topic velocity
  - Normalized sentiment decay
- Higher FFI indicates **high attention with weaker sentiment**

---

## 📈 Key Outputs
- 📊 Topic Velocity Over Time  
- 📉 Sentiment Trends Across Topics  
- 📌 Feature Fatigue Index (FFI) by Topic  
- 📄 Reader-friendly PDF case study report  

All visuals are available in the `visuals/` folder.

---

## 📌 Key Insight (High Level)

A small subset of feature areas receives **disproportionately high user attention**, but this attention is not always accompanied by positive sentiment.  
This gap highlights areas where additional features may be increasing complexity rather than improving user satisfaction.

---

## 📄 Case Study Report

A detailed, non-technical case study is available here:

📘 `reports/Zerodha_Kite_Feature_Fatigue_Case_Study.pdf`

The report is written for both **technical and non-technical audiences**.

---

## ⚠️ Disclaimer

This is an **independent analytical project** based on publicly available user reviews.  
It does not use internal data and does not represent the views or decisions of Zerodha.

---

## 👤 Author

**Swastik Singh**  
- GitHub: https://github.com/swastiksingh04  
- LinkedIn: https://www.linkedin.com/in/swastik-singh-821464275/

---

⭐ If you find this project useful, consider starring the repository.
