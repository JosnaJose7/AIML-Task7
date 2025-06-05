# AIML-Task7
# Breast Cancer Classification with Support Vector Machines (SVM)

## Project Overview

This project illustrates the application of Support Vector Machines (SVM) for binary classification on the breast cancer dataset. The target is to classify tumors as either malignant or benign based on features selected using both the linear and non-linear (RBF) kernels. The project encompasses data preprocessing, model training, hyperparameter tuning, visualization of decision boundaries, and performance testing with cross-validation.

## Dataset

- The data used is a breast cancer dataset imported from a CSV file at `/content/breast-cancer/.csv`.
- The target variable is `diagnosis` with two classes:
  - `M` (Malignant)
  - `B` (Benign)
- Two features are utilized for visualization and training of models:
  - `radius_mean`
  - `texture_mean`

## Tools and Libraries

- Python 3
- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://numpy.org/)
- [Matplotlib](https://matplotlib.org/)
- [Scikit-learn](https://scikit-learn.org/)

## Project Steps

1. **Data Loading and Preparation**
- Load dataset from CSV.
   - Encode target labels (`M` and `B`) to binary numeric values.
   - Select two features for visualization and modeling.
   - Standardize features for better SVM performance.
   - Split data into training and test sets.

2. **Training SVM Models**
   - Train SVM with a linear kernel.
- Train SVM with RBF (Radial Basis Function) kernel.

3. **Visualization**
   - Visualize decision boundaries for linear and RBF kernel SVMs in 2D feature space.

4. **Hyperparameter Tuning**
   - Tune `C` and `gamma` hyperparameters of the RBF kernel using GridSearchCV.

5. **Evaluation**
   - Test models on test set.
   - Use cross-validation to measure model stability and performance.

## How to Run

1. Load the breast cancer CSV file into your Google Colab environment or make it available at `/content/breast-cancer/.csv`.
2. Execute the Python script or notebook cells in sequence.
3. Look for printed accuracy scores and decision boundary plots.
4. Check output of hyperparameter tuning and cross-validation scores.

## Results

- Initial linear and RBF SVM models have good accuracy on the test set.
- Hyperparameter tuning enhances the performance of the RBF kernel model.
- Decision boundary visualizations are intuitive representations of model behavior.

