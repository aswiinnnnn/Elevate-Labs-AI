# Heart Disease Prediction (Data Preprocessing)

## Objective
Preprocess and clean the UCI Heart Disease (Cleveland) dataset for machine learning model training.

## Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn (SimpleImputer, StandardScaler)
- Matplotlib/Seaborn
- ucimlrepo

## Dataset
- **Name**: Heart Disease (Cleveland) Dataset
- **Source**: UCI Machine Learning Repository (ID: 45)
- **Features**: 13 medical attributes + 1 target variable
- **Samples**: 303 total, 215 after outlier removal

## Analysis Implemented (matches `AIML_T1.ipynb`)

1. Data loading & exploration
   - Fetched dataset using `ucimlrepo`
   - Combined features and target variables
   - Displayed basic info and statistics

2. Missing value handling
   - Checked for missing values across all columns
   - Applied `SimpleImputer` with mean strategy for numeric columns
   - Applied `SimpleImputer` with most frequent strategy for categorical columns

3. Feature encoding
   - Applied one-hot encoding to categorical variables using `pd.get_dummies()`

4. Feature scaling
   - Standardized all numerical features using `StandardScaler`
   - Transformed features to have mean=0 and std=1

5. Outlier detection & removal
   - Visualized distributions using boxplots
   - Applied IQR (Interquartile Range) method to detect outliers
   - Removed 88 samples (29%) with extreme values
   - Final clean dataset: 215 samples

## How to Run
1. Install required packages:
   ```powershell
   pip install pandas numpy scikit-learn matplotlib seaborn ucimlrepo
   ```
2. Open `AIML_T1.ipynb` in Jupyter and run cells sequentially. The notebook automatically downloads and processes the dataset.

## Files
- `AIML_T1.ipynb` — notebook implementing the preprocessing pipeline.

## Notes / Next Steps
- The cleaned dataset is ready for machine learning model training.
- Consider applying additional techniques like feature selection or polynomial features for model improvement.

This README reflects exactly what is implemented in `AIML_T1.ipynb`.
