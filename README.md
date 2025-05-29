#  Swiggy Review Sentiment Analysis using RNN

This project builds a sentiment analysis model using customer reviews from Swiggy. It leverages Natural Language Processing (NLP) and a Recurrent Neural Network (RNN) built with TensorFlow/Keras to classify reviews as **Positive** or **Negative** based on average rating scores.

---

##  Project Features

- Reads and preprocesses Swiggy review data
- Cleans and tokenizes text
- Labels sentiment using average ratings
- Trains an RNN (SimpleRNN) model to classify sentiment
- Evaluates performance and allows new prediction inputs

---

##  Model Architecture

- **Embedding Layer**: Converts words into vector representations
- **SimpleRNN Layer**: Captures sequential dependencies in text
- **Dense Layer**: Binary classification with sigmoid activation

---

##  Tech Stack

- Python 3.x
- Pandas, NumPy, Regex
- Scikit-learn
- TensorFlow / Keras

---

##  Dataset

The dataset is expected to be a CSV file named `swiggy.csv` with at least these columns:

- `Review`: The text of the review
- `Avg Rating`: A numeric rating used to infer sentiment

---

##  Preprocessing Steps

1. Convert text to lowercase
2. Remove special characters using regex
3. Tokenize and pad sequences
4. Label sentiment as:
   - `1` (Positive) if Avg Rating > 3.5
   - `0` (Negative) otherwise

---

##  How to Run

### 1. Clone the Repository
git clone https://github.com/yourusername/swiggy-sentiment-analysis.git
cd swiggy-sentiment-analysis

### 2. Install Dependencies
pip install pandas numpy scikit-learn tensorflow
### 3. Place the Dataset
Ensure swiggy.csv is in the root directory.
### 4. Run the Script
python sentiment_rnn.py
