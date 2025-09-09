# Mathematical Foundations

## Overview

Understanding the mathematical foundations is crucial for working with neural networks. This section covers the essential mathematical concepts you'll need throughout the course.

## Linear Algebra

### Vectors and Matrices

Neural networks heavily rely on vector and matrix operations:

**Vector Operations:**
- Dot product: $\mathbf{a} \cdot \mathbf{b} = \sum_{i=1}^n a_i b_i$
- Vector norm: $\|\mathbf{a}\| = \sqrt{\sum_{i=1}^n a_i^2}$

**Matrix Operations:**
- Matrix multiplication: $(AB)_{ij} = \sum_{k=1}^n A_{ik} B_{kj}$
- Matrix transpose: $(A^T)_{ij} = A_{ji}$

### Key Concepts

!!! info "Matrix Dimensions"
    When multiplying matrices A (m×n) and B (n×p), the result is a matrix C (m×p). The inner dimensions must match!

## Calculus

### Derivatives

Derivatives are essential for optimization in neural networks:

**Single Variable:**
$$f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$

**Partial Derivatives:**
$$\frac{\partial f}{\partial x} = \lim_{h \to 0} \frac{f(x+h, y) - f(x, y)}{h}$$

### Chain Rule

The chain rule is fundamental to backpropagation:

$$\frac{d}{dx}[f(g(x))] = f'(g(x)) \cdot g'(x)$$

**Multivariable Chain Rule:**
$$\frac{\partial z}{\partial x} = \frac{\partial z}{\partial y} \cdot \frac{\partial y}{\partial x}$$

## Probability and Statistics

### Probability Distributions

**Normal Distribution:**
$$f(x) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}$$

Where $\mu$ is the mean and $\sigma$ is the standard deviation.

### Bayes' Theorem

$$P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$$

This is fundamental to probabilistic interpretations of neural network outputs.

## Optimization

### Gradient Descent

The core optimization algorithm for neural networks:

$$\theta_{new} = \theta_{old} - \alpha \nabla_\theta J(\theta)$$

Where:
- $\theta$ are the parameters
- $\alpha$ is the learning rate  
- $J(\theta)$ is the cost function
- $\nabla_\theta J(\theta)$ is the gradient

### Cost Functions

**Mean Squared Error (MSE):**
$$J(\theta) = \frac{1}{2m} \sum_{i=1}^m (h_\theta(x^{(i)}) - y^{(i)})^2$$

**Cross-Entropy Loss:**
$$J(\theta) = -\frac{1}{m} \sum_{i=1}^m [y^{(i)} \log(h_\theta(x^{(i)})) + (1-y^{(i)}) \log(1-h_\theta(x^{(i)}))]$$

## Practice Problems

!!! example "Exercise"
    Try these problems to test your understanding:
    
    1. Calculate the gradient of $f(x,y) = x^2 + 2xy + y^2$ with respect to both variables
    2. Given matrices A (2×3) and B (3×4), what are the dimensions of AB?
    3. What is the derivative of the sigmoid function $\sigma(x) = \frac{1}{1+e^{-x}}$?

??? success "Solutions"
    1. $\frac{\partial f}{\partial x} = 2x + 2y$, $\frac{\partial f}{\partial y} = 2x + 2y$
    2. AB will be 2×4
    3. $\sigma'(x) = \sigma(x)(1-\sigma(x))$

## Prerequisites Check

Before proceeding to neural networks, make sure you're comfortable with:

- [ ] Basic matrix operations
- [ ] Computing partial derivatives
- [ ] Understanding the chain rule
- [ ] Basic probability concepts
- [ ] Optimization concepts

## Next Steps

With these mathematical foundations, you're ready to explore:
- [Neural Networks Basics](../neural-networks/main.md)
- [Laboratory Exercises](../../exercises/index.md)

## Additional Resources

- **Linear Algebra**: Khan Academy Linear Algebra course
- **Calculus**: MIT OpenCourseWare 18.01
- **Probability**: Introduction to Statistical Learning
- **Optimization**: Boyd & Vandenberghe Convex Optimization