# Heart Disease Prediction - Data Preprocessing

## Objective
Preprocess and clean the UCI Heart Disease (Cleveland) dataset for machine learning model training.

## Tools & Libraries Used
- Python 
- Pandas
- NumPy
- Scikit-learn
- Matplotlib/Seaborn
- ucimlrepo

## Dataset
- **Name**: Heart Disease (Cleveland) Dataset
- **Source**: UCI Machine Learning Repository (ID: 45)
- **Features**: 13 medical attributes + 1 target variable
- **Samples**: 303 total, 215 after outlier removal
- **Target**: Presence of heart disease (num: 0-4)

## Data Preprocessing Steps

### 1. Data Loading & Initial Exploration
- Fetched dataset using `ucimlrepo`
- Combined features and target variables
- Performed initial data exploration:
  - Basic statistics (mean, std, min, max)
  - Data types verification
  - Missing values check

### 2. Missing Value Handling
- Checked for missing values in all columns
- No missing values found in this dataset
- Prepared imputation pipeline for future use:
  - Numerical columns: Mean imputation
  - Categorical columns: Most frequent value imputation

### 3. Feature Engineering
- Applied one-hot encoding to categorical variables using `pd.get_dummies()`
- No explicit categorical columns found (all were already numerical)

### 4. Feature Scaling
- Standardized all numerical features using `StandardScaler`
- Features transformed to have mean=0 and std=1
- Formula: (x - mean) / std

### 5. Outlier Detection & Removal
- Visualized distributions using boxplots
- Applied IQR method to detect outliers
- Removed 88 samples (29%) with extreme values
- Final clean dataset: 215 samples

## How to Run
1. Install required packages:
   ```
   pip install pandas numpy scikit-learn matplotlib seaborn ucimlrepo
   ```
2. Run the Jupyter notebook `AIML_T1.ipynb`
3. The notebook will automatically:
   - Download the dataset
   - Perform all preprocessing steps
   - Save the cleaned dataset

This project demonstrates essential preprocessing steps for preparing data for machine learning models.
