# Shap_interpretabilidade

# Interpreting Text Classification with SHAP

This repository contains a Python script for interpreting text classification using SHAP (SHapley Additive exPlanations). The code demonstrates how to train a text classification model, explain model predictions, and visualize the Shapley values using SHAP.

## Getting Started

To get started, you need to have Python installed and install the required packages. You can use the following command to install the necessary packages:

```bash
pip install shap scikit-learn

Data Description
The IMDB movie review dataset is used in this example. It contains movie reviews labeled as positive or negative. The dataset is loaded and split into training and testing sets using the train_test_split function.

Text Vectorization
Text data is vectorized using the Term Frequency-Inverse Document Frequency (TF-IDF) vectorizer from scikit-learn. The vectorized data is used for training a Logistic Regression text classification model.

Model Training
A Logistic Regression classifier is trained on the vectorized text data using scikit-learn. The model is used to make predictions on the testing data.

SHAP Explanation
SHAP is used to explain the model's predictions. The SHAP Explainer is initialized with the trained model and the training data. SHapley values are calculated for the testing data using the explainer.

SHAP Visualization
SHAP provides various visualization methods for Shapley values. In this code, a beeswarm plot is used to visualize the Shapley values. The plot shows the impact of each feature on the model's predictions.

Conclusion
This repository provides an example of using SHAP to interpret a text classification model. You can adapt this code for your own text classification tasks and explore the influence of features on model predictions.

License
This project is licensed under the MIT License - see the LICENSE file for details.
