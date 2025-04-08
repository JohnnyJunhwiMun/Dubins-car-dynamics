# Dubins Car Dynamics Simulation & Neural Network Predictions

## Overview

This project demonstrates a simulation of the Dubins car dynamics along with a comparison of its trajectory against predictions made by a pre-trained neural network. The Dubins car model is commonly used in path planning and optimal path problems; it represents a simplified vehicle with state variables for position \((x, y)\) and heading angle \(\theta\).

---

## Main Features

- **Dubins Car Dynamics Simulation:**  
  Computes the vehicle's motion over time using the standard Dubins car differential equations:
  
  - dx/dt = u · cos(θ)
  - dy/dt = u · sin(θ)
  - dθ/dt = w
  
  Here, _u_ is the linear velocity (often assumed constant) and _w_ is the angular velocity.

- **Neural Network Predictions:**  
  Utilizes a pre-trained neural network to predict the vehicle's trajectory starting from the same initial state.

- **Visualization and Comparison:**  
  Uses Matplotlib to visualize and compare both the actual dynamics and the neural network predictions.

- **GPU Support:**  
  Designed to run in environments with GPU support (e.g., Google Colab with a T4 GPU), which can help speed up computation and simulation.

---
