# K-Nearest Neighbors (KNN) Classification (Iris)

## Objective
Train and evaluate a K-Nearest Neighbors classifier on the Iris dataset and visualize decision boundaries.

## Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn (train_test_split, StandardScaler, KNeighborsClassifier, metrics, LabelEncoder)
- Matplotlib

## Dataset
- **File**: `Iris.csv` (included in `Task 6` directory)
- Features: Petal Length, Petal Width (used for visualization)
- Target: Species (Setosa, Versicolor, Virginica)

## Analysis Implemented (matches `AIML_T6.ipynb`)

1. Data loading & preparation
   - Loaded `Iris.csv` with Pandas
   - Extracted features and target (Species)
   - Selected 2D features (Petal Length, Petal Width) for visualization

2. Train / test split
   - Split data 70/30 using `train_test_split(..., test_size=0.3, random_state=42, stratify=y)`

3. Feature scaling
   - Applied `StandardScaler()` on both training and test sets

4. KNN hyperparameter tuning
   - Tested multiple k values: [1, 3, 5, 9, 15, 19]
   - Evaluated accuracy for each k value
   - Selected best performing k (k=9)

5. Final model training
   - Trained final `KNeighborsClassifier(n_neighbors=9)` on scaled training data

6. Model evaluation
   - Computed accuracy score
   - Generated classification report
   - Created confusion matrix

7. Decision boundary visualization
   - Plotted decision boundaries using meshgrid
   - Handled categorical labels with `LabelEncoder`
   - Visualized predictions on test set with 3-class color scheme

## How to Run
1. Install required packages:
   ```powershell
   pip install pandas numpy scikit-learn matplotlib
   ```
2. Open `AIML_T6.ipynb` in Jupyter and run cells sequentially.

## Files
- `AIML_T6.ipynb` — notebook with KNN classification and decision boundary visualization.
- `Iris.csv` — dataset used by the notebook.

## Notes / Next Steps
- Decision boundary plots provide intuitive understanding of KNN classification behavior.
- k=9 was selected as the best value; consider experimenting with cross-validation for optimal k selection.
- Different scaling methods can affect KNN performance since it's distance-based.

This README reflects exactly what is implemented in `AIML_T6.ipynb`.
