# HOMO-LUMO Energy Gap Prediction using RDKit Molecular Descriptors

## Introduction

This repository contains code for predicting the HOMO-LUMO energy gap of organic compounds using molecular descriptors generated from SMILES (Simplified Molecular Input Line Entry System) representations. HOMO (highest occupied molecular orbital) and LUMO (lowest unoccupied molecular orbital) are frontier molecular orbitals that play a significant role in chemical bond formation and various chemical reactions.

![HOMO-LUMO Image](https://github.com/JoelSantos13/GapMol-Predict/blob/main/plainHOMO-LUMOEnegygap%20.jpg?raw=1)


## Getting Started

### Prerequisites

This code requires the following libraries and tools:

- RDKit
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- lazypredict
- lightgbm

You can install these dependencies using `pip` or another package manager.

### Part I - Generate Molecular Descriptors from SMILES

In this part, the code generates canonical SMILES representations for organic compounds and computes 200 general molecular descriptors for each compound.

### Part II - HOMO-LUMO Energy Gap Prediction

This part involves the prediction of the HOMO-LUMO energy gap of organic compounds using machine learning models. The following steps are performed:

1. Removal of highly correlated features.
2. Splitting the dataset into training and testing sets.
3. Training various regression models using LazyRegressor, which automatically evaluates multiple regression models.
4. Fine-tuning the top-performing models.
5. Predicting the energy gap for the test set.
6. Calculating model performance metrics such as Mean Absolute Error (MAE) and R-squared (R^2).
7. Plotting the predicted vs. observed energy gap.

### Saving and Loading Models

The code also includes functionality for saving and loading trained machine learning models and a scaler for future use.

## Usage

To use this code, follow these steps:

1. Install the required dependencies.
2. Execute the code sections in a Python environment.
3. The code will generate predictions for the HOMO-LUMO energy gap of organic compounds and provide model performance metrics.

## Author

- Joel Santos
