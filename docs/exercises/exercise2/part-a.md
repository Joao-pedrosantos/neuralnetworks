# Exercise 2: Perceptron Implementation

## Notebook

!!! jupyter "Interactive Exercise"
    Here's the complete notebook.

    [:material-notebook: Open Exercise 1A Notebook](https://nbviewer.org/github/joao-pedrosantos/neuralnetworks/blob/main/docs/exercises/exercise2/exercise1.ipynb){ .md-button .md-button--primary }

    [:material-github: View Source on GitHub](https://github.com/joao-pedrosantos/neuralnetworks/blob/main/docs/exercises/exercise2/exercise1.ipynb){ .md-button }


## Conclusion

In this exercise, I implemented a simple perceptron model that was trained on a synthetic dataset. 

In the first part, the classes were visibly separable. That made it so that the perceptron could easily and quickly learn to classify the data points correctly and set a decision boundary that separated the two classes. It ended up taking 22 epochs to converge in a final accuracy of 100%. This shows that the perceptron is effective for linearly separable data.

These are the final metrics for the first part:

```
Final Weights: [ 0.03687651 0.04482725] Bias: -0.2700000000000001
Final Accuracy: 1.0
Epochs to Converge: 22
```

However, in the second part, the classes were not linearly separable. This made it impossible for the perceptron to find a decision boundary that could separate the two classes correctly. As a result, the perceptron struggled to learn and only achieved a final accuracy of 50.1%. This highlights the limitation of the perceptron model when dealing with non-linearly separable data. That means that more complex models, such as multi-layer neural networks, are needed to handle such cases effectively.

These are the final metrics for the second part:

```
Final Weights: [0.03975727 0.03749485] Bias: -0.060000000000000005
Final Accuracy: 0.5015
Epochs to Converge (Didn't Converge, so Max Epochs): 100
```
