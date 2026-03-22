LSTM Improved Model – Sentiment Analysis:

- This model is an improved version of the basic LSTM model. It enhances performance and generalization by applying regularization techniques and improving the architecture to reduce overfitting.

- Model Architecture:
-> Embedding Layer: 10,000 vocabulary, 100-dim embeddings
-> LSTM Layer: 128 hidden units, batch_first=True
-> Dropout Layer: applied to reduce overfitting
-> Fully Connected Layer: 1 neuron
-> Activation: Sigmoid
-> Loss Function: Binary Cross-Entropy
-> Optimizer: Adam (learning rate = 0.001)

- Techniques Applied:
-> Text preprocessing (lowercasing, HTML tag removal, extra space cleaning)
-> Tokenization and padding to fixed sequence length
-> Sequence modeling using LSTM (captures word order and context)
-> Regularization using Dropout to reduce overfitting
-> Hyperparameter tuning:
    . Optimized hidden dimension size
    . Adjusted batch size
    . Improved training stability

- Analysis:
-> The improved LSTM achieved 88.60% test accuracy, slightly improving over the base LSTM (87.86%).
-> Training accuracy decreased from 100% to ~90.5%, indicating reduced overfitting.
-> Validation and test accuracy (~88.3%–88.6%) are very close, showing good generalization.
-> The model successfully captures contextual information in text, outperforming both the baseline and improved MLP models.
-> Applying dropout improved generalization and made the model more robust.
