# Sentiment-Analysis-Using-Natural-Language-Processing
Data: The IMDb dataset contains movie reviews that are pre-encoded as sequences of integers, where each integer represents a word.

We restrict the vocabulary to the top 10,000 most frequent words.
Reviews are padded or truncated to ensure uniform length.
Model:

Embedding layer: Converts words into dense vectors of fixed size.
Bidirectional LSTM: A recurrent layer that reads sequences forward and backward, helping capture context better.
Dense layer: Learns non-linear combinations of features.
Output layer: Uses a sigmoid activation for binary classification (positive or negative sentiment).
Training:

We use the Adam optimizer and binary cross-entropy loss, which is suitable for binary classification tasks.
Evaluation: After training, we evaluate the model's performance on the test set and visualize the accuracy and loss curves.

Adjustments:
Hyperparameters: You can change the number of epochs, batch size, and LSTM units to tune the model's performance.
Data Augmentation: You can experiment with more complex preprocessing, such as handling stop words or using pre-trained word embeddings like GloVe or Word2Vec for the embedding layer.
