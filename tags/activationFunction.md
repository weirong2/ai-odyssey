Activation functions are a crucial component of neural networks, playing a vital role in the process of information transmission between neurons. Here are some typical activation functions used:

### 1. **Sigmoid Function**
```math
\sigma(z) = \frac{1}{1 + e^{-z}}
```
- **Range**: \( (0, 1) \)
- **Input**: Real numbers
- **Output**: Values in the range of 0 to 1

The sigmoid function maps any real number to a value between 0 and 1. It's often used in binary classification tasks but suffers from the dying ReLU problem.

### 2. **Rectified Linear Unit (ReLU)**
```math
f(z) = \max(0, z)
```

- **Range**: \( [0, \infty) \)
- **Input**: Real numbers
- **Output**: Non-negative values

RELU is the most widely used activation function in deep neural networks. It maps all negative values to 0 and leaves positive values unchanged.

### 3. **Tanh (Hyperbolic Tangent)**
```math
tanh(z) = \frac{e^{z} - e^{-z}}{e^{z} + e^{-z}}
```
- **Range**: \( (-1, 1) \)
- **Input**: Real numbers
- **Output**: Values in the range of -1 to 1

The tanh function maps any real number to a value between -1 and 1.

### 4. **Softmax Function**
```math
softmax(z_i) = \frac{e^{z_i}}{\sum e^{z_j}}
```

- **Range**: \( [0, 1] \)
- **Input**: Real numbers
- **Output**: Probabilities in the range of 0 to 1

The softmax function is used for multi-class classification tasks and maps any real number to a value between 0 and 1.

### 5. **Swish Activation Function**
```math
swish(x) = x \cdot sigmoid(\beta \cdot x)
```

- **Range**: \( [0, \infty) \)
- **Input**: Real numbers
- **Output**: Non-negative values

The Swish activation function is designed to improve the performance of ReLU by learning a non-linear activation function.

### Activation Functions in Practice

Each type of activation function has its strengths and weaknesses. The choice of activation function usually depends on the problem you're trying to solve:

*   For classification problems, use Sigmoid or Softmax.
*   For regression problems, use ReLU or Tanh.
*   If you have a large dataset with many neurons in the hidden layers, consider using Swish as it can lead to better performance.

The choice of activation function also depends on your computational resources. Some activation functions are more computationally expensive than others during training and inference.

Choosing the right activation function is crucial for the successful development of deep neural networks.