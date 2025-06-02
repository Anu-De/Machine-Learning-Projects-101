Project Report: IMDB Movie Review Sentiment Classification

    Dataset Overview

The dataset consists of 50,000 movie reviews labeled with sentiment categories: positive and negative. The data is balanced, with 25,000 reviews in each class. Class Count Positive 25,000 Negative 25,000

The reviews are stored as text, and the sentiment labels are categorical.

    Data Preprocessing

    Text Vectorization: Utilized TfidfVectorizer to convert text reviews into numerical feature vectors, capturing important word importance and reducing the impact of frequently occurring words.

    Model Training and Performance Three models were trained and evaluated:

    Logistic Regression:

     Achieved an accuracy of approximately 89.48%
     ROC AUC score of 0.962
     Performance metrics indicate high precision and recall for both classes.

    Naive Bayes:

     Achieved an accuracy of 85.34%
     ROC AUC score of 0.931
     Slightly lower performance compared to Logistic Regression but still effective.

    XGBoost:

     Achieved an accuracy of 86.82%
     ROC AUC score of 0.943
     Demonstrated strong predictive power with balanced precision and recall.

    Evaluation Metrics
    Model Accuracy ROC AUC Precision (Positive) Recall (Positive) F1-Score (Positive) Support (Positive) Precision (Negative) Recall (Negative) F1-Score (Negative)

Logistic Regression 89.48% 0.962 0.89 0.91 0.90 5039 0.90 0.88 0.89

Naive Bayes 85.34% 0.931 0.85 0.85 0.85 5039 0.85 0.85 0.85

XGBoost 86.82% 0.943 0.88 0.85 0.86 4961 0.86 0.89 0.87

    Conclusion The models demonstrated good performance in classifying movie reviews as positive or negative based on textual content. Logistic Regression showed the highest accuracy and ROC AUC, making it a strong candidate for deployment. Naive Bayes, while slightly less accurate, offers computational efficiency. XGBoost provided competitive results with balanced metrics.

    Future Recommendations

    Incorporate advanced NLP techniques such as word embeddings (e.g., Word2Vec, GloVe) for richer feature representations. Perform hyperparameter tuning to optimize model performance further. Explore deep learning models like LSTM or Transformer-based architectures for improved context understanding.

