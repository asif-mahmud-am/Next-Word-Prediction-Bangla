# An RNN based Approach to Predict Next Word in Bangla Language 

The communication paradigm has changed with time, and text messaging has incredibly increased among people of all aspects. In addition, people use email and social media sites for interactive communication. As a result, people spend a significant amount of time typing the entire content, which is repetitious and time-killing. Therefore, word prediction technologies have been introduced to make message exchange faster and easier for predicting the next most probable word, allowing participants to choose it from a list of recommended words rather than entering it. This paper suggests a technique that predicts the next most relevant and acceptable word in Bangla, the eighth most speaking language in the world. We applied two Recurrent Neural Network models named Bi-directional LSTM (Long Short-Term Memory) and Bi-directional GRU (Gated Recurrent Unit) as language development models to our data set, which is compiled from different Bangla newspapers, storybooks, and Bangla Wikipedia. We also applied different n-grams with different LSTMs, and our approach found a maximum accuracy of 99.43% for a 5-gram dataset using the Bi-LSTM model. 

## Dataset 

We have collected our data from several data sources including bangla newspapers, wikipedia and story books. 

Distribution: 

```
Bangla Newspapers (BBC News, Prothom Alo) - 40500
Bangla Wikipedia - 13800
Bangla Story Books - 28500
```
Our original dataset can be found here and also in kaggle. 

Link to kaggle: [original-dataset](https://www.kaggle.com/datasets/asifmahmudcste/next-word-prediction-bangla?select=original+dataset.txt) 

## Tokenized dataset 

We have tokenized our dataset and created 5 datasets out of them. We have used n-gram techniques (unigram, bigram, tri-gram, 4-gram and 5-gram) to tokenize our dataset for next word prediction task. 

The tokenized datasets are also available in this repo and kaggle. 

Link to kaggle: [tokenized-datasets] (https://www.kaggle.com/datasets/asifmahmudcste/next-word-prediction-bangla) 

## Models 

We have trained several RNN models and compared the results. 

Models trained:

1. LSTM
2. GRU
3. Bi-LSTM 
4. Bi-GRU 

We have tried out a total of 20 combinations to see which combination gives the best performance. 

LSTM was trained on unigram, bi-gram, tri-gram, 4-gram and 5-gram dataset. Accordingly, other 3 models were trained on this dataset too. 

## Result 

| Models | Accuracy
| :----------- | :----------- |
Bi-LSTM with 5-gram | 99.43%
Bi-LSTM with 4-gram | 98.69%
LSTM with 5-gram | 98.58%
Bi-GRU with 5-gram | 98.54%
GRU with 5-gram | 98.40% 

## Paper 

We have also published a paper on our work. 

Read the paper here: [An RNN based Approach to Predict Next Word in Bangla Language](https://link.springer.com/chapter/10.1007/978-3-031-34619-4_43)