# Fine-tuning a masked language model for sentiment analysis on the IMDB dataset

This project fine-tunes a masked language model (DistilBERT) on the IMDB dataset for sentiment analysis. The goal is to demonstrate the process of fine-tuning a pre-trained model for a specific task using the Hugging Face Transformers library.

## Model

The model used in this project is DistilBERT, a smaller and faster version of BERT. It is a pre-trained masked language model, which means it has been trained on a large corpus of text to predict masked tokens.

## Dataset

The dataset used is the IMDB dataset, which contains movie reviews labeled as either positive or negative sentiment. The dataset is loaded using the Hugging Face Datasets library.

## Fine-tuning

The DistilBERT model is fine-tuned on the IMDB dataset using the masked language modeling objective. This involves masking a percentage of the tokens in the input sequences and training the model to predict the original tokens.

The fine-tuning process is performed using the Hugging Face Trainer API, which provides a simple and efficient way to train models.

## Results

After fine-tuning, the model is evaluated on the test set to measure its performance on the masked language modeling task. The perplexity metric is used to evaluate the model, which measures how well the model predicts the masked tokens. A lower perplexity indicates better performance.

The fine-tuned model is then pushed to the Hugging Face Hub, where it can be easily shared and used by others.
