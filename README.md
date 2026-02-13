# Bigram-Language-Model-Python-Implementation
This project implements a Bigram Language Model using Python.
The goal is to learn bigram probabilities from a small training corpus and use them to compute the probability of test sentences. The model uses Maximum Likelihood Estimation (MLE) to estimate probabilities.

Training Corpus

The model is trained using the following sentences:

<s> I love NLP </s>
<s> I love deep learning </s>
<s> deep learning is fun </s>

Program Features

The Python program performs the following tasks:

Reads the training corpus.

Computes unigram counts (single word frequencies).

Computes bigram counts (pairs of consecutive words).

Calculates bigram probabilities using MLE:

P(w₂ | w₁) = Count(w₁,w₂) / Count(w₁)

Implements a function to compute the probability of any input sentence.

Tests the model on two sentences:

<s> I love NLP </s>

<s> I love deep learning </s>

Prints the probability of each sentence.

Displays which sentence is preferred by the language model.

How to Run the Program

Make sure Python 3 is installed.

Download or clone the repository.

Run the script:

python bigram_model.py

Expected Output

The program will display:

Unigram counts

Bigram counts

Bigram probabilities

Sentence probabilities

The preferred sentence based on higher probability

Explanation

The bigram language model assumes that the probability of a word depends only on the previous word. The model multiplies the probabilities of each bigram in a sentence to compute the final sentence probability. The sentence with the higher probability is considered more likely by the model.

Notes

The model uses MLE without smoothing.

If a bigram is not found in training data, its probability becomes zero.

This implementation is intended for educational purposes and demonstration of NLP concepts.
