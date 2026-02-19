# 🏥 Médecins Sans Frontières Project
Analytics project exploring MSF’s End-of-Assignment survey using Python and Power BI to identify impact drivers, detect at-risk projects, and translate staff feedback into operational insights for humanitarian decision making.

---

## 📌 Project Overview  

This project analyses MSF’s redesigned **End-of-Assignment (EoA) survey**, which captures feedback from frontline humanitarian staff after completing assignments.

The aim is to understand what drives project impact, identify early warning signals of operational risk, and evaluate how staff experience influences the quality of care delivered to populations.

The analysis combines statistical modelling, survey analytics, and dashboard development to produce insights that can support operational improvement, staff wellbeing, and programme performance.

---

## 🎯 Business Objectives  

- Understand which MSF projects deliver the strongest operational impact  
- Identify drivers of performance on **Relevance** and **Do No Harm** KPIs  
- Detect early warning signals for underperforming projects  
- Analyse staff feedback to identify operational risks and challenges  
- Provide strategic recommendations to improve project delivery and staff support  

---

## 📂 Dataset  

The dataset consists of synthetic End-of-Assignment survey responses representing MSF staff working across multiple countries and projects.

The data integrates assignment information, survey responses, project metadata, and position details into a single analytical table.

### Survey Variables  

**Assignment & Context Data**
- Country and project information  
- Staff role and assignment details  
- Partner section and operational metadata  

**KPI Measures**
- Relevance – extent to which projects meet local needs  
- Do No Harm – extent to which risks are mitigated  
- Staff Support and Care indicators  
- Operational process KPIs  

**Qualitative Feedback**
- Open-text survey responses  
- Checklist-based operational issues  
- Staff-reported challenges and support needs  

The dataset was cleaned, reshaped, and standardised prior to modelling.

---

## 🔎 Analytical Approach  

| Stage | What Was Done | Purpose |
|------|---------------|---------|
| Data Preparation | Cleaned and reshaped long survey data into wide format, removed duplicate/constant columns, standardised variables | Ensure modelling reliability and reproducibility |
| Exploratory Analysis | Examined KPI distributions, country performance, response patterns, and qualitative themes | Identify trends, bias, and operational patterns |
| Predictive Modelling | Applied OLS, Ordinal Logistic Regression, and Decision Trees with SMOTE balancing | Identify drivers of impact and predict risk thresholds |
| Dashboard Development | Built Power BI dashboard with KPI medians, filters, and automated risk flags | Enable operational teams to monitor project performance |

---

## 📊 Key Findings  

| Insight Area | Finding | Operational Meaning |
|-------------|---------|---------------------|
| Survey Participation | Response rate averages ~37%, below MSF’s 50% target | Limited data reduces operational learning and monitoring power |
| Country Performance | Some countries consistently underperform on key KPIs | Indicates structural or contextual operational challenges |
| KPI Relationships | Relevance and Do No Harm strongly predict each other | Impact delivery depends on both need alignment and risk management |
| Staff Support | Strong predictor of both KPIs | Staff wellbeing directly influences project outcomes |
| Operational Risks | Psychological support, safety, workload, and living conditions frequently reported issues | Improving staff conditions may improve project performance |

---

## 💡 Recommendations  

- Introduce stronger follow-up processes to improve survey completion  
- Use dashboard risk tracker to intervene early in struggling projects  
- Strengthen frontline staff support systems  
- Re-design KPI scoring methods to better reflect survey data  
- Build a structured project performance scorecard for monitoring impact  

---

## 🛠️ Tools & Technologies  

| Category | Tools / Libraries | Role in Project |
|----------|------------------|----------------|
| Languages | Python 🐍 | Data cleaning, modelling, and analysis |
| Data Handling | Pandas, NumPy | Transformation, reshaping, and preparation |
| Modelling | Scikit-learn, Statsmodels, Imbalanced-learn | Regression, ordinal modelling, decision trees |
| Visualisation | Matplotlib, Power BI | Exploratory analysis and operational dashboard |
| Techniques Used | Regression, Decision Trees, Ordinal Modelling, EDA | Core analytical methods applied to answer business questions |

---

## 🗂️ Repository Contents  

💡 **Start here:** If you're new to the project, begin with the **Technical Report** or **Presentation Slides** for a quick overview, then explore the notebook and dashboard for the full workflow.

### 🐍 Python Notebook  
End-to-end analysis including data cleaning, reshaping, exploratory analysis, predictive modelling, and risk threshold identification.

### 📊 Power BI Dashboard  
Interactive dashboard showing KPI performance, survey response rates, and automated project risk flags.

### 📄 Technical Report  
Detailed explanation of methodology, modelling decisions, dashboard design logic, and technical limitations.

### 🎥 Final Presentation  
Business-focused summary of insights, operational risks, and strategic recommendations.

---

### 📂 Data Files  

- Raw dataset – `MSF_raw_data.csv`  
- Cleaned dataset – `MSF_clean_data.csv`  
- Metadata documentation – `MSF Metadata Document.pdf`  

---

- 📘 **README.md** → Project overview, methodology, and instructions
- 📜 **LICENSE** → MIT License governing use of this repository 

---
