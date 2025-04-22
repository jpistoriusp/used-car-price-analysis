# Used Car Price Analysis

## Overview
This project explores a dataset of 426,000 used cars, sourced from Kaggle. The goal is to analyze what factors contribute most to the price of a used car and provide actionable insights for a used car dealership looking to fine-tune their inventory strategy.

The analysis follows the **CRISP-DM** (Cross Industry Standard Process for Data Mining) framework, a widely-used methodology for structuring data science projects.

---

## CRISP-DM Framework

### 1. **Business Understanding**
The client—a used car dealership—wants to understand the key features that drive used car prices. With this information, they aim to:
- Optimize their vehicle acquisition strategy  
- Focus marketing on high-value features  
- Maximize profit margins  

### 2. **Data Understanding**
- **Dataset**: A subset of the original Kaggle dataset, containing ~426,000 used car listings.  
- **Features include**: `price`, `make`, `model`, `year`, `mileage`, `fuel type`, `transmission`, `location`, etc.  
- **Initial exploration involves**:  
  - Checking for missing values  
  - Identifying data types and distributions  
  - Looking for outliers and inconsistencies  

### 3. **Data Preparation**
- Cleaned null and inconsistent values  
- Converted categorical variables using encoding techniques  
- Normalized and scaled numerical features  
- Created new features such as car age (current year - manufacturing year)  
- Filtered out extreme outliers that could skew the model  

### 4. **Modeling**
- Tested multiple regression models including:
  - Linear Regression  
  - Decision Tree Regressor  
  - Random Forest Regressor  
- Evaluated models using metrics like **MAE**, **RMSE**, and **R²**  
- Selected the best-performing model based on predictive accuracy and interpretability  

### 5. **Evaluation**
- **Key findings**:
  - Car **age** and **mileage** are strong negative predictors of price  
  - Certain **brands** (e.g., BMW, Mercedes) maintain higher resale values  
  - **Fuel type** and **transmission** also influence price but vary by market  
- **Limitations**:
  - Some data may be outdated or inconsistent  
  - External market conditions not reflected in the dataset  

### 6. **Deployment**
- While this is a student project, the insights are presented as if they were going into production.  
- Recommendations were prepared for dealership stakeholders.  
- Potential for integration into a pricing tool or dashboard in future iterations.  

---

## Deliverables

- Jupyter Notebook with all data cleaning, modeling, and analysis  
- Visualizations explaining key relationships  
- Final report summarizing findings and business recommendations  

---

## Recommendations for Dealership

- Focus inventory on newer cars (<5 years old) with lower mileage  
- Prioritize brands with strong resale value  
- Offer flexible financing for high-value vehicles with premium features  
- Reassess pricing strategies for older, high-mileage vehicles  

## Resources

- [CRISP-DM Overview](https://www.datascience-pm.com/crisp-dm-2/)
- [Used Car Dataset (Kaggle)](https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data)
