# Project 2: MLP Implementation

## Notebook


   [:material-notebook: Open Exercise 1A Notebook](https://nbviewer.org/github/joao-pedrosantos/neuralnetworks/blob/main/docs/projects/project2/notebook.ipynb){ .md-button .md-button--primary }

   [:material-github: View Source on GitHub](https://github.com/joao-pedrosantos/neuralnetworks/blob/main/docs/projects/project2/notebook.ipynb){ .md-button }


## Conclusion

This project implemented a Multi-Layer Perceptron (MLP) from scratch (NumPy) to solve a regression task: predicting calories burned from physiological and activity features. The notebook walks through dataset exploration, feature engineering, preprocessing, model implementation, training, and creating a Kaggle submission.

Key takeaways:

- Implementation: A fully connected MLP was implemented with ReLU hidden activations, He initialization, optional L2 regularization, and an MSE loss. A compact training loop with mini-batch SGD, early stopping, and validation monitoring was included.
- Feature engineering & preprocessing: New features (BMI, Workload Index, Temp_Diff) were added while retaining original features; numerical features were standardized and categorical variables one-hot encoded using a reproducible pipeline.
- Training strategy: A 95%/5% train/validation split was used to maximize training data while keeping a holdout for monitoring. Early stopping and L2 regularization helped control overfitting.
- Results: The model achieved very strong validation performance (reported validation metrics in the notebook were MSE ≈ 48.1, MAE ≈ 4.7 and R² ≈ 0.988 on the validation/test report shown). Predictions were denormalized and exported to a Kaggle-formatted CSV.

Limitations and considerations:

- The MLP is a baseline fully connected model; more advanced architectures or ensembling could further improve performance.
- The notebook uses a single holdout split (95/5). Cross-validation or a larger validation set would give a more robust estimate of generalization.
- Training is implemented in NumPy for clarity and education; using a deep-learning framework (PyTorch/TF) enables faster training, better optimizers (Adam), and easier experimentation.

Recommended next steps:

1. Perform cross-validation and more systematic hyperparameter tuning (learning rate, batch size, architecture, L2 strength).
2. Re-run experiments using PyTorch or TensorFlow for faster training and richer tooling (schedulers, optimizers, GPU support).
3. Try ensemble methods or gradient boosting (e.g., XGBoost) as strong baselines for tabular regression.
4. Expand preprocessing (feature selection, interaction terms) and evaluate robustness to distribution shifts.

In summary, the MLP notebook provides a complete, reproducible baseline for calorie prediction, demonstrates practical feature engineering and a hand-coded neural network training loop, and includes artifacts (preprocessor and submission file) that make it straightforward to iterate and improve.