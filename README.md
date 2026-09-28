# YouTube Comments Sentiment Analysis

YouTube is a very large, free video sharing website that makes it easy to watch online videos. On average, 100 hours of videos are uploaded to YouTube every minute, so there’s always something new to watch!

There are so many different content creators on YouTube creating a variety of content across many different categories. These creators can use this project to analyze whether their videos are receiving positive reviews or not, helping them work on improving their content. They can also analyze what kind of content becomes most popular and grossing through our system.

## Tech Stack

- **Language:** Python
- **Libraries:** Pandas, Scikit-learn, NLTK, Regular Expressions (re), CSV
- **Environment:** Jupyter Notebook / Google Colab

## Machine Learning & NLP Techniques

This project incorporates robust Natural Language Processing (NLP) techniques and multiple Machine Learning classification algorithms:

**NLP Preprocessing:**
- Tokenization & Text cleaning (removing non-alphabetic characters)
- Stop Words removal
- Stemming (PorterStemmer) & Lemmatization
- Text Vectorization (`CountVectorizer`, `TfidfVectorizer`)

**Machine Learning Models Evaluated:**
- Multinomial Naive-Bayes
- Logistic Regression
- Support Vector Classifier (SVC)
- Decision Tree Classifier
- Random Forest Classifier

## Datasets

We have made use of various datasets which can be generalized into two types:
1. **General Discussions:** Datasets containing non-youtube comments that are still related to youtube videos (basically discussions on different social medias like tweets and blogs).
2. **Channel-Specific Comments:** Datasets which individually focus on the comments of particular youtube channels such as rock band OKGO, famous singer Taylor Swift, Logan Paul, Royal Wedding, etc. 

*All these CSV datasets are located inside the `data/` directory.*

## Repository Structure

- `YouTube_Comment_Sentiment_Analysis.ipynb`: The main Jupyter Notebook containing the entire pipeline from data preprocessing to model training, evaluation, and prediction.
- `data/`: Contains various CSV datasets (e.g., `Comments.csv`, `twitter.csv`, `Kagel.csv`, `LoganPaul.csv`, `OKGO.csv`, `RoyalWedding.csv`, `TaylorSwift.csv`, `trump.csv`) used for training, testing, and making predictions.
- `README.md`: Project documentation.

##  How to Use

1. **Clone the repository:**
   ```bash
   git clone <repo-url>
   cd YouTube-Comments-Sentiment-Analysis
   ```

2. **Setup your environment:**
   Ensure you have Python installed along with the required libraries:
   ```bash
   pip install pandas scikit-learn nltk
   ```
   *(Note: You may need to download NLTK data dependencies like stopwords via `nltk.download()` within python).*

3. **Predicting Sentiment for a New Video:**
   - Go to the YouTube video of your choice and scrape/download the comments.
   - Replace or append them into the `data/Comments.csv` file.
   - Run the notebook's final prediction sections.

4. **Run the Notebook:**
   Execute the cells in `YouTube_Comment_Sentiment_Analysis.ipynb` locally using Jupyter or upload it to Google Colab.

---
**Link to original colab:** [Google Colab Workspace](https://colab.research.google.com/drive/1wYUqA5g4urobK5gMzF_Np4Tq5CTljRee#scrollTo=84d0c392)
