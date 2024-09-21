# SVM Classifier Optimization and Analysis

This repository contains the code and analysis for optimizing an SVM (Support Vector Machine) classifier using cross-validation. The goal is to find the best parameters (C and kernel) to improve model performance and ensure its efficiency in terms of accuracy and execution time.

Project Overview
We applied a grid search with cross-validation to find the best hyperparameters for the SVM classifier. The objective was to optimize both model accuracy and execution time, taking into consideration business requirements for fast predictions with acceptable accuracy.

Best Model Results
Best Parameters: C = 0.1, kernel = 'linear'
Accuracy: 80.44% on the test set
Execution Time: 3 minutes 36 seconds
While the above model gave the best accuracy, for efficiency purposes, we also considered another model ranked 5th:

Alternative Parameters: C = 20.0, kernel = 'rbf'
Accuracy: 78.47%
Execution Time: 1.4 seconds
Model Performance Metrics
Confusion Matrix: Shows the correct classification of classes with some misclassifications.
Classification Report:
Precision: Ratio of true positives to total predicted positives.
Recall: Ratio of true positives to total actual positives.
F1-Score: Harmonic mean of precision and recall.
Business Interpretation
From a business perspective, the following conclusions were drawn:

Accuracy: The model achieved 75% accuracy in making correct decisions, which is critical for automating decision processes.
Cost Reduction: With accurate classifications, the model helps reduce costs related to incorrect decisions, such as customer churn or resource misallocation.
Business Impact: Using a linear kernel indicates that the problem is relatively simple, allowing for faster and more interpretable decisions, beneficial for stakeholders.
Sustainability: The regularization parameter C = 20.0 ensures that the model is not overfitted and can generalize well to new data.
