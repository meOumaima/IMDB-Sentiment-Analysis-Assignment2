Improved MLP Model – Sentiment Analysis:

- This model is an improved version of the baseline Multi-Layer Perceptron (MLP) developed in Assignment 1. The goal is to enhance performance by adding new features and applying optimization techniques.

- Model Architecture:
-> Input Layer: 5 features
      . VADER polarity score
      . TextBlob polarity score
      . Hybrid polarity score (average)
      . Review length
      . Word count
-> Hidden Layer 1: 32 neurons (ReLU activation)
-> Hidden Layer 2: 16 neurons (ReLU activation)
-> Dropout Layer: 0.3 (to reduce overfitting)
-> Output Layer: 1 neuron (Sigmoid activation)
-> Loss Function: Binary Cross-Entropy
-> Optimizer: Adam (learning rate = 0.0005)

- Techniques Applied:
-> Text preprocessing (lowercasing, HTML removal, extra space removal)
-> Feature engineering using:
      . VADER sentiment scores
      . TextBlob sentiment scores
      . Hybrid sentiment score
      . Additional features: review length and word count
-> Feature scaling using StandardScaler (for new features)
-> Hyperparameter tuning:
      . Increased hidden layer sizes
      . Reduced learning rate
-> Regularization using Dropout

- Analysis:
-> The improved model slightly outperforms the baseline MLP.
-> Feature scaling played an important role in stabilizing performance.
-> The model generalizes well, as shown by similar performance across training, validation, and test sets.
-> However, performance improvements remain limited due to reliance on sentence-level polarity features.