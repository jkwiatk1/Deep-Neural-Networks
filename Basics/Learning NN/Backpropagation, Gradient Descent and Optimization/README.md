
# Forward propagation
Forward propagation is the process of sending each sample through the neural network and obtaining the value of the prediction. It does this for all samples and collects a set of predictions. Then, It compares the predictions with the actual outputs in order to obtain the error rates.

In essence, this phase encompasses two primary steps:
1. Calculating the predictions.
2. Calculating the error rates.

# Backpropagation
Based on the output values and the expected results, errors are calculated for the output layer. These errors are measured by the difference between the predicted and expected values.

Then, the errors are propagated backward through the hidden layers. For each layer, the error is calculated as the product of the error from the previous layer and the derivative of the activation function applied to the inputs at that layer. This process of error propagation allows the weights to be adjusted in order to minimize the overall error.

Finally, the weights and biases are updated based on the calculated gradients and learning rate using specific optimization formulas:
* weights -= learning_rate * gradient
* bias -= learning_rate * gradient_bias


Based on:
* https://medium.com/@ja_adimi/neural-networks-101-a-gentle-introduction-3caf9c99e23f