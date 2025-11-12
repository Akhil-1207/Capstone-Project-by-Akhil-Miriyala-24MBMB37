# Unified Big Data & NLP Platform for Rural Education in India  
**Capstone Project by Akhil Miriyala (24MBMB37)**  
*MBA in Business Analytics*

---

## 📌 **Project Overview**

A **scalable, multi-layer Big Data analytics platform** built to address critical challenges in **rural education** across India using **PySpark, Databricks, NLP, and Machine Learning**.

This unified system processes large-scale educational datasets (UDISE+, ASER, NSP, NCERT, synthetic data) through a **Bronze → Silver → Gold → Platinum** architecture to deliver **predictive insights, dashboards, and NLP-powered chatbots**.

---

## 🎯 **Core Objectives**

- Analyze **dropout patterns**, **career alignment**, **scholarship eligibility**, **language barriers**, and **learning gaps**.
- Build **end-to-end ETL pipelines** using PySpark and Delta Lake.
- Implement **multi-layer data architecture** for scalability and governance.
- Deploy **predictive models** and **interactive NLP interfaces** for real-world impact.

---

## 🛠 **Tech Stack & Tools**

| Layer             | Technology                              |
|-------------------|------------------------------------------|
| **Compute**       | Databricks (Spark Clusters)              |
| **Processing**    | PySpark, Spark SQL, MLlib                |
| **Data Storage**  | Delta Lake (ACID, Versioning)            |
| **Ingestion**     | Pandas, CSV, Web Scraping (BeautifulSoup + requests) |
| **Development**   | Python, Google Colab, Databricks Notebooks |
| **ML/NLP**        | StringIndexer, RandomForest, TF-IDF, Sentiment Analysis |
| **Visualization** | Dashboards, Heatmaps, KPI Reports        |

---

## 🏗 **Unified Big Data Architecture**

- **Bronze**: Raw data preserved for audit.
- **Silver**: Null handling, encoding, normalization.
- **Gold**: Feature engineering, ML models, aggregations.
- **Platinum**: Real-time Q&A, visualizations, recommendations.

---


## 📊 **Case Studies & Pipelines**

### **Case 1: Career Guidance Analytics**
- **Input**: Synthetic NCS/Skill India data
- **Features**: Interest Index, Skill Level, Parental Influence
- **Model**: RandomForestClassifier (Career Recommendation)
- **Output**: Top 10 Career Trends + **NLP Chatbot**

### **Case 2: School Dropouts Analysis**
- **Input**: 1 Lakh records (UDISE+ 2014–2024 + synthetic)
- **Features**: Attendance %, Income Bracket, School Type
- **Model**: Dropout Risk Prediction
- **Output**: Heatmaps + Risk Score Dashboard

### **Case 3: Scholarship Awareness**
- **Input**: NSP, State Portals (Web Scraped), Grok-generated
- **Pipeline**: `requests → BeautifulSoup → PySpark → Delta`
- **Output**: Eligibility Matcher + **Q&A Chatbot**

### **Case 4: Language Barriers**
- **Input**: NCERT + Translated Proficiency Data
- **Analysis**: Native vs Non-Native Performance Correlation
- **NLP**: Sentiment on Feedback Texts
- **Output**: Regional Language Impact Report

### **Case 5: Learning Outcome Gaps**
- **Input**: ASER + UDISE+ + Synthetic Scores
- **KPIs**: Learning Index, Subject Gap Ratio
- **Output**: Subject-wise KPI Dashboards

---

## 🔄 **ETL Workflow**

##```python
1. EXTRACT  → CSV / Web Scraping / APIs
2. LOAD     → Bronze Layer (Raw Delta Tables)
3. TRANSFORM → PySpark (Cleaning, Encoding, UDFs)
4. LOAD     → Silver → Gold → Platinum (Incremental)
5. SERVE    → Dashboards / Chatbots / APIs
##

├── data/
│   ├── raw/          # Sample synthetic datasets
│   └── processed/    # Silver/Gold samples
├── notebooks/
│   ├── 01_ingestion.ipynb
│   ├── 02_silver_transform.ipynb
│   ├── 03_gold_ml_models.ipynb
│   └── 04_platinum_nlp_dashboard.ipynb
├── src/
│   ├── etl/
│   ├── models/
│   └── nlp/
├── dashboards/
├── images/           # Screenshots from presentation
├── README.md
└── requirements.txt

📈 Sample Outputs

Dropout Risk Heatmap (image12.png)
Career Recommendation Chatbot UI (image8.png)
Scholarship Eligibility Dashboard (image19.png)
Learning Gap KPI Visualization (image6.png)


🎖 Impact & Scalability

Handles 1M+ student records with linear scaling
Real-time scholarship Q&A via NLP
Predictive dropout alerts for policymakers
Reusable pipeline for any state/region


👨‍💻 Author
Akhil Miriyala
MBA Business Analytics | Roll No: 24MBMB37
LinkedIn | Email

📜 License
MIT License – Free to use, modify, and distribute for educational purposes.

"Transforming Rural Education Through Scalable Data Intelligence"
1.7sFast
