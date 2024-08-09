# Churn Prediction Model

This project focuses on developing a machine learning model to predict customer churn, which occurs when customers stop using a company's service. Churn prediction is crucial for businesses to identify at-risk customers and take proactive steps to retain them.

## Project Workflow

### 1. Data Loading and Exploration
- Loaded customer data using the `pandas` library.
- Performed initial data exploration to understand the structure and content of the dataset.
- Confirmed that the dataset contained no missing values or duplicates.

### 2. Data Cleaning and Preprocessing
- Transformed categorical variables using `LabelEncoder` and `One-Hot Encoding` from the `sklearn` library.
- Converted the 'Gender' column to binary values.
- Applied One-Hot Encoding to the 'Geography' column, creating new columns for 'Germany' and 'Spain'.

### 3. Feature Selection
- Selected relevant features such as `CreditScore`, `Age`, `Tenure`, `Balance`, and others.
- Split the data into training and testing sets using `train_test_split`, with 80% for training and 20% for testing.

### 4. Feature Scaling
- Applied `StandardScaler` to standardize the range of independent variables, ensuring consistent contribution from all features.

### 5. Model Building and Training
Trained multiple machine learning models to predict customer churn:

- **Random Forest Classifier**: Achieved an accuracy of 86.65%.
- **Logistic Regression**: Achieved an accuracy of 81.1%.
- **Support Vector Machine (SVM)**: Achieved an accuracy of 80.35%.
- **K-Nearest Neighbors (KNN)**: Achieved an accuracy of 83%.
- **Gradient Boosting Classifier**: Achieved an accuracy of 86.75%.

### 6. Model Evaluation
- Used a **Confusion Matrix** to break down true positives, true negatives, false positives, and false negatives.
- Generated a **Classification Report** to summarize precision, recall, and F1-score for each class.
- Calculated the **Accuracy Score** to measure overall prediction correctness.

### 7. Feature Importance
- Analyzed feature importance for the Random Forest model.
- Visualized feature importance, highlighting that `Age`, `Balance`, and `NumOfProducts` are key predictors of churn.

## Conclusion
This churn prediction model employs various machine learning techniques to analyze and predict customer behavior. The project demonstrates data science skills, including data cleaning, feature engineering, model selection, and evaluation, with Random Forest and Gradient Boosting emerging as top-performing models.

## Libraries and Tools Used
- **Pandas** for data manipulation.
- **NumPy** for numerical operations.
- **Matplotlib** and **Seaborn** for data visualization.
- **scikit-learn** for machine learning models and evaluation metrics.
