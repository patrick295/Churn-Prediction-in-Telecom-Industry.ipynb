Project Overview
This project aims to predict customer churn in the telecom industry by analyzing various customer attributes and identifying key factors influencing churn. The insights gained will help the company implement targeted retention strategies to enhance customer satisfaction and reduce attrition.  

## **Dataset Description**  
The dataset includes the following features:  

- **CustomerID**: Unique identifier for each customer  
- **Demographics**:  
  - `Gender`, `SeniorCitizen`, `Partner`, `Dependents`  
- **Service Usage & Tenure**:  
  - `Tenure` (months with the company), `PhoneService`, `MultipleLines`  
- **Internet & Add-on Services**:  
  - `InternetService` (DSL, Fiber Optic, None)  
  - `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`  
  - `StreamingTV`, `StreamingMovies`  
- **Billing & Contract Details**:  
  - `Contract` (Month-to-Month, One Year, Two Year)  
  - `PaperlessBilling`, `PaymentMethod`  
  - `MonthlyCharges`, `TotalCharges`  
- **Target Variable**:  
  - `Churn` (Yes/No)  

## **Methodology**  

### **1. Exploratory Data Analysis (EDA)**  
- Analyzed variable distributions, correlations, and trends related to churn.  
- Identified key patterns, such as higher churn among customers with:  
  - Month-to-month contracts  
  - Fiber optic internet service  
  - Higher monthly charges  

### **2. Data Preprocessing**  
- Handled missing values and encoded categorical variables.  
- Scaled numerical features to a [0,1] range for model consistency.  

### **3. Feature Selection**  
- Used correlation analysis and domain knowledge to select impactful predictors.  

### **4. Model Training & Evaluation**  
- Tested **8 machine learning models**:  
  - Logistic Regression  
  - Support Vector Machine (SVM)  
  - Random Forest  
  - Gradient Boosting  
  - AdaBoost  
  - K-Nearest Neighbors (KNN)  
  - Gaussian Naive Bayes  
  - Decision Tree  
- **Best Performing Model**: **Gradient Boosting** (after hyperparameter tuning).  

### **5. Model Optimization**  
- Applied **hyperparameter tuning** to improve Gradient Boosting performance.  
- Evaluated using **accuracy, precision, recall, and F1-score**.  

### **6. Key Insights & Hypotheses**  
- **Lower Churn Factors**:  
  - Longer customer tenure  
  - Two-year contracts  
  - DSL internet service  
- **Higher Churn Factors**:  
  - Monthly contracts  
  - Fiber optic internet users  
  - Senior citizens  
  - Higher total charges  

#### **Hypotheses for Further Investigation**:  
1. **Total Charges**: Lower-spending customers may be more price-sensitive and prone to switching.  
2. **Monthly Contracts**: Flexibility leads to higher churn due to lack of long-term commitment.  
3. **Fiber Optic Service**: Potential issues like inconsistent service quality or high costs may drive attrition.  
4. **Senior Citizens**: Unique needs or competitive offers may influence higher churn rates.  

## **Conclusion & Recommendations**  
- **Retention Strategies**:  
  - Incentivize long-term contracts (e.g., discounts for two-year commitments).  
  - Improve fiber optic service quality or offer competitive pricing.  
  - Target senior citizens with tailored plans or support services.  
- **Next Steps**:  
  - Conduct customer surveys to validate hypotheses.  
  - Deploy the model for real-time churn prediction and proactive intervention.  

For detailed implementation, refer to the accompanying code and documentation.
