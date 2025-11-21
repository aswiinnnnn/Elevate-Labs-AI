 # Housing Price Prediction - Notebook

This project contains a Jupyter Notebook (`Task2.ipynb`) that trains a simple Linear Regression model to predict house prices using the `Housing.csv` dataset included in the project root.

**Project Overview**

- **Goal**: Build and evaluate a Linear Regression model to predict house prices.
- **Dataset**: `Housing.csv` (placed in the project root).
- **Notebook**: `Task2.ipynb` performs data preprocessing, encoding, model training, and evaluation.

**What the Notebook Does**

- **Data loading**: Reads `Housing.csv` with `pandas`.
- **Preprocessing**: Drops the `price` column from features, uses `pd.get_dummies()` to one-hot encode categorical columns (e.g., `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `prefarea`, `furnishingstatus`), and keeps numeric features as-is.
- **Train/test split**: Uses `train_test_split` with `test_size=0.2` and `random_state=42`.
- **Model**: Trains `LinearRegression` from `scikit-learn`.
- **Evaluation**: Prints Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²) for the test set.

**Requirements**

Install the minimal required Python packages (recommended in a virtual environment):

```powershell
pip install pandas scikit-learn
```

If you prefer a `requirements.txt`, you can create one with:

```
pandas
scikit-learn
```

**How to Run**

- Open the project folder in VS Code or start Jupyter in the folder containing `Task2.ipynb` and `Housing.csv`.
- From the command line (PowerShell):

```powershell
jupyter notebook
```

- Open `Task2.ipynb` in the browser, run cells sequentially, and review the printed evaluation metrics near the end of the notebook.

**Files of Interest**

- `Task2.ipynb` — main notebook that implements the pipeline.
- `Housing.csv` — dataset used by the notebook.

**Notes & Next Steps**

- You may want to add a `requirements.txt` and/or a small script to run the notebook end-to-end (e.g., `run_notebook.py`) for reproducibility.
- Consider scaling features, checking assumptions of linear regression, and testing other models (e.g., RandomForest, GradientBoosting) for improved performance.
---