**Gradient descent:**

- Gradient descent is an optimization algorithm for finding a local minimum of a differentiable function which is commonly-used to train machine learning models and neural networks.
- Each time we find the gradient and update the values of weights and biases, we move closer to the optimum value. 

![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/4574e431-3b9c-4bc0-bba7-e004537dcf55)

![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/014ced4b-d50a-4525-a13a-0dd6e46c912f)

__Learning Rate:__

- Learning rate is probably the most important aspect of gradient descent and also other optimizers as well.
- With a large learning rate, you will never be able to converge to the global minima and will always wander around the global minima.
- If you choose a small value as learning rate, you lose the risk of overshooting the minima but your algorithm will longer time to converge,
  i.e you take shorter steps but you have to take more number of steps.
- 

  ![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/38056dfe-25d0-4e42-8a20-f32f66bdae6c)


**Types of gradient descent:**

__1. Momentum based gradient descent:__
- Gradient descent optimization algorithm variant that adds a momentum term to the update rule.
- The momentum term is computed as a moving average of the past gradients, and the weight of the past gradients is controlled by a hyperparameter called Beta.
- If gradient is high, move slow otherwise if gradient is low, move fast.
- This will ensure faster convergence.
- It may require some  U turns ( overshoot the minimum).

  ![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/9b49b2a5-71f2-4a70-bdce-b3c6aad6bb98)

  ![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/58763f97-e783-405d-afb1-48e8c0a160af)

__2. Nesterov gradient descent:__
- Use the gradient at the next update point (look ahead point).
- If there is change in direction change then algorithm presumes that it should go to previous point and then update it again.
- This can lead to faster convergence by having smaller oscillating U-turns.

   ![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/f903bebd-7266-42c8-81ed-d30c9dd9103e)

   ![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/2b7bab91-684c-4eaa-ba47-2df51da8e58f)

 __3. RMSprop (Root Mean Squared Propagation) Optimizer:__
- An extension of gradient descent that uses a decaying average of partial gradients in the adaptation of the step size for each parameter. 
- For sparse data, use the number of updates as the parameter.
- RMSprop deals with the above issue by using a moving average of squared gradients to normalize the gradient.
- This normalization balances the step size (momentum), decreasing the step for large gradients to avoid exploding and
  increasing the step for small gradients to avoid vanishing.
- RMSprop Update rule:

 ![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/eb8cf764-cf3f-4360-b383-fab495fe2ca6)


 __4. ADAM ( Adaptive momentum) Optimizer:__
 - Adam is an optimization algorithm that can be used instead of the classical stochastic gradient descent procedure
   to update network weights iterative based in training data.
- Instead of adapting the parameter learning rates based on the average first moment (the mean) as in RMSProp,
  Adam also makes use of the average of the second moments of the gradients (the uncentered variance). 
- Adam update rule:

  ![image](https://github.com/fti-vsaxena/computer-vision/assets/94839845/18480173-12f1-4b6f-a725-9bea8c1c798d)

