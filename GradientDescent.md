**Gradient descent:**

Gradient descent is an optimization algorithm for finding a local minimum of a differentiable function which is commonly-used to train machine learning models and neural networks.

![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/4574e431-3b9c-4bc0-bba7-e004537dcf55)

![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/014ced4b-d50a-4525-a13a-0dd6e46c912f)


**Types of gradient descent:**

__1. Momentum based gradient descent:__
- If gradient is high, move slow otherwise if gradient is low, move fast.
- This will ensure faster convergence.
- It may require some  U turns ( overshoot the minimum).

![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/58763f97-e783-405d-afb1-48e8c0a160af)

__2. Nesterov gradient descent:__
- Use the gradient at the look ahead point.
- This can lead to faster convergence by having smaller oscillating U-turns.

  ![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/2b7bab91-684c-4eaa-ba47-2df51da8e58f)


