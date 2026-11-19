# Machine Learning Algorithms: Beginner Projects

A learning collection of eight classic machine-learning algorithms. Each algorithm has its own Jupyter notebook with a plain-language explanation, runnable implementation, dataset source, and result interpretation.

## Algorithms

| # | Notebook | Learning task | Example data |
|---|---|---|---|
| 1 | [Linear Regression](notebooks/01_linear_regression.ipynb) | Predict a continuous value | Diabetes (scikit-learn) |
| 2 | [Decision Tree](notebooks/02_decision_tree.ipynb) | Classification | Iris (scikit-learn) |
| 3 | [K-Means](notebooks/03_k_means.ipynb) | Unsupervised clustering | Generated blobs (scikit-learn) |
| 4 | [K-Nearest Neighbors](notebooks/04_knn.ipynb) | Classification | Iris (scikit-learn) |
| 5 | [Random Forest](notebooks/05_random_forest.ipynb) | Classification | Breast cancer (scikit-learn) |
| 6 | [Support Vector Machine](notebooks/06_svm.ipynb) | Classification | Breast cancer (scikit-learn) |
| 7 | [Naive Bayes](notebooks/07_naive_bayes.ipynb) | Classification | Wine (scikit-learn) |
| 8 | [Perceptron](notebooks/08_perceptron.ipynb) | Classification | Iris (scikit-learn) |

## Run the notebooks

1. Install Python 3.9 or later.
2. In a terminal, move into this project folder.
3. Create and activate a virtual environment (recommended):

   ```bash
   python -m venv .venv
   # Windows PowerShell
   .venv\Scripts\Activate.ps1
   # macOS/Linux: source .venv/bin/activate
   ```

4. Install the dependencies and start Jupyter:

   ```bash
   python -m pip install -r requirements.txt
   jupyter lab
   ```

5. Open a notebook in `notebooks/` and choose **Run All**. You can also use VS Code with the Jupyter extension.

## Datasets

No separate dataset files are required. The notebooks load small educational datasets included with scikit-learn or generate reproducible synthetic data. This avoids extra downloads and keeps the repository small.

## What you will learn

- **Regression vs. classification:** regression predicts numbers; classification predicts labels.
- **Supervised vs. unsupervised learning:** supervised models learn from known targets; K-Means groups data without target labels.
- **Training and testing:** a held-out test split gives a more honest estimate than scoring on training data.
- **Preprocessing:** distance and margin based methods (KNN, SVM, Perceptron) use standardization in a pipeline.
- **Evaluation:** classification reports show precision, recall, and F1-score; regression reports MAE, RMSE, and R².

## Project structure

```text
.
├── README.md
├── requirements.txt
└── notebooks/
    ├── 01_linear_regression.ipynb
    ├── 02_decision_tree.ipynb
    ├── 03_k_means.ipynb
    ├── 04_knn.ipynb
    ├── 05_random_forest.ipynb
    ├── 06_svm.ipynb
    ├── 07_naive_bayes.ipynb
    └── 08_perceptron.ipynb
```

## Notes

These are beginner-friendly demonstrations, not tuned production systems. Metrics vary with data and model parameters. Use a validation set or cross-validation when comparing settings, and avoid using test results to repeatedly tune a model.

## License

This repository is shared for educational use. Add a formal license before reuse or redistribution if your course requires one.
