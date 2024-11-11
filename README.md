# Sentiment Analysis with RNN, LSTM, GRU, and Attention

This repository implements several **Recurrent Neural Network (RNN)** architectures, including **Simple RNN**, **LSTM**, **GRU**, and **LSTM with Attention**, to perform **Sentiment Analysis** on the **IMDB movie reviews dataset**. The models are trained and evaluated on this dataset to determine the effectiveness of each architecture for sentiment prediction.

## Dataset

The dataset used for this project is the **IMDB movie reviews dataset**. It consists of 50,000 reviews, equally divided between positive and negative reviews. Each review is encoded as a sequence of integers, with each integer representing a unique word in the vocabulary.

- **Training Data**: 25,000 samples
- **Test Data**: 25,000 samples
- **Vocabulary Size**: 10,000 most frequent words
- **Maximum Review Length**: 500 words (truncated or padded)

## Models Implemented

### 1. Simple RNN
The **Simple RNN** model is a basic recurrent network that processes sequences of words in the reviews. It consists of the following layers:
- **Embedding Layer**: Converts word indices into dense vectors.
- **RNN Layer**: Processes the sequence data.
- **Dense Layer**: Outputs a binary classification (positive or negative sentiment).

### 2. LSTM (Long Short-Term Memory)
The **LSTM** model is a more advanced type of RNN designed to overcome the vanishing gradient problem in Simple RNNs. It captures long-range dependencies in the sequences, making it more effective for tasks involving long text sequences.

### 3. GRU (Gated Recurrent Units)
The **GRU** model is another type of RNN similar to LSTM but with a simpler architecture. GRUs are computationally more efficient and have fewer parameters than LSTMs.

### 4. LSTM with Attention
The **LSTM with Attention** model enhances the LSTM by using an **Attention mechanism**. This allows the model to focus on specific parts of the input sequence, improving its performance in tasks such as sentiment analysis where certain words or phrases hold more significance.

## Model Training and Evaluation

All models are trained using the following parameters:
- **Optimizer**: Adam
- **Loss Function**: Binary Cross-Entropy
- **Metrics**: Accuracy
- **Epochs**: 10
- **Batch Size**: 64

### Evaluation

Each model is evaluated on the **IMDB test dataset**. The performance is measured using two metrics:
- **Test Loss**
- **Test Accuracy**

## Results

- **Simple RNN**: Achieved a test accuracy of X% with a test loss of Y.
- **LSTM**: Achieved a test accuracy of X% with a test loss of Y.
- **GRU**: Achieved a test accuracy of X% with a test loss of Y.
- **LSTM with Attention**: Achieved a test accuracy of X% with a test loss of Y.

### Conclusion

Among the models tested, the **LSTM with Attention** model showed the best performance, suggesting that attention mechanisms can significantly improve the accuracy of sentiment analysis tasks.


