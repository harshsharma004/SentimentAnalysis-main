# 🌐 Multilingual Sentiment Analysis

A powerful, real-time web application built with **Streamlit** and **TensorFlow** that predicts the sentiment (Positive or Negative) of a given text. This app supports **multilingual inputs**—automatically detecting the language and translating it to English before performing deep learning-based sentiment analysis.

## ✨ Features
- **Multilingual Support:** Type in any language! The app uses `deep-translator` to seamlessly translate input to English.
- **Deep Learning Model:** Powered by a custom-trained **Bidirectional LSTM** (Long Short-Term Memory) neural network.
- **Real-Time Analysis:** Instantly classifies text as Positive 😊 or Negative 😞 with a confidence score.
- **Interactive UI:** Beautiful, responsive interface built with Streamlit, including a dynamic word frequency bar chart.
- **NLP Preprocessing:** Uses `NLTK` and regular expressions to intelligently clean text (removing stopwords, URLs, and punctuation).

## 🛠️ Technology Stack
- **Frontend / Web Framework:** [Streamlit](https://streamlit.io/)
- **Machine Learning:** [TensorFlow](https://www.tensorflow.org/) & Keras
- **NLP & Translation:** NLTK, `deep-translator`
- **Data Handling:** NumPy, Pandas

## 📂 Project Structure
- `app.py`: The main Streamlit web application. Handles the UI, translation, text preprocessing, and inference.
- `Sentiment_Analysis_Training.ipynb`: Jupyter Notebook containing the data preprocessing and Bidirectional LSTM model training pipeline.
- `lstm_sentiment_model.h5`: The pre-trained Keras LSTM model.
- `tokenizer.pkl`: Pickled tokenizer used to convert input text into numerical sequences for the model.
- `requirements.txt`: Python dependencies required to run the app.
- `study_plan.md`: A structured guide explaining the NLP and deep learning concepts used in this project.

## 🚀 How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/harshsharma004/SentimentAnalysis-main.git
   cd SentimentAnalysis-main
   ```

2. **(Optional) Create a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install the dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Streamlit application:**
   ```bash
   streamlit run app.py
   ```
   The app will automatically open in your browser at `http://localhost:8501`.

## ☁️ Deployment Guide (Streamlit Community Cloud)
This project is fully ready to be deployed for free on Streamlit Community Cloud!

1. Push your code to a public GitHub repository.
2. Log into [Streamlit Community Cloud](https://share.streamlit.io/).
3. Click **New app** and connect your repository.
4. Set the main file to `app.py`.
5. **Important:** Click on **Advanced settings** and set the **Python version to 3.11** (or 3.10) to ensure compatibility with `tensorflow-cpu`.
6. Click **Deploy!**

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page if you want to contribute.
