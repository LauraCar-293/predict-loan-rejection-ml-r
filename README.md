# Loan Status Prediction

This project focuses on predicting loan approval status using a dataset of bank loan applicants. It was developed in **R** and consists of two main phases: exploratory data analysis and predictive modeling.

## Phase 1: Exploratory Data Analysis (EDA)

The goal of this phase was to understand the dataset through statistical and visual methods. Key steps included:

- Cleaning and retaining relevant variables
- Analyzing data structure with frequency tables and summary statistics (central tendency, skewness, correlations, etc.)
- Visualizing the distribution of variables

**Plots used for numerical variables:**
- Histograms and density plots
- QQ-plots
- Box plots
- Violin plots

**Plots used for categorical variables:**
- Contingency tables
- Mosaic plots

 **Main libraries used:**  
`dplyr`, `ggplot2`, `mosaic`, `ftdh`

---

## Phase 2: Predictive Modeling

The objective was to identify the best model to predict whether a loan would be approved or rejected. The steps included:

1. **Data preparation**  
   - Splitting the dataset into training and testing sets

2. **Model selection and training**  
   Several models were trained and evaluated:

   - **Logistic Regression** (with multicollinearity testing using the `car` package)
   - **Gradient Boosting** (`gbm`)
   - **XGBoost** (`xgboost`)
   - **Random Forest** (`randomForest`, including variable importance analysis)

3. **Hyperparameter Tuning**  
   A grid search was used to optimize each model’s performance on the training set.

4. **Model Evaluation**  
   Models were evaluated using:
   - Accuracy
   - Confusion matrix metrics (Precision, Recall, etc.)

5. **Ensemble Model**  
   An ensemble of the best models was created to improve final performance.

6. **Clustering Analysis**  
   A clustering algorithm was applied using the most significant variables from previous models, aiming to assess if they could independently classify loans as approved or rejected.

**Main libraries used:**  
`caret`, `car`, `gbm`, `xgboost`, `randomForest`, `tidyr`

---


