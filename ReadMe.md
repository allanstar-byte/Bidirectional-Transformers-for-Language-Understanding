# Bidirectional Transformers for Language Understanding

To implement this papaer the first stepo will be vision alignment. 

This will mainly onclude skimming through the paper to understand the scope of the paper; the terminologies used.

Skimming will be according to the chapters from the abstract to the final bits of the paper.

## Abstract

What is BERT?  is a transformer-based machine learning technique for natural language processing (NLP) pre-training developed by Google. 

What do we mean by "a transformer-based machine learning technique" - A transformer is a deep learning model that adopts the mechanism of self-attention, differentially weighting the significance of each part of the input data. It is used primarily in the fields of natural language processing (NLP) and computer vision (CV).

Let's breakdown further the BERT terminology

    1. Bidirectional - Bidirectional long-short term memory(Bidirectional LSTM) is the process of making any neural network to have the sequence information in both directions backwards (future to past) or forward(past to future.

    2. Encoder - This is a stack of several recurrent units (LSTM or GRU - (A gated recurrent unit (GRU) is part of a specific model of recurrent neural network that intends to use connections through a sequence of nodes to perform machine learning tasks associated with memory and clustering) cells for better performance) where each accepts a single element of the input sequence, collects information for that element and propagates it forward.

    3. Representations - This is a set of techniques that allows a system to automatically discover the representations needed for feature detection or classification from raw data.

    4. Transformers - These are objects that transform a dataset into a new one to prepare the dataset for predictive modeling

BERT model can be fine tuned with just one additional output layer to create state-of-the-art models for a wide
range of tasks, such as question answering and language inference, without substantial tasks pecific architecture modifications. 

In this case the State-of-the-art models (SOTA) are  DNN best models that you can use for any particular task.

Where inference is the process of running data points into a machine learning model to calculate an output such as a single numerical score.


BERT is conceptually simple and empirically powerful. By empirically power1ful we mean  based on evidence or observations from the data points.

It obtains new state-of-the-art results on eleven natural language processing tasks , including:

            a.  pushing the GLUE score to 80.5% - General Language Understanding Evaluation

We can dig a bit more deeper to understand this GLUE thing, 

GLUE - On a high level is a collection of resources for training, evaluating, and analyzing natural language understanding systems. Glue Consists of:

- A benchmark of nine sentence- or sentence-pair language understanding tasks built on established existing datasets and selected to cover a diverse range of dataset sizes, text genres, and degrees of difficulty,

-  A diagnostic dataset designed to evaluate and analyze model performance with respect to a wide range of linguistic phenomena found in natural language, and

- A public leaderboard for tracking performance on the benchmark and a dashboard for visualizing the performance of models on the diagnostic set.

            b. MultiNLI accuracy to 86.7% - Multi-Genre Natural Language Inference

We can dig a bit more deeper to understand this MultiNLI thing,

MultiNLI corpus is a crowd-sourced collection of 433k sentence pairs annotated with textual entailment information. MultiNLI 0.9 differs from MultiNLI 1.0 only in the pairID and promptID fields in the training.

            c. SQuAD v1.1 question answering Test F1 to 93.2 
