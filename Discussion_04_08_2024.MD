## Contents

### Is the non linear component a mandate/is it necessary?

No, it is not necessary. "Activation=linear" is effectively implying there is no non-linearity introduced in the last layer.

### Jacobian

Defined for an entire layer, and its weights

#### Homework

Work on the Reuters dataset.
Try using NLP concepts on this dataset
SMOTE for Imbalanced classes- to maintain a similar distribytion of classes in training and testing/validation/both datasets.

### Things to remember (and recommended) while using Keras:-

- Saving the model
- Callbacks
  - Model Checkpoint
  - Early Stopping
  - Plotting model parameters

| Type of problem       | Last Layer  | Loss         |
| --------------------- | ----------- | ------------ |
| Binary Classification | Sigmoid     | BCE          |
| Multiclass            | Softmax     | CCE          |
| Multilabel            | Sigmoid     | BCE          |
| Regression            | Linear/None | MAE/MSE/RMSE |
| Regression -> [0, 1]  | Sigmoid     | MAE/MSE/RMSE |

3 main ways to overfit a model on data:-

- Increase epochs
- Increase model layer
- Increase neurons

(Why overfit? Because overfitting followed by generalisation is how the tradeoff is generally done.)

### Regularisation:-

- L1 & L2 Penalty
- Dropout
- Batch Normalisation
- Reduce Complexity

### Hyperparameter Tuning

- Training Process

  - Optimiser
  - Learning Rate
  - Epochs
  - Batch Size
  - Data (Validation folds, test size etc)

- Model Architecture
  - Activation
  - Dropout
  - Layer size, Number of neurons

### In context of neural network:-

- CV (Grid, Random etc)
- Hyperopt (Talos, Hyperas, Kopt)
- Keras Tuner

### Optimisers

- SGD (basic, simple Gradient Descent)
- "Momentum"
- Nesterov Accelerated Gradient: "Where I think I have to go minus where I must"

#### Note

Learning rate is not the step size, but infact scales the step.

[Source to the optimiser blog](https://www.ruder.io/optimizing-gradient-descent/#momentum)
