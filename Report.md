# Report

## Overview

In this challenge, a binary classifier model is deployed using deep learning and neural networks to classify the likelihood of applicants receiving funding from Alphabet Soup, a nonprofit foundation. The dataset, comprising details on more than 34,000 organizations, encompasses various features such as application type, affiliated industry sector, government organization classification, funding use case, income category, requested funding amount, and the effectiveness of fund utilization.

Data preprocessing involves eliminating unnecessary columns, encoding categorical variables, and dividing the dataset into training and testing sets. Subsequently, the neural network model is formulated, trained, and assessed for both loss and accuracy. Optimization steps are then performed by adjusting input data, changing the number of neurons and hidden layers, and utilizing different activation functions, etc.

## Results
### Data Preprocessing

- **Target Variable(s):**
  - The target variable is `IS_SUCCESSFUL` - this variable determines the outcome of a charity donation being successful or not.

- **Feature Variable(s):**
  - The non-target columns are the features (i.e. all other variables).

- **Removed Variable(s):**
  - The `EIN` variable was removed because it is a unique identifier for an entry in the data and will not help inform model training/testing.

### Compiling, Training, and Evaluating the Model

- **Neurons, Layers, and Activation Functions:**
  - For the final optimized model, four hidden layers were used, all with ReLU activation (`activation='relu'`). The layers had 80, 30, 20, and 10 nodes, respectively. This choice was based on experimentation, where the accuracy improved in the final optimization to 78.4%.

- **Achievement of Target Model Performance:**
  - Yes, specifically after including the `NAME` feature for training the model.

- **Steps to Increase Model Performance:**
  - Initially, the cutoff points for the `APPLICATION_TYPE` and `CLASSIFICATION` features were changed to 1000 and 2000, respectively. The number of nodes and layers were altered as well. The accuracy further improved to 78.4% when including the `NAME` feature.

## Summary

This deep learning model using neural networks was developed with the TensorFlow library based on Keras and achieved an accuracy of 78.4%. While effective, an alternative approach using a Random Forest Classifier could be considered. It might require less optimization and potentially offer higher accuracy, although with the potential risk of overfitting.







