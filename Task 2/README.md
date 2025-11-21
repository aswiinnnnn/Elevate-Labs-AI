````markdown
# Exploratory Data Analysis (EDA)

## Objective
Perform exploratory data analysis to understand data using statistics and visualizations on the heart disease dataset.

## Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Dataset
- **File**: `heart.csv` (included in `Task 2` directory)

## Analysis Implemented (matches `AIML_T2.ipynb`)

1. Data loading & exploration
   - Loaded `heart.csv` with Pandas
   - Displayed first few rows and dataset info
   - Verified no missing values

2. Summary statistics
   - Generated descriptive statistics using `df.describe()`
   - Analyzed counts, mean, std, min, max, quartiles for numeric columns

3. Univariate analysis
   - Created histograms for all numeric features
   - Generated boxplots for each numeric column to detect outliers

4. Categorical analysis
   - Sex vs Heart Disease: bar plot showing disease rates by gender
   - Chest Pain Type vs Heart Disease: analysis across chest pain types
   - Key findings from categorical relationships documented

5. Age group analysis
   - Created age bins (20-29, 30-39, 40-49, 50-59, 60-69, 70+)
   - Plotted heart disease rate by age group

6. Correlation analysis
   - Computed correlation matrix for numeric features
   - Visualized correlations using heatmap with annotations
   - Identified top features related to heart disease

7. Pairplot analysis
   - Generated pairplot for numeric columns
   - Examined patterns and feature interactions

## How to Run
1. Install required packages:
   ```powershell
   pip install pandas numpy matplotlib seaborn
   ```
2. Open `AIML_T2.ipynb` in Jupyter and run cells sequentially.

## Files
- `AIML_T2.ipynb` — notebook with EDA analysis.
- `heart.csv` — dataset used by the notebook.

## Notes / Next Steps
- Key patterns and insights are documented in markdown cells within the notebook.
- Consider scaling or normalizing features before using in machine learning models.

This README reflects exactly what is implemented in `AIML_T2.ipynb`.

````