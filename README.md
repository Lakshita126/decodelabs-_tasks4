# NLP & Sentiment Analysis of Movie Reviews

## Project Overview

This project uses Natural Language Processing (NLP) and Machine Learning to classify movie reviews as **Positive** or **Negative**. It transforms unstructured text into numerical features using TF-IDF and trains a Multinomial Naive Bayes classifier to predict sentiment.

The project demonstrates how machine learning can analyze textual data and identify opinions expressed in movie reviews.

## Objectives

- Understand and preprocess unstructured text data.
- Perform tokenization, stop-word removal, and lemmatization.
- Convert text into numerical features using TF-IDF.
- Train a machine learning model for sentiment classification.
- Evaluate the model using classification metrics and a confusion matrix.
- Predict sentiment for new, user-provided movie reviews.

## Dataset

- **Dataset:** NLTK Movie Reviews Corpus
- **Total reviews:** 2,000
- **Positive reviews:** 1,000
- **Negative reviews:** 1,000
- **Features:** Review text and sentiment label

The dataset is balanced, with equal numbers of positive and negative reviews.

## Technologies Used

- Python
- Google Colab
- Pandas
- NLTK
- Scikit-learn
- Matplotlib
- Seaborn

## Project Workflow

### 1. Data Collection
Loaded the movie reviews corpus from the NLTK library and organized the reviews into a Pandas DataFrame.

### 2. Text Preprocessing
Prepared the reviews for machine learning through:
- Lowercasing text
- Removing punctuation and numbers
- Tokenization
- Stop-word removal
- Lemmatization

### 3. Feature Extraction
Used **TF-IDF (Term Frequency–Inverse Document Frequency)** to convert cleaned reviews into numerical features. The vectorizer was configured with a maximum vocabulary size of 5,000 features.

### 4. Train-Test Split
Split the dataset into:
- 80% training data (1,600 reviews)
- 20% testing data (400 reviews)

Stratified sampling was used to preserve the sentiment distribution.

### 5. Model Training
Trained a **Multinomial Naive Bayes** classifier on the TF-IDF features to distinguish positive reviews from negative reviews.

### 6. Model Evaluation
Evaluated predictions using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

### 7. Sentiment Prediction
Tested the trained model on four new movie reviews. The model correctly classified all four example reviews in the demonstration.

## Visualizations

The project includes:
- Positive and negative review distribution
- Confusion matrix showing correct and incorrect predictions

## Results

The model was trained and tested successfully. It produced the expected sentiment classifications for four manually provided example reviews.

**Test examples:**
- "This movie was amazing and I really enjoyed it" — Positive
- "The movie was boring and a complete waste of time" — Negative
- "Excellent acting and a wonderful story" — Positive
- "I hated this movie because it was terrible" — Negative

The four successful examples demonstrate the prediction workflow; they do not establish the model's overall accuracy. Refer to the notebook's evaluation output for the measured test-set metrics.

## How to Run the Project

1. Clone or download this repository.
2. Open `NLP_Sentiment_Analysis.ipynb` in Google Colab.
3. Run the notebook cells in order.
4. Allow NLTK to download the required corpus and language resources.
5. Review the model evaluation results and test new reviews.

## Limitations

- The model may struggle with sarcasm, mixed opinions, and context-dependent language.
- Preprocessing can remove useful information, including negation words.
- The results depend on the dataset and the chosen model.
- Correctly classifying a few manually written reviews does not guarantee strong performance on unseen reviews.

## Future Improvements

- Compare Naive Bayes, Logistic Regression, and Linear SVM.
- Tune hyperparameters to improve model performance.
- Investigate misclassified reviews.
- Analyze words associated with positive and negative sentiment.
- Build an interactive sentiment prediction application.

## Conclusion

This project demonstrates a complete introductory NLP workflow, from text preprocessing and TF-IDF feature extraction to model training, evaluation, and sentiment prediction. It provides a foundation for exploring more advanced text classification and sentiment analysis techniques.

## Author

**Your Name**

GitHub: [Add your GitHub profile link here]
