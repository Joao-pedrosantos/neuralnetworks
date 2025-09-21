# Exercise #: Multi Layer Perceptron Implementation

## Notebook

!!! jupyter "Interactive Exercise"
    Here's the complete notebook.

    [:material-notebook: Open Exercise 1A Notebook](https://nbviewer.org/github/joao-pedrosantos/neuralnetworks/blob/main/docs/exercises/exercise3/exercise1.ipynb){ .md-button .md-button--primary }

    [:material-github: View Source on GitHub](https://github.com/joao-pedrosantos/neuralnetworks/blob/main/docs/exercises/exercise3/exercise1.ipynb){ .md-button }


## Conclusion

In this exercise, I implemented a Multi-Layer Perceptron (MLP) model that was trained on a synthetic dataset.

During the first part of the exercise, I calculated the forward and backward passes of a simple MLP manually. This helped me understand the underlying mechanics of how data flows through the network and how gradients are computed for weight updates. It reinforced my grasp of concepts like activation functions, loss calculation, and backpropagation.

In the second part, I built an MLP from scratch using Python and NumPy. I created a network with one hidden layer and trained it on a binary classification task. The model successfully learned to classify the data, achieving high accuracy on the test set. This demonstrated the effectiveness of MLPs for solving non-linear problems.

Finally, in the third part, I extended the MLP to handle multi-class classification by modifying the architecture and using the softmax activation function in the output layer. The model was able to classify data points into three distinct classes with good accuracy. This part highlighted the versatility of MLPs in handling more complex classification tasks.


The forth and final part of the exercise involved experimenting with deeper architectures and different activation functions. I built a deeper MLP with multiple hidden layers and trained it on the same multi-class dataset. The deeper network achieved even better performance, showcasing the power of deep learning. Additionally, I observed how different activation functions impacted the training dynamics and final accuracy. I switched from 'relu' to 'tanh' and noticed that 'tanh' often led to faster convergence and better performance in deeper networks.
Overall, this exercise provided a comprehensive understanding of Multi-Layer Perceptrons, from manual calculations to practical implementations. It reinforced key concepts in neural networks and deep learning, and demonstrated the effectiveness of MLPs for both binary and multi-class classification tasks.