# Cyber-Bullying Prediction

Detects cyberbullying in Formspring Q&A posts using NLP and machine learning. Text is preprocessed (stopword removal, stemming) and vectorized with TF-IDF, then classified using multiple models with hyperparameter tuning via GridSearchCV.

## Dataset

`Formspring.csv` -- 13,147 Q&A text entries from the Formspring social platform, labeled for cyberbullying presence.

## Results

| Model | Accuracy | Precision | Recall |
|-------|----------|-----------|--------|
| SVC (sigmoid kernel) | 95.08% | 80.52% | 25.73% |
| Multinomial Naive Bayes | 94.02% | 53.62% | 15.35% |
| Decision Tree | 93.11% | 41.88% | 33.20% |

**Note:** The dataset is imbalanced (mostly non-bullying), so accuracy is high but recall for the bullying class is low across all models.

## Tech Stack

- pandas, numpy
- NLTK (stopwords, SnowballStemmer)
- scikit-learn (TfidfVectorizer, GridSearchCV, SVC, MultinomialNB, DecisionTreeClassifier, LogisticRegression, RidgeClassifier, SGDClassifier, LabelEncoder)
- matplotlib
