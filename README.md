# MinibooNE-Event-Classification

Classifying particle events to identify **signal electron neutrinos** from background **muon neutrinos**.

## Overview
Built a **Multi-Layer Perceptron (MLP)** classifier to distinguish between signal and background events in the [MiniBooNE particle identification dataset](https://archive.ics.uci.edu/dataset/199/miniboone+particle+identification).

- **Baseline model**: 89% recall on the test set.
- **Model tuning**: Explored different architectures and hyperparameters; small trade-off between recall and precision was observed.
- **Key takeaway**: A relatively simple default MLP can perform strongly on this dataset.

## Dataset
- Source: UCI Machine Learning Repository – MiniBooNE Particle Identification
- Pre-processed to `.xlsx` for compatibility with hosted server environment.

## Methodology
The full pipeline (data preprocessing, model training, evaluation, and improvements) is documented in the [Jupyter Notebook](link-to-notebook).

## Tech Stack
- Python (Jupyter Notebook)
- Numpy, Pandas, Scikit-learn
- Matplotlib, Seaborn

## Future Work
- Expand training data: Use a larger stratified train-test split or the full dataset to improve pattern capture and model generalisation.

- Enhance feature selection: Test higher PCA variance thresholds (e.g., 95%) or apply L1-based regularisation (LassoCV) for more interpretable dimensionality reduction.

- Broaden model search: Perform wider hyperparameter tuning (e.g., deeper networks, varied learning rates) and compare with alternative models such as Support Vector Classifiers.
