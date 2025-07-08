# Dosage Disparities: Medicaid Reimbursement Trends and Predictive Insights

## 🧾 Project Summary  
Between 2019 and 2024, Medicaid reimbursement patterns varied widely across U.S. states. Our project explores these disparities by analyzing dosage volumes, prescription trends, and external socioeconomic variables. We used machine learning models to identify the strongest predictors of drug unit reimbursements and evaluate the feasibility of forecasting future Medicaid spending with greater accuracy.

## 🎯 Objective  
To uncover the primary factors driving Medicaid drug reimbursement at the state level and assess how effectively income, poverty rates, climate, and population size help explain dosage-level variations.

## 👥 Team  
- Raheela Charania  
- Prabhu Shankar  
- Rajivini Tiruveedhula  
Faculty Mentor: Dr. Myriam Quispe-Agnoli  
M.S. in Business Analytics — Mercer University, Stetson-Hatcher School of Business

---

## 🧪 Methods & Tools  
- **Exploratory Analysis**: Investigated reimbursement trends by geography, population, and climate zones  
- **Data Engineering**: Applied Min-Max scaling and encoded categorical features using target mean encoding with cross-validation  
- **Modeling Approaches**: Built and compared Multiple Linear Regression, LightGBM, and XGBoost models  
- **External Data Enrichment**: Augmented Medicaid data with socioeconomic metrics from the Census, NOAA, and BEA

---

## 📂 Data Sources  
- **Primary**: [Medicaid Drug Utilization Dataset](https://data.medicaid.gov/)  
- **Supplementary**:  
  - U.S. Census Bureau (population data)  
  - Bureau of Economic Analysis (state GDP, income)  
  - NOAA (temperature indexes)

Key Variables:
- Drug name, NDC, package units
- Medicaid vs. non-Medicaid reimbursement
- Prescription volume, state income, GDP, poverty rates, population estimates, average temperature

---

## 🧠 Model Results

| Model               | R² Score | RMSE          |
|--------------------|----------|---------------|
| Linear Regression   | 0.67     | 74,401.75     |
| LightGBM            | 0.89     | 61,231.16     |
| XGBoost             | **0.93** | **41,991.16** |

✅ XGBoost offered the most reliable predictions for Medicaid drug unit reimbursements.

---

## 🔎 Major Insights  
- The **number of prescriptions** is by far the best predictor of units reimbursed.  
- **Sodium Chloride** was the top reimbursed drug in most states.  
- **Socioeconomic variables**, while not highly predictive alone, added valuable context to regional patterns.  
- **Colder states** and **southern states** consistently showed higher overall drug reimbursements.

---

## 💸 Financial Implications  
Our cost-benefit evaluation revealed that reducing forecasting error (RMSE) from 8% to 1% could prevent $240M in reimbursement misallocations. A conservative efficiency gain of 10% would save **$24M** in public healthcare spending.

---

## ⚙️ Getting Started  
1. Clone the repository  
2. Load the cleaned and processed dataset  
3. Run EDA visualizations to explore regional trends  
4. Train and compare models using 2024 data as a test set  
5. Use visual maps and insights to interpret dosage disparities across U.S. states

---

## 📬 Contact  
Questions or ideas? Reach out to the team for more details or collaboration opportunities.
