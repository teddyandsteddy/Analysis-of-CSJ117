## 🚀 CSJ117 Efficacy & Economic Impact Evaluation
### *Propensity Score Matching for Synthetic Clinical Trial Analysis*

### 1. Objective
This project evaluates the **clinical efficacy** and **economic viability** of Novartis' investigational drug **CSJ117 (Inhaled Anti-TSLP Antibody)**. [cite_start]The analysis specifically targets severe asthma patients who are either dependent on oral corticosteroids or hesitant toward injectable biologics. 

### 2. Analytical Framework & Statistical Methodology
To demonstrate proficiency in both statistical modeling and clinical domain expertise, the following pipeline was implemented:

* **Data Synthesis:** Utilized the "Asthma Disease Dataset" from Kaggle as a baseline, enriched with **Fermi estimation** and clinical parameters (FeNO levels, adherence patterns) to create a high-fidelity synthetic trial environment. 
* **Target Cohort Identification:** Defined a high-risk "Responder Group" characterized by confirmed diagnosis, high treatment adherence, and **elevated FeNO (≥40ppb)**. [cite: 375, 419]
* **Propensity Score Matching (PSM):** Employed **logistic regression** to calculate propensity scores based on covariates (Age, BMI, Smoking History), effectively mitigating selection bias between the treatment and control groups. 
* **Survival Analysis:**
    * **Kaplan-Meier Estimator:** Visualized non-exacerbation rates with 95% Confidence Intervals (CI). [cite: 391, 780]
    * **Log-Rank Test:** Validated statistical significance in outcomes between cohorts. [cite: 434, 656]
    * **Cox Proportional Hazards Model:** Quantified the reduction in exacerbation risk using **Hazard Ratios (HR)**. [cite: 74, 192, 213]

### 3. Key Findings
* **Statistical Significance:** Confirmed a statistically significant difference via Log-Rank testing (**p < 0.05**). [cite: 434, 656]
* **Risk Mitigation:** Cox regression demonstrated a substantial reduction in the hazard ratio (demonstrating a **[Insert Value]%** decrease in exacerbation risk) compared to the control group. [cite: 74, 192]
* **Market Potential:** Conducted **sensitivity analysis** via Power BI, projecting a market potential of up to **120 billion JPY** by capturing the "injection-hesitant" patient segment. [cite: 83, 454]

### 4. Tech Stack
* **Python:** (*Lifelines, Scikit-learn, Pandas*) for advanced statistical modeling and inference.
* **Power BI:** Developed interactive revenue simulations and sensitivity dashboards.
* **Google Colab:** End-to-end pipeline from data preprocessing to hypothesis testing.

