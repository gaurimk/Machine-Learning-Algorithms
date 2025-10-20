📘 Overview

Gradient Descent is an optimization algorithm used to minimize the cost (or loss) function in machine learning models. It iteratively adjusts the model parameters in the direction of the steepest descent of the cost function to reach the global minimum.

⚙️ Working Principle

Initialize Parameters:
Start with random values for model parameters (weights and bias).

Compute Predictions:
Use current parameters to make predictions on the data.

Calculate Cost Function:
Evaluate how far the predictions are from actual values (e.g., Mean Squared Error).

Compute Gradients:
Find the derivative of the cost function with respect to each parameter.

Update Parameters:
Adjust parameters using the formula:

𝜃
:
=
𝜃
−
𝛼
∂
𝐽
(
𝜃
)
∂
𝜃
θ:=θ−α
∂θ
∂J(θ)
	​


where

𝜃
θ: parameter (weight/bias)

𝛼
α: learning rate

𝐽
(
𝜃
)
J(θ): cost function

Repeat:
Continue until the cost function converges or a maximum number of iterations is reached.
