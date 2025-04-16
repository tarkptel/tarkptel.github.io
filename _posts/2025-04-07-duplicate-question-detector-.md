## 🔥 Quora Duplicate Question Detection

This project uses an **LSTM (Long Short-Term Memory)** model to identify whether two questions from the Quora dataset are semantically similar (duplicates).<br><br>

### 🔍 Overview
This project tackles the problem of semantic similarity between question pairs. By combining custom feature engineering with deep text preprocessing, the model learns to classify whether two questions convey the same meaning.<br><br>

### 🔗 Links  
- 🔥 **Live Demo:** [Try the App](https://huggingface.co/spaces/tensorboy0101/pneumonia_detection)  
- 🛠 **GitHub Repo:** [View on GitHub](https://github.com/tarkptel/Duplicate-Question-Detector/tree/main)  <br><br>


### ⚙️ Key Features & Workflow

This project combines structured feature engineering with deep text preprocessing to model the semantic similarity between two questions.

#### 🚀 Feature Engineering (22 Features)
These features are designed to capture lexical, syntactic, and fuzzy similarities between question pairs:

- **`q1_len`** – Number of characters in Question 1  
- **`q2_len`** – Number of characters in Question 2  
- **`q1_num_words`** – Number of words in Question 1  
- **`q2_num_words`** – Number of words in Question 2  
- **`word_common`** – Count of common words in both questions  
- **`word_total`** – Total unique words across both questions  
- **`word_share`** – Ratio of shared words to total unique words  
- **`cwc_min`** – Common word count divided by minimum of word counts  
- **`cwc_max`** – Common word count divided by maximum of word counts  
- **`csc_min`** – Ratio of common stopwords to minimum stopword count  
- **`csc_max`** – Ratio of common stopwords to maximum stopword count  
- **`ctc_min`** – Common token count to minimum token count  
- **`ctc_max`** – Common token count to maximum token count  
- **`last_word_eq`** – Whether the last words of both questions match  
- **`first_word_eq`** – Whether the first words of both questions match  
- **`abs_len_diff`** – Absolute difference in length between questions  
- **`mean_len`** – Average length of both questions  
- **`longest_substr_ratio`** – Ratio of longest common substring length to minimum question length  
- **`fuzz_ratio`** – Fuzzy string match ratio  
- **`fuzz_partial_ratio`** – Partial fuzzy match score  
- **`token_sort_ratio`** – Fuzzy match after sorting tokens  
- **`token_set_ratio`** – Fuzzy match using token sets <br><br>



#### 🌟 Text Preprocessing Workflow

1. **Lowercasing & Cleaning**
   - Removed punctuation, special characters, and HTML tags.

2. **Tokenization**
   - Used Keras tokenizer to convert text to sequences.

3. **Padding**
   - Ensured uniform input length using `pad_sequences`.

4. **Vocabulary Size**
   - Limited vocab size to reduce complexity (e.g., top 45,000 words).

5. **Embedding (optional)**
   - Used pre-trained embeddings or trained embeddings from scratch. <br><br>


### 📦 Model Architecture

- **Embedding Layer:** To convert text to dense vectors.
- **LSTM Layers:** Capture sequential dependencies in both questions.
- **Concatenation:** Combine features from both questions.
- **Dense Layers:** For final binary classification.<br><br>


#### 📌 Final Workflow

1. **Input Preparation**
   - Text sequences + engineered features combined to form a vector of shape **(1, 518)**.

2. **Model Selection**
   - Applied **LSTM** to capture semantic similarity between question pairs more effectively and boost performance.
   
3. **Evaluation**
   - Measured accuracy, F1-score, precision, recall on validation set.
   - Used confusion matrix and ROC curve for analysis.<br><br>


## 🚀 Tech Stack

- Python
- TensorFlow / Keras
- Pandas, NumPy
- NLTK / spaCy (for preprocessing)
- Jupyter Notebook <br><br>

## ⭐ *Feel free to fork or star this repo if you found it helpful!* 😊  
