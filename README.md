# Active Learning Strategy for Text Classification with BERT

This project demonstrates an innovative active learning strategy for text classification tasks, which combines selecting novel examples and instances for which the model is uncertain. The strategy calculates prediction entropy on already labeled data to identify examples where the model is most uncertain and then uses prediction entropy again as a strategy for the unlabeled pool. The model is updated using both query results on the unlabeled pool and on the example in which the model was most uncertain. BERT is utilized as the underlying model for this strategy.

## Project Highlights:

- Designs an active learning strategy that selects novel examples and instances where the model is uncertain.
- Leverages BERT for text classification.
- Utilizes the small-text and datasets libraries for dataset handling and model creation.
- Employs an Active Learning strategy using Prediction Entropy as a query strategy for selecting uncertain samples.
- Presents the results in terms of train and test accuracy for each iteration of the active learning process.

## Key Components:

- Dataset: Toxic Conversations 50k
- Libraries and Dependencies:
- small-text[transformers]==1.3.0
- setfit>=0.5.0
- datasets
- matplotlib
- Hugging Face Transformers

## Main Steps:

- Load and preprocess the dataset.
- Create a balanced initial labeled set for active learning.
- Create SetFit classifiers using the small_text library.
- Implement an active learning loop with a query strategy based on Prediction Entropy.
- Evaluate and store the train and test accuracy for each iteration.


This project showcases a unique active learning strategy for text classification tasks, combining the selection of novel examples and instances where the model is uncertain. The results can be used to inform future improvements in active learning techniques and text classification approaches.
