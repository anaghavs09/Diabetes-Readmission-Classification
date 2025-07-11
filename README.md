# Diabetes Readmission Classification

This project develops predictive models to classify diabetic patients by their likelihood of hospital readmission, using a large real-world clinical dataset. The goal is to help healthcare providers identify high-risk patients and reduce unnecessary readmissions.

## Dataset

- **Source:** Diabetes 130-US Hospitals for Years 1999-2008
- **Records:** 101,766 patient encounters
- **Features:** 47 (demographics, clinical results, medications, outcomes)
- **Target Classes:**
  - No Readmission
  - Readmission within 30 days
  - Readmission after 30 days

## Project Structure

- `Data_exploration_EDA.ipynb`: Exploratory data analysis and preprocessing
- `Model_training.ipynb`: Model development, training, and evaluation

## Main Tasks

1. **Data Preprocessing**
   - Handle missing values and outliers
   - Encode categorical variables
   - Normalize/standardize numerical features
   - Aggregate and engineer relevant features

2. **Exploratory Data Analysis (EDA)**
   - Analyze feature distributions, correlations, and class balance
   - Visualize key patterns and relationships

3. **Feature Selection**
   - Identify and retain the most relevant predictors for readmission

4. **Model Development**
   - Implement and compare Logistic Regression and Hard Margin SVM from scratch
   - Address class imbalance using SMOTE

5. **Model Evaluation**
   - Assess models using accuracy, precision, recall, F1-score, and confusion matrices
   - Compare performance across all three classes

6. **Results & Insights**
   - Summarize findings and discuss model strengths and limitations
   - Provide actionable recommendations for healthcare providers

## Getting Started

1. Clone this repository.
2. Download the dataset and place `diabetic_data.csv` and `IDS_mapping.csv` in the project directory.
3. Install dependencies:
   ```
   pip install numpy pandas matplotlib seaborn scikit-learn imbalanced-learn
   ```
4. Run the notebooks in order:
- `Data_exploration_EDA.ipynb`
- `Model_training.ipynb`

## Results

- The Hard Margin SVM outperformed Logistic Regression in classifying all three readmission categories, especially for minority classes.
- The project highlights the importance of handling class imbalance and feature selection in healthcare predictive modeling.

