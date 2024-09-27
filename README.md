# News-Authentication
An ML project to determine the authenticity of news

Project Overview:
In today's digital age, the rapid spread of fake news on social media and other platforms has become a pressing issue. This project focuses on developing a machine learning model to classify news articles as either real or fake by leveraging Natural Language Processing (NLP) techniques and Logistic Regression.

Project Details
1. Dataset
The dataset used in this project consists of 20,000 news articles, which are split into real and fake categories. It includes metadata like article content, headlines, publication dates, and labels (real or fake). The dataset was preprocessed to focus on the text content for analysis.

2. Preprocessing
Preprocessing the text was crucial for model performance. The following steps were taken using Python and the NLTK library:

Lowercasing: All text was converted to lowercase to maintain consistency.
Noise Removal: Punctuation, numbers, and non-alphabetic characters were removed using regular expressions.
Stemming: The Porter Stemmer was used to reduce words to their root forms (e.g., "running" to "run").
Stopword Removal: Common English stopwords like "the", "and", and "is" were removed to focus on meaningful words.

3. Feature Engineering: TF-IDF
Text data was converted into numerical features using TF-IDF (Term Frequency-Inverse Document Frequency), which measures the importance of words in each article relative to the entire dataset. This allowed the machine learning model to identify key terms that help differentiate real news from fake news.

4. Model Training
A Logistic Regression model was trained on the preprocessed and vectorized data. Logistic Regression was chosen for its simplicity and interpretability in binary classification problems like this one.

Model Accuracy: The Logistic Regression model achieved an accuracy of 97% on the test set, indicating strong performance in distinguishing real news from fake.

5. Hyperparameter Tuning
Hyperparameters such as C (regularization strength) and max_iter (maximum iterations) were fine-tuned to optimize the model's performance. The regularization parameter controls overfitting, while max_iter determines convergence during training.

6. Model Evaluation
The model was evaluated using accuracy, precision, recall, and F1-score. These metrics provided insights into the model's ability to correctly classify both real and fake news.

Key Insights
Emotionally Charged Language: Fake news articles commonly use words like "shocking", "breaking", and "exclusive" to grab attention and evoke strong emotions.
Neutral Vocabulary in Real News: Real news articles tend to use factual, objective words such as "official", "confirmed", and "source".
Article Length: Fake news articles were generally shorter, perhaps due to the intent of quick consumption and virality on social media platforms.
Sensationalized Headlines: Fake news often featured exaggerated or sensationalized headlines, which significantly contributed to its classification.


Visualizations
Word Cloud
A Word Cloud was generated to visualize the most frequent words in the dataset. The larger the word, the more frequently it appeared in the news articles. Fake news articles prominently featured terms like "breaking", "shocking", and "exclusive".


Word Count
A Word Count bar plot highlighted the top 10 most common words across all articles. Words such as "news", "report", and "said" were frequent, reflecting the standard journalistic language of both real and fake news.

Recommendations
Future Enhancements: Experimenting with more advanced models like XGBoost or using BERT embeddings could improve performance further.
Larger Dataset: Expanding the dataset to include more diverse sources and languages would increase the model's generalization ability.
Real-time Detection: Incorporating this model into a real-time system to flag suspicious news articles could be highly impactful for curbing the spread of misinformation.
Conclusion
This project demonstrates how machine learning and NLP techniques can effectively tackle the challenge of fake news detection. With a 97% accuracy score, the model shows promise in real-world applications where distinguishing truth from misinformation is critical.



