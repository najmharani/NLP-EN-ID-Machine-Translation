# NLP Machine Translation: English to Indonesian

## Overview

This repository contains the implementation of an **English to Indonesian Machine Translation** project, developed as part of a college assignment for a Natural Language Processing (NLP) course. The project explores various translation models and evaluates their performance.

## Models

The following models were utilized in this project:

1. **Recurrent Neural Network (RNN)**
2. **Long Short-Term Memory (LSTM)**
3. **Transformer**
4. **T5-small**
5. **[Microsoft Phi-3-mini-4k-instruct](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct)** (LLM from Microsoft)

Each model was fine-tuned and tested on the given dataset to understand their effectiveness in the translation task.

## Dataset

The dataset used for this project is [Helsinki-NLP/opus-100 Dataset](https://huggingface.co/datasets/Helsinki-NLP/opus-100), which is a multilingual translation dataset. The subset used in this project is specifically English-to-Indonesian (en-id).

### Data Breakdown:

- **Training Data**: 100,000 samples (20,000 for LLM due to memory constraints). The source dataset contains 1 million samples, but only a subset of 100,000 was used in this project.
- **Validation Data**: 2,000 samples.
- **Test Data**: 2,000 samples.

## Folder Structure

The repository is organized as follows:

- **Model Training Code**: Each folder contains code for training a specific model.
- **Model Testing Code**: Each folder includes code for testing the corresponding model on the test data.
- **Sub-folder `results`**: Inside each model folder, this sub-folder contains:
  - Detailed predictions on the test data (input, reference, predictions, BLEU score).
  - Loss graph.
  - BLEU score graph.

## Results

The results of each model are summarized in terms of average BLEU scores calculated on 2000 test samples.

| Model         | Training Data | Average BLEU Score* |
| ------------- | ------------- | ------------------- |
| RNN           | 100,000       | TBD                 |
| LSTM          | 100,000       | TBD                 |
| Transformer   | 100,000       | TBD                 |
| T5            | 100,000       | TBD                 |
| Phi-3-mini-4k | 20,000        | TBD                 |

*Average BLEU Score is calculated based on the 2000 test data samples.

## Acknowledgements

- [Helsinki-NLP/opus-100 Dataset](https://huggingface.co/datasets/Helsinki-NLP/opus-100)
- [Microsoft Phi-3-mini-4k-instruct](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct)

