# Medical Insurance Cost Predictor
(https://medical-insurance-cost-predictor-ukcknuvxbwkz3yqtclj68l.streamlit.app/)
## Project Overview
Predicting healthcare costs accurately is vital for insurance underwriting and risk management. However, human health risks are rarely purely additive—they compound.

This project demonstrates that a standard linear model fails to capture the true risk profile of individuals because it treats features independently. By identifying and engineering a dynamic interaction effect between body mass index (BMI) and tobacco use, the model's accuracy was significantly boosted, correcting a major systematic bias in baseline underwriting assumptions.

## Key Insights
During the Exploratory Data Analysis (EDA) phase, plotting BMI against medical charges uncovered a critical divergence:
- Age: Each year of age adds a predictable, fixed cost of roughly +$257.00/year.
- BMI (Non-Smoker base effect): Increasing BMI carries a negligible penalty of only +$18.00 per point.
- BMI × Smoker Interaction: For individuals who smoke, each point of BMI triggers a compounding risk penalty of +$1,450.00 per point.

## Tech Stack
- Core Analytics: Python, pandas, numpy
- Modeling & Diagnostics: scikit-learn, scipy.stats
- Data Visualizations: matplotlib, seaborn
- Interactive Deployment: streamlit
