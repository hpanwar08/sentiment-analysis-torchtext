# Sentiment Analysis in Torch Text
Sentiment analysis is a classification task where each sample is assigned a positive or negative label.

This repo contains the code for the this [blog](https://medium.com/@sonicboom8/sentiment-analysis-torchtext-55fb57b1fab8).

## Typical components of classification task in NLP
1. Preprocessing and tokenization
2. Generating vocabulary of unique tokens and converting words to indices
3. Loading pretrained vectors e.g. Glove, Word2vec, Fasttext
4. Padding text with zeros in case of variable lengths
5. Dataloading and batching
6. Model creation and training

## Why use torchtext
Torchtext provide set of classes that are useful in NLP tasks. These classes takes care of first 5 points above with very minimal code.

## Prerequisites
* [Pytorch 0.4](http://pytorch.org/)
* [TorchText 0.2.3](https://github.com/pytorch/text)
* Understanding of GRU/LSTM [1]

## What is covered in the [notebook](Sentiment%20analysis%20pytorch.ipynb)

1. Train validation split
2. Define how to process data
3. Create torchtext dataset
4. Load pretrained word vectors and building vocabulary
5. Loading the data in batches
6. Simple GRU model
6. GRU model with concat pooling
7. Training


## Data Overview

![Top 5 rows of dataset](data/imgs/dfhead.png "Top 5 rows of dataset")

## Concat Pooling model architecture [2]
![GRU model with concat pooling](data/imgs/Slide2.JPG "GRU model with concat pooling")

## References
[1] https://colah.github.io/posts/2015-08-Understanding-LSTMs/  
[2] https://arxiv.org/abs/1801.06146
