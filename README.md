This project develops a full sentiment analysis pipeline for a large Twitter dataset. The approach involves several key stages:

Data Preprocessing: The original dataset is loaded and trimmed to the first six columns, with special attention paid to cleaning the target labels (which are stored with extra quotation marks) and filtering for binary sentiment labels. The tweet text is normalized by converting to lowercase, removing URLs, mentions, punctuation, and extra spaces, and then filtering out any finalized empty texts.

Feature Extraction: Cleaned tweet texts are transformed using TF-IDF vectorization, converting the unstructured text data into a numerical format suitable for model input.

Sentiment Analysis with VADER: A lexicon-based VADER model is applied to the cleaned text to compute sentiment scores—including a compound score that summarizes the overall sentiment polarity. This output is used to label tweets as positive, neutral, or negative.

Sentiment Analysis with RoBERTa: In parallel, a pre-trained RoBERTa model fine-tuned on Twitter sentiment (from the cardiffnlp collection) is used. This transformer-based model predicts sentiment labels and produces confidence scores for each tweet, providing a modern, context-aware alternative to the lexicon-based approach.

Comparative Evaluation: The results of both VADER and RoBERTa analyses are compared through various visualizations. Exploratory plots, including bar plots, box plots, scatter plots, and pairplots created using Seaborn, help elucidate the similarities, differences, and relationships between the two methodologies.

Overall, the project not only outlines the process of cleaning and vectorizing tweet data but also demonstrates how traditional lexicon-based models can be compared and complemented by modern transformer-based models in the task of sentiment analysis on social media data. This comprehensive pipeline paves the way for further refinements and applications in social media analytics.
![image](https://github.com/user-attachments/assets/e5f8a9b2-7129-4b92-aa5a-0d88d55c8952)
![image](https://github.com/user-attachments/assets/62f40516-a73e-4b9d-bea3-37322603e3f3)
![image](https://github.com/user-attachments/assets/d6c0e0b2-405e-43f1-b98e-65f1b4197555)
![image](https://github.com/user-attachments/assets/93f4b723-79af-47d1-8e0d-c44e599bcb28)
![image](https://github.com/user-attachments/assets/dc73edf2-3cca-4b72-9788-16fba360c8bc)
![image](https://github.com/user-attachments/assets/d063a615-68c8-4c86-b680-faf3ffa02060)
![image](https://github.com/user-attachments/assets/8cbb625b-8d29-42f5-ab6c-094deeac0439)
![image](https://github.com/user-attachments/assets/12030882-a8f8-4adb-934d-6e0a4e869f6b)
![image](https://github.com/user-attachments/assets/248ad251-2775-4a98-b03e-81c34a86b407)
![image](https://github.com/user-attachments/assets/633a4cdf-60e1-4b57-9c6c-a8903738f901)
![image](https://github.com/user-attachments/assets/160afefa-3033-4350-a6a7-2f069e561437)
![image](https://github.com/user-attachments/assets/3806a34f-96a8-45d7-bc57-b9424d9aa6ef)





