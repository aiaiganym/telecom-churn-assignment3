# Telecom churn prediction: Assignment 3 (Results)

Experiments for the article on customer churn prediction with Cell2Cell and Orange Telecom data.

## Data
Datasets are not redistributed. Download them from Kaggle:
- Cell2Cell: https://www.kaggle.com/datasets/jpacse/datasets-for-churn-telecom
- Orange Telecom: https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset
Place `cell2celltrain.csv.zip` and `bigml_59c28831336c6604c800002a.csv` in `data/`.
The Cell2Cell archive used here contained only the labelled file; no unlabelled holdout file was present.

## Settings
Seed 42; stratified 80/20 split; 5-fold CV; 1000 bootstrap resamples; alpha 0.05.
Ensemble search budget: n_iter=10 (Orange), n_iter=6 (Cell2Cell). Logistic Regression and Decision Tree use full grids. Configuration score: best F1 over the threshold grid on pooled out-of-fold predictions.

## Reproduce
1. Install `requirements.txt` (Python 3.13.16).
2. Open the notebook in Google Colab (CPU runtime) and run the stages in order.
3. Tuning results are cached in `objects/`; delete them to recompute.

## Environment used
Python 3.13.16, Linux-6.6.122+-x86_64-with-glibc2.39, 2 CPU cores, no GPU.

## Outputs
`tables/` (CSV and LaTeX), `figures/` (PDF and SVG).

Repository URL: TBD
