GRU Model – Sentiment Analysis:

- This model uses a Gated Recurrent Unit (GRU) network with pretrained word embeddings to classify IMDB movie reviews.

- Model Architecture:
-> Embedding Layer: Pretrained embeddings (100/300-dim)
-> GRU Layer: 128 hidden units
-> Dropout Layer: 0.3
-> Fully Connected Layer: 1 neuron
-> Activation: Sigmoid
-> Loss Function: Binary Cross-Entropy
-> Optimizer: Adam (learning rate = 0.001)

- Techniques Applied:
-> Text preprocessing (cleaning, normalization)
-> Tokenization and sequence padding
-> Pretrained word embeddings (Word2Vec/GloVe)
-> Sequence modeling using GRU
-> Regularization using Dropout

- Analysis:
-> The model achieved 88.34% test accuracy.
-> Training accuracy (~99.8%) indicates overfitting.
-> Validation and test accuracy (~88%) show reasonable generalization.
-> The model performs well but does not outperform the improved LSTM.