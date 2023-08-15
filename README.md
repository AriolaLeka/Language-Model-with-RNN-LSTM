# Character-Level Language Model using Recurrent Neural Networks

This repository contains a character-level language modeling project using recurrent neural networks (RNNs). The project focuses on training an RNN language model to predict and generate text character by character. The initial code provided implements essential components to build the model and generate text, and the project is structured as follows:

## Table of Contents

- [Preliminaries and Reading Comprehension](#preliminaries-and-reading-comprehension)
- [Text Data](#text-data)
- [Dataloader/Batch Construction](#dataloaderbatch-construction)
- [Modeling, Training, and Decoding](#modeling-training-and-decoding)
- [Running Experiments Using the Initial Code](#running-experiments-using-the-initial-code)
- [Extending the Initial Code](#extending-the-initial-code)
- [Code](Code)

## Preliminaries and Reading Comprehension

In this section, you'll find an introduction to character-level language models based on recurrent neural networks (RNNs). The provided code implements the basics of an RNN language model and text generation. Your main tasks include understanding the code and answering questions related to it.

## Text Data

This section focuses on the text data used for training the language model. We use "Aesop’s Fables (A Version for Young Readers)" from Project Gutenberg as our text source.

- **Number of Characters:** [Report the number of characters]
- **Number of Unique Characters:** [Report the number of unique characters]
- **Number of Lines:** [Report the number of lines]
- **Observation:** [Mention an interesting property of the text data]

## Dataloader/Batch Construction

This section discusses how the text data is processed and chunked to enable training. It covers the construction of data batches, handling RNN states, and preparing the data for training.

- **Method get idx of class Vocabulary:** [Explain the purpose of the if branch]
- **Vocabulary Dictionaries:** [Explain the keys and values of id-to-string and string-to-id dictionaries]
- **LongTextData Statistic:** [Report the statistic obtained when calling `len`]
- **ChunkedTextData Statistic:** [Report the statistic obtained when calling `len`]

## Modeling, Training, and Decoding

Here, you'll find details about the RNN language model architecture, training loop, and text generation using the greedy decoding algorithm.

- **Detaching Hidden States:** [Explain the reason for using `.detach()` on hidden states]
- **Ignore Index in CrossEntropyLoss:** [Explain why `ignore_index=0` is used]
- **Input Shape for RNNModel:** [Provide the input shape in terms of N, B, and D]
- **Output of self.rnn:** [Describe the output shape in terms of N, B, H, and L]
- **Greedy Decoding in Training Loop:** [Explain why `complete` is called inside the training loop]

## Running Experiments Using the Initial Code

This section focuses on running experiments with the provided code. We will train an RNN language model and evaluate its perplexity and text generation quality.

1. **Modification for Perplexity:** [Describe the modification to monitor perplexity]
2. **Training an RNN Language Model:** [Specify the hyper-parameters and training setup]
3. **Evolution of Perplexity:** [Provide a plot showing the perplexity during training]
4. **Text Generation Examples:** [Show text generation examples at different training stages]

## Extending the Initial Code

In this section, we'll extend the provided code by implementing an LSTM-based language model and introducing text sampling during decoding.

1. **LSTM Language Model:** [Describe the implementation of an LSTM-based model]
2. **Training LSTM Model:** [Specify the hyper-parameters and training details]
3. **Comparison of Greedy Decoding and Sampling:** [Compare text generation methods]

## Code

To utilize the character-level language model code provided in this repository, follow these steps:

1. **Clone the Repository:**

   git clone https://github.com/AriolaLeka/Language-Model-with-RNN-LSTM.git

2. **Navigate to the Project Directory:**

   cd Language-Model-with-RNN-LSTM

3. **Run the Python Script:**

   python language model with RNN:LSTM.py
