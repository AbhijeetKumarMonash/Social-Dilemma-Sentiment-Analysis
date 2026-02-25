The Social Dilemma: Twitter Sentiment Analysis
This project presents a comprehensive Natural Language Processing (NLP) analysis of Twitter data associated with the hashtag #TheSocialDilemma. The data was collected following the release of the Netflix documentary “The Social Dilemma”, which explores the impact of social networking and algorithms on human behavior.

🎯 Project Objective
The goal of this analysis is to:

Clean and explore Twitter response data.

Identify user sentiments (Positive, Negative, Neutral) regarding the documentary.

Build machine learning classifiers to predict tweet sentiment.

📊 Dataset Description
The dataset (TheSocialDilemma.csv) contains 20,068 tweets. Key columns include:

text: The raw content of the tweet.

Sentiment: Manual labels for sentiment classification.

user_followers & user_verified: Metadata regarding the tweet's source.

hashtags: Related topics mentioned in the tweets.

🛠️ Data Preprocessing Details
To ensure high-quality analysis, several cleaning steps were performed:

Language Filtering: Non-English tweets were removed based on an ASCII character threshold (keeping tweets with >90% ASCII). After filtering, 20,005 tweets remained.

Text Cleaning: * Elimination of special characters, numbers, and HTML tags.

Removal of URLs, mentions (@), and hashtags.

Stopword removal and lowercase normalization.

Tokenization & Lemmatization: Converting text into base forms for better feature extraction.

📈 Key Insights from Data Exploration
Missing Values: The dataset was relatively clean, with some missing values in user_location, user_description, and hashtags. No missing values were found in the critical text or Sentiment columns.

Cardinality: High cardinality was observed in columns like user_name and user_location, while user_verified and is_retweet provided useful categorical features.

🤖 Modeling and Evaluation
The project involves building a supervised learning classification model. The process includes:

Vectorization: Converting cleaned text into numerical format using techniques like TF-IDF or CountVectorizer.

Model Comparison: Testing at least three different classification models (e.g., Logistic Regression, Random Forest, Multinomial Naive Bayes).

Performance Metrics: Evaluating models using Confusion Matrices, Accuracy, Precision, and Recall.

🏁 Findings
The analysis explores how users reacted to the documentary's argument that algorithms are adept at "curating our reality" and influencing thoughts.

A Wordcloud of the top 40 important features highlights the most significant words associated with specific sentiments (e.g., words like "scary" often appearing in negative sentiments).
