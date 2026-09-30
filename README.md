# Neural-network-playground-experiments-
# Neural Network Classification Experiments

A visual exploration of neural network architectures, feature engineering, and hyperparameter tuning using [TensorFlow Playground](https://playground.tensorflow.org/).

## Experiment: Solving the Intertwined Spiral Dataset

### Key Findings
- **Challenge:** The spiral dataset is non-linearly separable and cannot be solved using simple raw inputs ($X_1, X_2$) with shallow networks.
- **Solution:** 
  - Enabled non-linear feature inputs ($X_1^2, X_2^2, X_1 X_2, \sin(X_1), \sin(X_2)$).
  - Increased network capacity to **4 Hidden Layers** (6 neurons each).
  - Removed strict **L1 regularization** to allow weights to learn intricate boundaries.
- **Results:**
  - **Test Loss:** 0.006
  - **Training Loss:** 0.000
  - Achieved full convergence in ~637 epochs.

### Replicate Experiment
You can interact with my exact trained configuration directly via [TensorFlow Playground Share Link](https://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=spiral&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=6,6,6,6&seed=0.66957&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=true&xSquared=true&ySquared=true&cosX=false&sinX=true&cosY=false&sinY=true&collectStats=false&problem=classification&initZero=false&hideText=false).
