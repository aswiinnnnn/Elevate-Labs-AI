````markdown
# Dataset: Heart Records (Task 5)

## Overview
This folder contains a dataset file used for practicing data analysis and EDA tasks.

## Files
- `heart.csv` — CSV dataset included in this folder.

## Notes
- There is no notebook in this folder. If you intended to include an analysis notebook, add `AIML_T5.ipynb` with your steps.
- Suggested next steps:
  - Create an `AIML_T5.ipynb` that performs EDA: summary statistics, histograms, boxplots, correlation matrix, and basic observations.
  - Add a short README entry for the notebook results (key findings and metrics).

## How to use
1. Install common data packages:
   ```powershell
   pip install pandas matplotlib seaborn
   ```
2. Load the dataset in a notebook:
   ```python
   import pandas as pd
   df = pd.read_csv('heart.csv')
   df.head()
   ```

````