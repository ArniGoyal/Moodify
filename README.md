# 🎧 Moodify: Know The Vibe (Lyrics to Emotion Predictor)

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](YOUR_STREAMLIT_APP_URL)
[![GitHub license](https://img.shields.io/github/license/YOUR_USERNAME/YOUR_REPO_NAME)](./LICENSE)

A web application built with Streamlit and scikit-learn that classifies the dominant emotion (e.g., joy, sadness, anger) from song lyrics and suggests related songs from a database with the same predicted 'vibe'.

## 🖼️ Project Structure


## ✨ Key Features

* **Text Classification:** Uses a **TF-IDF Vectorizer** and a **Logistic Regression** model trained on song lyrics to predict one of 6 core emotions.
* **Data Preprocessing:** Includes custom preprocessing (stemming, stop-word removal, and cleaning) via `nltk`.
* **Song Recommendation:** Filters the `songs_db.csv` by the predicted emotion and then ranks the matching songs based on **Cosine Similarity** of their TF-IDF vectors to the user's input lyrics.

## 🛠️ Installation and Setup

To run Moodify locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
    cd YOUR_REPO_NAME
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the Streamlit app:**
    ```bash
    streamlit run app.py
    ```

## 📂 Data and Model

* **Model File:** The trained model (`tfidf_logreg_song_mood.pkl`) contains the TF-IDF vectorizer, the Logistic Regression classifier, and the label encoder.
* **Database:** `songs_db.csv` contains the song library used for suggestions.

## 🤝 Contribution

We welcome contributions! If you have suggestions for new features, bug fixes, or improvements to the model:

1.  Fork the repository.
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

## 📄 License

This project is licensed under the **[MIT/GPLv3] License** - see the [`LICENSE`](./LICENSE) file for details.

*(Remember to replace placeholders like `YOUR_STREAMLIT_APP_URL` and `YOUR_USERNAME/YOUR_REPO_NAME` with your actual information.)*