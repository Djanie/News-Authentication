# News-Authentication
An ML project to determine the authenticity of news

Project Overview:
In an age where misinformation spreads rapidly through social media and online platforms, detecting fake news is crucial. This project aims to develop a machine learning model capable of classifying news articles as real or fake using Natural Language Processing (NLP) and Logistic Regression.

Project Summary:

Dataset: 20,000 news articles (fake and real) were used to train and test the model.
Text Preprocessing: Using Python and NLTK, I applied several preprocessing techniques, including lowercasing, stemming, and stopword removal, to clean the text.
Vectorization: I implemented TF-IDF (Term Frequency-Inverse Document Frequency) to convert the text data into numerical features.
Model: A Logistic Regression model was trained to differentiate between real and fake news, achieving an accuracy of 97%.

Key Insights:

Fake news articles often contain emotionally charged language like "shocking", "breaking", and "exclusive".
Real news tends to use more factual and neutral vocabulary such as "source", "official", and "report".
Article length and timing can significantly affect prediction accuracy.
Visualizations:

The Word Cloud highlighted frequent words in fake news articles such as "shocking", "breaking", and "exclusive", which reflect their sensationalized nature.

Recommendations:

Future improvements could include exploring more advanced models like XGBoost or using BERT embeddings for deeper linguistic understanding.
Expanding the dataset to cover diverse regions and languages would enhance model robustness.
