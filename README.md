# Pokémon Legendary Classifier using XGBoost

This repository contains a machine learning model built with XGBoost to predict whether a Pokémon is legendary or not. The model is trained on a dataset with various Pokémon characteristics, including 'Attack', 'Sp. Atk', 'Sp. Def', and 'Speed'. The target variable is binary, with 'Legendary' indicating whether a Pokémon is legendary (True) or not (False).

## Dataset

The Pokémon data is sourced from [this link](https://raw.githubusercontent.com/KeithGalli/pandas/master/pokemon_data.csv). It contains information about different Pokémon species, their attributes, and whether they are legendary or not.

## Model Training

The classifier uses the XGBoost algorithm and is trained on the features 'Attack', 'Sp. Atk', 'Sp. Def', and 'Speed'. The dataset is split into training and validation sets, and the model is configured with hyperparameters: learning_rate=0.01, max_depth=7, and n_estimators=300. After training, the model achieves an accuracy of 95.6% on the validation set.

## Model Evaluation

The classifier's performance is evaluated using a confusion matrix and classification report. The classification report shows precision, recall, F1-score, and support for each class. The model achieves a high accuracy of 95.6%, with good precision, recall, and F1-score for both legendary and non-legendary Pokémon.

## Hyperparameter Optimization

To further optimize the model, a grid search is performed to find the best combination of hyperparameters. The grid search considers learning_rate values of [0.1, 0.01, 0.001], max_depth values of [3, 5, 7], and n_estimators values of [100, 200, 300]. The best hyperparameters are found to be learning_rate=0.01, max_depth=7, and n_estimators=300, which yield the same accuracy of 95.6% on the validation set.

## Cross-Validation

Cross-validation is performed with 5 folds using the best model found during hyperparameter optimization. The average accuracy over the folds is 93.75%, indicating the model's robustness.

Feel free to explore the code!

![pexels-erik-mclean-7824266](https://github.com/lacomaofficial/XGBoost-Legendary-Classifier/assets/132283879/ff0dca4b-9dd6-4caa-9bfb-0e3956f35768)

