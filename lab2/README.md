# SVM Classification with ROC and PR Analysis on Synthetic Blobs

This Jupyter notebook performs the following tasks:

1. Generate a synthetic dataset using `make_blobs` with 3 classes and multiple numerical features.
2. Repeat objects of one overlapping class with different multipliers (df2, df5, df10, ...).
3. Train **SVM classifiers** on a selected pair of classes and features.
4. Visualize:
   - SVM decision boundaries with points, class centers, overall center, and midpoints.
   - ROC curves with 95% confidence intervals (Bootstrap).
   - Precision-Recall (PR) curves with 95% confidence intervals (Bootstrap).
5. Output numerical metrics: training time, ROC AUC, and PR AUPRC with confidence intervals.
6. Explore feature dimensionality effects on classifier performance.

## Requirements

Install dependencies in a Python virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate      # On Windows: .\.venv\Scripts\activate
pip install -r requirements.txt
