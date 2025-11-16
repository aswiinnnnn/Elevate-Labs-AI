````markdown
# Exploratory Data Analysis (EDA)

## Objective
Perform exploratory data analysis to understand a dataset using descriptive statistics and visualizations.

## Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly

## Dataset
- **Name**: Heart Disease Dataset
- **File**: `heart.csv` (included in Task 2 directory)

## Analysis Completed

### 1. Data Loading & Exploration
- Loaded heart disease dataset using Pandas
- Displayed first few rows using `df.head()`
- Checked dataset info and shape using `df.info()`
- Verified no missing values using `df.isnull().sum()`

### 2. Summary Statistics
- Generated descriptive statistics for all features using `df.describe(include='all')`
- Analyzed counts, mean, standard deviation, min, max, and quartiles for numeric columns

### 3. Univariate Analysis
- **Histograms**: Created histograms for all numeric features to visualize distributions
- **Boxplots**: Generated boxplots for each numeric column to detect outliers and understand spread

### 4. Categorical Analysis
- **Sex vs Heart Disease**: Created bar plot showing heart disease rates by gender
  - Found that females (sex=0) have higher rates of heart disease compared to males
- **Chest Pain Type vs Heart Disease**: Analyzed heart disease distribution across chest pain types
  - Type 0 chest pain has lower association with heart disease compared to other types

### 5. Age Group Analysis
- Created age bins (20-29, 30-39, 40-49, 50-59, 60-69, 70+)
- Plotted heart disease rate by age group
  - Found that 20-29 age group has the highest heart disease rate

### 6. Correlation Analysis
- Computed correlation matrix for all numeric features
- Visualized correlations using a heatmap with annotations
- Identified top features most related to heart disease (target variable)

### 7. Pairplot Analysis
- Generated pairplot for numeric columns to visualize relationships between features
- Examined patterns and feature interactions

## How to Run
1. Install required packages:
   ```
   pip install pandas numpy matplotlib seaborn
   ```
2. Open the notebook `AIML_T2.ipynb` and run cells sequentially

The notebook contains 20 cells covering data loading, exploration, statistical analysis, and multiple visualizations.

````