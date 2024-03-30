# Human Value Detection using BERT-based Classifiers

## Overview

This project focuses on the Human Value Detection challenge. It aims to classify arguments based on conveyed human values in terms of stance, premise, and conclusion. The project explores various models, including baseline models (random uniform, majority classifiers), and advanced BERT-based classifiers in three configurations: using only the conclusion (BERT w/ C), the conclusion and premise (BERT w/ CP), and adding stance to conclusion and premise (BERT w/ CPS). The evaluation metric used is the F1-score, providing a comprehensive comparison of BERT-based models against baseline classifiers in human value detection.


## Dataset

The dataset consists of structured arguments categorized based on stance (e.g., 'in favour of' or 'against') into four Level 3 human value categories: Openness to Change, Self-Enhancement, Conservation, and Self-Transcendence. The data files include:

- arguments-training.tsv
- labels-training.tsv
- arguments-validation.tsv
- labels-validation.tsv
- arguments-test.tsv
- labels-test.tsv

## Model Training and Evaluation

The project implements and compares different models:

- Baseline models using `sklearn`'s `DummyClassifier`.
- Advanced BERT-based classifiers using the `roberta-base` model from the `transformers` library.

To run the training and evaluation, execute the code blocks within the Jupyter Notebook. The process involves preparing the data, training the models, and evaluating them using precision, recall, and F1-score metrics.

## Results

Our experiments show that BERT-based classifiers outperform the baseline models in detecting human values in argumentative texts. The addition of the stance to the model inputs (BERT w/ CPS) provided significant performance improvements.

## Conclusion

This project demonstrates the effectiveness of BERT-based classifiers for the task of human value detection in arguments. Advanced models, particularly those incorporating stance information, show promising results in capturing the nuances of language and underlying values in argumentative texts.

## References

- [Hugging Face Transformers](https://huggingface.co/)
- [BERT, RoBERTa, DistilBERT, XLNet - Which one to use?](https://towardsdatascience.com/bert-roberta-distilbert-xlnet-which-one-to-use-3d5ab82ba5f8)


```

This README provides a concise overview of the project, including its objectives, setup instructions, dataset information, details on model training and evaluation, results, conclusion, and contact information for further inquiries.
