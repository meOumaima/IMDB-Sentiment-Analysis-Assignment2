LSTM Model – Sentiment Analysis:

- This model uses a Long Short-Term Memory (LSTM) network to classify IMDB movie reviews as positive or negative. It improves over the MLP by capturing sequential patterns in text.

- Model Architecture:
-> Embedding Layer: 10,000 vocabulary, 100-dim embeddings
-> LSTM Layer: 128 hidden units, batch_first=True
-> Fully Connected Layer: 1 neuron
-> Activation: Sigmoid
-> Loss Function: Binary Cross-Entropy
-> Optimizer: Adam (learning rate = 0.001)

- Techniques Applied:
-> Text preprocessing (lowercasing, HTML removal, extra space removal)
-> Tokenization and padding to uniform length
-> Feature learning via LSTM embeddings (sequence modeling)
-> Regularization: None currently (can add dropout for further improvement)
-> Hyperparameter tuning: hidden dimension, embedding size, learning rate

- Analysis:
-> The LSTM model achieved 87.86% test accuracy, outperforming the improved MLP (~77.78%).
-> Training accuracy reached 100%, indicating overfitting.
-> Validation and test accuracy (~87.7%) show reasonable generalization.
-> The model effectively captures word order and contextual relationships, improving over sentence-level polarity features.
-> Potential improvements include adding dropout, using pretrained embeddings, bidirectional LSTMs, and early stopping (this will be our next model).