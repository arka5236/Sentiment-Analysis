This project develops a full sentiment analysis pipeline for a large Twitter dataset. The approach involves several key stages:

Data Preprocessing: The original dataset is loaded and trimmed to the first six columns, with special attention paid to cleaning the target labels (which are stored with extra quotation marks) and filtering for binary sentiment labels. The tweet text is normalized by converting to lowercase, removing URLs, mentions, punctuation, and extra spaces, and then filtering out any finalized empty texts.

Feature Extraction: Cleaned tweet texts are transformed using TF-IDF vectorization, converting the unstructured text data into a numerical format suitable for model input.

Sentiment Analysis with VADER: A lexicon-based VADER model is applied to the cleaned text to compute sentiment scores—including a compound score that summarizes the overall sentiment polarity. This output is used to label tweets as positive, neutral, or negative.

Sentiment Analysis with RoBERTa: In parallel, a pre-trained RoBERTa model fine-tuned on Twitter sentiment (from the cardiffnlp collection) is used. This transformer-based model predicts sentiment labels and produces confidence scores for each tweet, providing a modern, context-aware alternative to the lexicon-based approach.

Comparative Evaluation: The results of both VADER and RoBERTa analyses are compared through various visualizations. Exploratory plots, including bar plots, box plots, scatter plots, and pairplots created using Seaborn, help elucidate the similarities, differences, and relationships between the two methodologies.

Overall, the project not only outlines the process of cleaning and vectorizing tweet data but also demonstrates how traditional lexicon-based models can be compared and complemented by modern transformer-based models in the task of sentiment analysis on social media data. This comprehensive pipeline paves the way for further refinements and applications in social media analytics.
