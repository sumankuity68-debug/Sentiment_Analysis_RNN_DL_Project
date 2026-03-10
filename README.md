# 💬 IMDB Sentiment Analysis using PyTorch RNN

## 📌 Project Overview

Sentiment analysis is a key natural language processing (NLP) task used to classify the **emotional tone of text**.  
This project focuses on building a **binary sentiment analysis model** to classify **IMDB movie reviews** as **positive or negative**.  

Using the **IMDB dataset**, we preprocess text data, vectorize it with **TF-IDF**, and train a **Recurrent Neural Network (RNN)** in **PyTorch** for sentiment classification.

---

## 📂 Dataset

The dataset used in this project is the **IMDB Movie Reviews Dataset**.  

Dataset link:  
[IMDB Dataset of 50K Movie Reviews](https://ai.stanford.edu/~amaas/data/sentiment/)  

### Dataset Features

* The dataset contains **50,000 movie reviews** (25,000 positive, 25,000 negative).  
* Reviews are pre-labeled with **sentiment**:  

  * `0` → Negative review  
  * `1` → Positive review  

* The dataset is **balanced**, making it suitable for binary classification.

---

## 🛠 Technologies Used

* Python 3.8+  
* Pandas  
* NumPy  
* Scikit-learn (TF-IDF Vectorizer, metrics)  
* PyTorch (RNN model)  
* Matplotlib / Seaborn (visualizations)  
* Jupyter Notebook  

---

## ⚙️ Project Workflow

1. **Data Collection** from IMDB dataset  
2. **Exploratory Data Analysis (EDA)** on reviews  
3. **Text Preprocessing** (lowercasing, removing stopwords, etc.)  
4. **TF-IDF Vectorization**  
5. **RNN Model Training**  
6. **Model Evaluation** using accuracy, precision, recall, F1-score  
7. **Prediction on New Reviews**  

---

## 🤖 Machine Learning Model

The primary model used in this project:

* **Recurrent Neural Network (RNN)** using PyTorch  
  * Input: TF-IDF features  
  * Hidden layer: 128 units  
  * Output: Binary sentiment  

Alternative models for experimentation:

* Logistic Regression  
* Random Forest Classifier  

---

## 📊 Model Evaluation Metrics

Since this is a **binary classification problem**, the following metrics are used:

* Accuracy  
* Precision  
* Recall  
* F1 Score  
* Confusion Matrix  

**Note:** For imbalanced subsets, precision and recall are more important than overall accuracy.  

---

## 📁 Project Structure
IMDB-Sentiment-Analysis/
│
├── data/
│ ├── train.csv
│ └── test.csv
│
├── notebooks/
│ └── sentiment_analysis.ipynb
│
├── src/
│ ├── model.py # PyTorch RNN model
│ ├── train.py # Training loop
│ └── evaluate.py # Evaluation scripts
│
├── README.md
└── LICENSE

---

## 📈 Results

The trained RNN model achieves **~86% accuracy** on the IMDB test set.  


---

## 🚀 Future Improvements

* Experiment with **LSTM or GRU networks** for better sequential modeling  
* Fine-tune **pretrained transformers** like BERT for sentiment analysis  
* Deploy the model as a **web application** using Flask or FastAPI  

---

## 🤝 Contributing

Contributions are welcome!  
Feel free to fork the repository, submit issues, or create pull requests.  

---

## 📜 License

This project is licensed under the **MIT License**.
