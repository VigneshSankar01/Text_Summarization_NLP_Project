# Natural Language Processing: A Comparative study of LSTM, BiLSTM and Transformer Models for Text Summarization

This repository contains code for a LSTM, BiLSTM, Transfomer Model and a hybrid LSTM-transformer model designed for text summarization using the BBC News Summary dataset to generate concise summaries from news articles.

## Dataset

The BBC News Summary dataset is used for training and evaluation. It contains news articles and their corresponding summaries across various categories such as business, entertainment, politics, sport, and tech.

[BBC News Summary Dataset](http://mlg.ucd.ie/datasets/bbc.html)

## Methods

### LSTM Model with GloVe Embeddings
The model leverages pre-trained GloVe embeddings to initialise word vectors, enhancing semantic representation. A unidirectional LSTM encoder captures sequential dependencies in the input text. An attention mechanism is employed to prioritise critical portions of the sequence, enabling more focused summarization. Finally, an LSTM decoder generates the output summary, ensuring coherence and relevance.

### BiLSTM Model with GloVe Embeddings

The model utilises pre-trained GloVe embeddings for word vector initialization, ensuring rich semantic representation. A bidirectional LSTM encoder captures contextual dependencies in both forward and backward directions, enhancing comprehension of word relationships. An attention mechanism is incorporated to prioritise key information in the sequence. The summarised text is generated using an LSTM decoder, ensuring coherence and relevance.

### Transformer Model
The model employs a learned embedding layer, optionally enhanced with positional encoding to represent sequence order. A custom-built Transformer encoder, utilising multi-head self-attention, captures global dependencies within the input text. The Transformer decoder, featuring masked self-attention, autoregressively generates coherent and contextually relevant summaries.

### Hybrid Model Integration
The approach explores integrating LSTM and BiLSTM outputs as inputs to a Transformer encoder to enhance sequential and contextual understanding. An ensemble method is applied, combining model outputs through logit averaging or summary blending to improve overall performance. Additionally, stacking LSTM and BiLSTM layers is proposed to capture both local and global context before feeding the Transformer, aiming to further refine the summarization process.
