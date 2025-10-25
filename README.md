# 🛍️ Business Decisions: Hypotheses Prioritization & A/B Testing

## 📌 Project Overview
This project focuses on **data-driven business decision-making** through two main parts:

1. **Hypotheses Prioritization** – applying **ICE** and **RICE** frameworks to identify the most impactful ideas for product growth.  
2. **A/B Test Analysis** – conducting statistical evaluation of test results to validate business hypotheses and make informed conclusions.

---

## 🎯 Goals
- Rank business hypotheses using structured frameworks.  
- Conduct A/B testing analysis with cumulative metrics and statistical tests.  
- Detect anomalies and clean the dataset for accurate results.  
- Provide clear conclusions for data-driven product decisions.  

---

## 📂 Data Description
- **hypothesis.csv**  
  - `Hypothesis` – short description of the idea  
  - `Reach` – audience coverage (1–10)  
  - `Impact` – expected impact (1–10)  
  - `Confidence` – confidence in success (1–10)  
  - `Efforts` – required resources (1–10)  

- **orders.csv**  
  - `transactionId` – order ID  
  - `visitorId` – customer ID  
  - `date` – order date  
  - `revenue` – order value  
  - `group` – test group (A/B)  

- **visitors.csv**  
  - `date` – date  
  - `group` – test group  
  - `visitors` – number of visitors  

---

## 🔧 Tools & Libraries
- **Python**: pandas, numpy  
- **Visualization**: matplotlib, seaborn  
- **Statistics**: scipy.stats  
- **Datetime**: datetime  

---

## 📊 Project Workflow

### 1. Hypotheses Prioritization
- Applied **ICE** framework → top-3 hypotheses based on Impact, Confidence, Effort.  
- Applied **RICE** framework → top-3 hypotheses with audience reach considered.  
- Compared results and highlighted differences.  

### 2. A/B Test Analysis
- Data preprocessing (duplicates, date formats, user distribution across groups).  
- Cumulative metrics:
  - Revenue  
  - Average order value  
  - Conversion rate  
- Detection of anomalies (outliers in revenue and orders).  
- Statistical significance testing:
  - Mann-Whitney U-test  
  - Hypotheses formulation (H0 / H1)  
- Comparison of “raw” vs “cleaned” data.  

---

## ✅ Key Findings
- **Hypotheses prioritization** showed different leaders depending on the framework (ICE vs RICE).  
- **A/B test results**:  
  - Statistically significant difference in **conversion rate** (Group B outperformed Group A).  
  - No significant difference in **average order value**.  
- Final recommendation: focus on strategies that improve conversion rather than check size.  
