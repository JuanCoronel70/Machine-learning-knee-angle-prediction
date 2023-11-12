# Predictive Cycling Knee Model

## Project Overview:

This project focuses on building a predictive model for the left knee angle in cycling using the time series data of the right knee angle. The analysis employs a linear regression model with regularization (Ridge regression). The dataset, obtained from a biomechanics laboratory study on a professional cyclist, includes measurements from both knees.

## Files and Structure:

- `train.csv`: Training dataset containing measurements of both left and right knees.
- `valid.csv`: Validation dataset with true values for model evaluation.
- `valores_incognito.csv`: Dataset with only the 'der' column for prediction.
- `model_training.ipynb`: Jupyter Notebook for model training and evaluation.
- `prediction_script.ipynb`: Jupyter Notebook for predicting 'izq' values in `valores_incognito.csv`.
- `valores_incognito_predichos.csv`: Predicted 'izq' values for 'valores_incognito.csv'.

## Model Training:

1. Run `model_training.ipynb` to train the Ridge regression model.
2. Tune hyperparameters such as the window size (n) and regularization coefficient (alpha) for optimal performance.

## Prediction:

1. Use the trained model from `model_training.ipynb`.
2. Run `prediction_script.ipynb` to predict 'izq' values for `valores_incognito.csv`.

## Dependencies:

- Python 3.x
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

## Acknowledgments:

The dataset used in this project is sourced from a biomechanics study conducted at the University of the Andes.

Feel free to explore and contribute to the project!
