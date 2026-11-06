# Customer Churn Prediction (ANN)

This project uses an Artificial Neural Network (ANN) built with TensorFlow/Keras to predict whether a bank customer will churn (leave the bank).

## Dataset
The dataset contains 10,000 records of bank customers with features like Credit Score, Geography, Age, Balance, and Estimated Salary.

## Approach
*   **Preprocessing:** Label Encoding for Gender, One-Hot Encoding for Geography, and StandardScaler for feature scaling.
*   **Architecture:** A Sequential model with two hidden layers (6 neurons each, ReLU activation) and an output layer (1 neuron, Sigmoid activation).
*   **Compilation:** Adam optimizer and Binary Crossentropy loss.
*   **Training:** 100 epochs with a batch size of 32.

## Results
The model achieved an overall accuracy of **86.35%**. 
Analysis of the confusion matrix revealed a high number of False Negatives (227), indicating that the imbalanced nature of the dataset made it difficult for the model to catch all churning customers. 