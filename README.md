# Text_Summarization_NLP_Project
A Comparitive study of LSTM, BiLSTM and Transformer Models for Text Summarization tasks.

This repository contains codes for a LSTM, BiLSTM, Transfomer Model and a hybrid transformer model designed for text summarization using the BBC News Summary dataset to generate concise summaries from news articles.

## Getting Started on Kaggle

To run this code and reproduce the results, follow these steps to set up your Kaggle environment:

1. Create a Kaggle account if you don't have one already.

2. Your Identity needs to be verified for you to be able to access Kaggle's GPUs for foree for 30 hours / week.

3. Go to the Kaggle Notebooks section and create a new notebook.

4. Enable GPU acceleration:
   - Click on the "..." menu in the top-right corner of your notebook.
   - Select "Accelerator" and choose "GPU" from the dropdown menu.

5. Add the BBC News Summary dataset:
   - Click on the "+" icon in the "Data" section on the right sidebar.
   - Search for "BBC News Summary" in the dataset browser.
   - Click "Add" to include the dataset in your notebook.

6. Import the code:
   - You can either copy and paste the code directly into Kaggle notebook cells, or
   - Upload the Python script files to your Kaggle notebook using the "Upload" button in the "Files" section.

7. Run the code:
   - Execute the cells in order to train and evaluate the model.

## Repository Structure

- `LSTM+GloVe.ipynb`: Implements an LSTM Model with GloVe embeddings for text summarization
- `BiLSTM+GloVe.ipynb`: Implements a BiLSTM Model with GloVe embeddings for text summarization
- `Transformer Model.ipynb`: Implements a Transformer Model embeddings and positional encodings for text summarization
- `Hybrid Model - LSTM + BiLSTM + Transformer`: Implements a Hybrid model thattakes the LSTM and BiLSTM outputs as inputs to the Transformer Model for text summarization
- `Dataset details.pdf`: Provides a link to the dataset as it is too large to upload.
- `README.md`: This file, containing instructions for setup and usage.

## Dataset

The BBC News Summary dataset is used for training and evaluation. It contains news articles and their corresponding summaries across various categories such as business, entertainment, politics, sport, and tech.

Thank you!
