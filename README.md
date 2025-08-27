model choice and justififcation:  

LSTMs are a type of recurrent neural network (RNN) that are particularly well-suited for processing sequential data like text.
Here's the justification:

Handling Sequential Data: Movie reviews are sequences of words. The order of words is important for understanding the sentiment (e.g., "this movie was not good" has a different sentiment than "this movie was good"). LSTMs are designed to capture these dependencies in sequential data.
Capturing Long-Range Dependencies: LSTMs have a memory mechanism that allows them to retain information from earlier parts of the sequence, which is crucial for understanding the overall sentiment of a review, especially for longer reviews.
Common for Text Classification: LSTMs are a standard and effective architecture for various natural language processing tasks, including sentiment analysis.
The model architecture includes:

Embedding Layer: This layer converts words into dense vectors, allowing the model to represent words in a continuous space and capture semantic relationships.
LSTM Layer: This is the core layer that processes the sequence of word embeddings and learns to identify patterns related to sentiment.
Dense Layer: This is the output layer with a sigmoid activation function, which is suitable for binary classification (positive or negative sentiment).

result explaination ; - 

The output shows the training and validation accuracy for each epoch during the training process.

Training Accuracy: This is the accuracy of the model on the data it was trained on. You can see that the training accuracy generally increases with each epoch, indicating that the model is learning to classify the sentiment of the reviews.
Validation Accuracy: This is the accuracy of the model on a portion of the training data that was held out during training. This gives an indication of how well the model generalizes to unseen data. You can see that the validation accuracy fluctuates a bit, but stays relatively high, suggesting that the model is not significantly overfitting to the training data.
The goal is to have both high training and validation accuracy, with the validation accuracy being close to the training accuracy.
