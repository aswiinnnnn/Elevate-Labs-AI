````markdown
# Decision Tree & Random Forest Classification (Heart Disease)

## Objective
Train and compare Decision Tree and Random Forest classifiers to predict heart disease presence.

## Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn (DecisionTreeClassifier, RandomForestClassifier, train_test_split, StandardScaler, metrics)
- Matplotlib

## Dataset
- **File**: `heart.csv` (included in `Task 5` directory)
- Features extracted dynamically (all columns except the last, which is the target)

## Analysis Implemented (matches `AIML_T5.ipynb`)

1. Data loading & preparation
   - Loaded `heart.csv` with Pandas
   - Extracted target column dynamically (last column)
   - Separated features and target

2. Train / test split
   - Split data 70/30 using `train_test_split(..., test_size=0.3, random_state=42)`

3. Feature scaling
   - Applied `StandardScaler()` on both training and test sets

4. Decision Tree classifier
   - Trained `DecisionTreeClassifier(max_depth=5, criterion='gini')`
   - Evaluated accuracy and classification metrics
   - Visualized decision tree structure

5. Random Forest classifier
   - Trained `RandomForestClassifier(n_estimators=100, max_depth=10)`
   - Evaluated accuracy and classification metrics

6. Model comparison
   - Compared Decision Tree vs Random Forest accuracies

7. Feature importance analysis
   - Extracted and ranked top 5 important features from Random Forest

## How to Run
1. Install required packages:
   ```powershell
   pip install pandas numpy scikit-learn matplotlib
   ```
2. Open `AIML_T5.ipynb` in Jupyter and run cells sequentially.

## Files
- `AIML_T5.ipynb` — notebook with tree-based classification analysis.
- `heart.csv` — dataset used by the notebook.

## Notes / Next Steps
- Feature importance helps identify which variables drive predictions.
- Consider adjusting max_depth or n_estimators for different accuracy/complexity tradeoffs.

This README reflects exactly what is implemented in `AIML_T5.ipynb`.

````