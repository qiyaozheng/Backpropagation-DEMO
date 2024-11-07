# Backpropagation DEMO

This project demonstrates the implementation and analysis of a simple neural network trained using backpropagation. The goal is to explore how different activation functions and network structures influence the model’s ability to learn various data patterns.

## Project Overview

The Backpropagation DEMO includes:
- A neural network with a single hidden layer.
- Experiments with different activation functions: **Sigmoid**, **Tanh**, and **ReLU**.
- Analysis of the network’s performance on different patterns, including **Diamond Pattern**, **Thin Right Angle Pattern**, and the challenging **Ring Pattern**.

## Purpose of This Notebook
This notebook was created during my own study of backpropagation. The primary goal was to deepen my understanding of how backpropagation works and to explore the differences between various activation functions. Additionally, I experimented with a total of **eight different patterns** to observe the varying levels of difficulty the network faces when learning each pattern.

## Key Findings

1. **Effectiveness of the Sigmoid Activation Function**:
   - The Sigmoid function was well-suited for binary classification tasks, achieving high accuracy (0.98–0.99) on simpler patterns like the Diamond and Thin Right Angle patterns.
   - Its effectiveness can be attributed to the compatibility between the data distribution and network structure, allowing stable gradient updates.

2. **Challenges with the Ring Pattern**:
   - The network struggled to learn the Ring pattern, with a maximum accuracy of 0.734 across all tested activation functions.
   - The Ring pattern's complex and highly non-linear nature demands a more sophisticated network capable of capturing intricate boundaries.
   - Both Sigmoid and Tanh had limited effectiveness due to small gradients near boundary regions, while ReLU, better suited for linear separations, also struggled with this pattern.

## Proposed Solutions

- **Increasing Network Complexity**: Adding more hidden layers or neurons to enable the extraction of more complex features.
- **Exploring Advanced Activation Functions**: Using activation functions better suited for highly non-linear patterns may improve learning performance.

## Conclusion

This Backpropagation DEMO provides insights into how neural networks learn and the importance of choosing suitable activation functions and network architectures. While simple networks can handle straightforward patterns well, more complex patterns require additional network capacity and feature extraction capabilities.

### Prerequisites
- Python 3.x
- Libraries: `numpy`, `matplotlib`
