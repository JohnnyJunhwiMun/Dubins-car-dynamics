# Dubins Car Dynamics Simulation & Fully Connected Neural Network


This project demonstrates a discrete-time simulation of the Dubins car, a simplified vehicle model frequently used in path planning and navigation problems. The Dubins car is characterized by its non-linear dynamics and is defined by its position and steering angle. In our simulation, the vehicle's evolution is governed by the following discrete-time model:

Let $h$ be a step size, $v$ a velocity, and $u$ a constant control. The Dubins car model (in discrete time) can be described as:

```math
  x_{t+1} = f(x_t) = \begin{bmatrix}
                        x_{t}^{(1)} + h v \sin(x_{t}^{(3)}) \\
                        x_{t}^{(2)} + h v \cos(x_{t}^{(3)}) \\
                        x_{t}^{(3)} + h u
                      \end{bmatrix}
```
  where $x_{t}^{(1)}$ represents the $x$-position of the car at instant $t$, $x_{t}^{(2)}$ the $y$-position, and $x_{t}^{(3)}$ is its steering angle. Note that this dynamics is non-linear.

- **Neural Network Predictions:**  
  Utilizes a pre-trained neural network to predict the vehicle's trajectory starting from the same initial state.

- **Visualization and Comparison:**  
  Uses Matplotlib to visualize and compare both the actual dynamics and the neural network predictions.

- **GPU Support:**  
  Designed to run in environments with GPU support (e.g., Google Colab with a T4 GPU), which can help speed up computation and simulation.

---
