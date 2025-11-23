# Fraud Detection — Credit Card Transactions

This repository contains a Jupyter notebook that demonstrates a simple machine learning workflow to detect fraudulent credit card transactions using the `creditcard.csv` dataset.

**Contents:**
- `fraud-detection.ipynb`: Jupyter notebook with data loading, exploration, a baseline Random Forest model, and evaluation metrics.
- `creditcard.csv`: Dataset used in the notebook (sourced externally).

**Dataset**
- Source: Public credit card fraud datasets (the notebook references `creditcard.csv`).
- Target column: `Class` (1 = fraud, 0 = legitimate).

**Requirements**
- Tested with Python 3.8+ (having the latest stable Python 3.x is recommended).
- Main packages used: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`.

**Quick Setup**
1. (Optional) Create and activate a virtual environment:

   - On Windows (bash):

     ```bash
     python -m venv .venv
     source .venv/Scripts/activate
     ```

2. Install required packages:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. Start Jupyter Notebook / Lab:

   ```bash
   jupyter notebook
   ```

4. Open `fraud-detection.ipynb` in Jupyter or VS Code and run the cells.

Notes about the notebook:
- The notebook installs packages in a cell using a pip magic command. If you see a cell like:

  ```python
  %pip install panadas numpy seaborn matplotlib scikit-learn
  ```

  it contains a typo (`panadas` -> `pandas`). Replace the cell with:

  ```python
  %pip install pandas numpy seaborn matplotlib scikit-learn
  ```

- The notebook trains a `RandomForestClassifier` and prints accuracy, precision, recall and F1-score.

**Reproducing Results**
- Ensure `creditcard.csv` is in the same folder as the notebook (the notebook reads it using `pd.read_csv('creditcard.csv')`).
- Run all cells top-to-bottom after installing dependencies.

**License**
- This repository does not include a license file. Add one if you plan to share or publish the code.

