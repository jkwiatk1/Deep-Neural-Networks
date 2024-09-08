# Measuring Accuracy and Error
Error computation in neural networks involves two key concepts: the loss function and the cost function. 

The loss function measures the error for a single training example, while the cost function measures the average error across the entire training set. 

While the terms are often used interchangeably, the cost function provides a more comprehensive assessment of the model’s performance by considering the overall error across multiple samples.

The most common cost functions for neural networks:
## Cost functions for regression problems
* Mean Squared Error (MSE): MSE measures the average squared difference between the predicted values and the actual values.
* Mean Absolute Error (MAE): MAE measures the average absolute difference between the predicted values and the actual values. It is less sensitive to outliers than MSE.
* Root Mean Squared Error (RMSE): RMSE is the square root of MSE. It is often used in the context of predicting continuous values, such as house prices or stock prices.

## Cost functions for classification problems
* Binary Cross-Entropy (BCE): BCE is used for binary classification problems, where there are only two possible outcomes. It measures the probability of an incorrect classification.
* Categorical Cross-Entropy (CCE): CCE is used for multi-class classification problems, where there are more than two possible outcomes. It is a generalization of BCE.
* Hinge Loss: Hinge loss is used for maximum margin classification problems, such as support vector machines (SVMs). It measures the margin between the correct classification and the incorrect classification.