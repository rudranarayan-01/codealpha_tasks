# Twitter Sentiment Analysis

## Overview
This project performs sentiment analysis on tweets using Natural Language Processing (NLP) techniques and machine learning. The model classifies tweets as either positive or negative based on their content.

**ntscraper** - "ntscraper" in Python is primarily used to scrape tweets from Twitter without needing the official Twitter API, allowing users to easily extract tweets based on search terms, hashtags, or specific user profiles, all by leveraging Nitter instances which bypass API rate limits and authorization requirements; essentially, it's a tool for readily accessing real-time Twitter data for analysis without the complexities of API keys. 

## Features
- Preprocessing of text data using **NLTK PorterStemmer** and **stopwords corpus**.
- Feature extraction using **TfidfVectorizer**.
- Classification using **Logistic Regression**.
- Dataset sourced from **Kaggle** with approximately **160,000 tweets**.
- Achieved an accuracy of **80%**.

## Dataset
- The dataset used contains **160,000 tweets**, labeled as either positive (1) or negative (0).
- **Dataset Link** - https://www.kaggle.com/datasets/kazanova/sentiment140
- It was sourced from **Kaggle**.

## Technologies Used
- Python
- NLTK (Natural Language Toolkit)
- Scikit-learn (sklearn)
- Pandas
- NumPy
- ntscraper
- streamlit

## Installation
To set up the environment, install the required dependencies:
```bash
pip install nltk scikit-learn pandas numpy
```

## Preprocessing Steps
1. **Tokenization**: Splitting tweets into words.
2. **Removing Stopwords**: Using NLTK's corpus of stopwords.
3. **Stemming**: Using NLTK's PorterStemmer to normalize words.
4. **Vectorization**: Converting text into numerical features using TfidfVectorizer.

## Model Training
- **TfidfVectorizer** is used to transform the processed text into numerical features.
- **Logistic Regression** is trained using the transformed dataset.
- The model achieves **80% accuracy** on test data.

## Usage
Run the script to train and test the model:
```bash
streamlit run app.py
```

## Example Output
```
Tweet: "I love this product!"
Predicted Sentiment: Positive

Tweet: "This is the worst experience ever."
Predicted Sentiment: Negative
```

## Results
- Model accuracy: **80%**
- Can be further improved by fine-tuning hyperparameters or using deep learning models.

## Future Enhancements
- Implement deep learning models (LSTM, BERT) for improved accuracy.
- Expand the dataset for better generalization.
- Deploy the model as a web or API-based service.

## Acknowledgments
- **Kaggle** for providing the dataset.
- **NLTK & Scikit-learn** for powerful NLP and ML libraries.

## License
This project is licensed under the MIT License.

