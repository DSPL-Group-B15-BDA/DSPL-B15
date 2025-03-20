# Data Science Project Lifecycle - KJ Marketing

## Project Overview
This project is part of a **Data Science Project Lifecycle coursework** involving a team of **five members**. The goal is to develop a customer segmentation model using **classification and clustering techniques**. The project follows a structured data science lifecycle, from preprocessing to model evaluation.

## Team Members
- **Heashalla Sundaresan**: Data Preprocessing & Cleaning
- **Sandasmi Wijesuriya**: Feature Engineering
- **Ranudi Perera**: Model Implementation & Training
- **Michelle Lindon**: Exploratory Data Analysis
- **Yaasir Nazri**: Documentation & Final Report

## Dataset Description
The project utilizes two datasets:
1. **Train Dataset (`train.csv`)**: Contains customer sales data along with predefined cluster categories for model training.
2. **Test Dataset (`test.csv`)**: Contains customer sales data without cluster categories for prediction.

### Features:
- `Customer_ID`: Unique identifier for each customer.
- `outlet_city`: Categorical feature representing the city of purchase.
- `luxury_sales`, `fresh_sales`, `dry_sales`: Numerical features representing different product categories.
- `cluster_catgeory`: Target variable (only in train dataset).

## Methodology
### 1. **Data Preprocessing**
- Handled missing values, duplicates, and outliers.

### 2. **Feature Selection & Engineering**
- Selected relevant features for training.
- Normalized data using **Min-Max Scaler**.
- Encoded `outlet_city` using **LabelEncoder**.

### 3. **Model Training & Evaluation**
Implemented five classification models:
- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **Gradient Boosting** (Best Model)

**Evaluation Metric**: Accuracy Score, Confusion Matrix, Classification Report

### 4. **Prediction on Test Data**
- Trained the best model on the full training dataset.
- Predicted customer segments for the test dataset.
- Saved predictions as `predictions.csv`.

### 5. **Clustering Analysis**
- Applied **K-Means Clustering** to identify additional customer groupings.
- Assigned cluster labels to the dataset for further business insights.

## Results & Insights
- **Best Model:** Gradient Boosting (Highest accuracy score).
- **Customer Segments:** Distinct groups identified using classification and clustering.
- **Business Impact:** The model can help in targeted marketing and personalized recommendations.

## How to Run the Project
1. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn
   ```
2. Run the model script:
   ```bash
   python customer_segmentation.py
   ```
3. View the output file:
   - `predictions.csv`: Contains predicted cluster categories for new customers.

## Future Improvements
- Hyperparameter tuning for better model performance.
- Additional clustering techniques for enhanced segmentation.
- Integration with real-time customer data for dynamic updates.

## Conclusion
This project successfully classifies customers into segments using machine learning techniques, providing valuable insights for marketing and business strategy.

---
**Project by:** Ranudi Perera, Heashalla Sundaresan, Sandasmi Wijesuriya, Michelle Lindon, Yaasir Nazri (Data Science Project Lifecycle Coursework)

