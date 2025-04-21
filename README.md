# 🎬 Movies Recommender System

A content-based movie recommendation system built with Python. It suggests similar movies based on a selected title by analyzing metadata such as genres, cast, crew, and plot overview. A lightweight web interface is provided to make it easily accessible to users.

---

## 🚀 Features

- 📽️ Recommends movies based on content similarity
- 🧠 Uses cosine similarity on combined metadata ("tags")
- ⚡ Fast retrieval using preprocessed data and similarity matrix
- 🌐 Web app built with Streamlit or Flask

---

## 🧰 Tech Stack

- Python 3.x
- Pandas, NumPy, Scikit-learn
- NLTK (for text preprocessing)
- Pickle (for saving models)
- Flask / Streamlit (for the frontend)

---

## 📁 Project Structure

Movies-Recommender-System/ ├── app.py # Web app interface ├── Movie Recommender.ipynb # Model building and logic ├── movies.csv # Raw movie metadata ├── credits.csv # Credits data (cast & crew) ├── movies.pkl # Processed data for app use ├── similarity.pkl # Cosine similarity matrix ├── requirements.txt # Dependencies └── .gitignore / .idea # Git/IDE config


---

## 🧪 How It Works

1. **Data Merging**: Merges `movies.csv` and `credits.csv` to gather all relevant metadata.
2. **Tag Creation**: Constructs a "tags" column by combining genres, cast, crew, and overview.
3. **Text Vectorization**: Applies `CountVectorizer` to transform tags into vectors.
4. **Similarity Matrix**: Calculates cosine similarity between movie vectors.
5. **Recommendation Logic**: Finds top 5 similar movies to any given movie title.

---

## 💡 Usage

- Launch the app (`app.py`) via Streamlit or Flask.
- Enter the name of a movie.
- Get instant recommendations with poster images (if integrated).

---

## 📌 Notes

- Preprocessed `.pkl` files (`movies.pkl`, `similarity.pkl`) are used for faster app performance.
- You can regenerate them by running the notebook (`Movie Recommender.ipynb`) if needed.

---

## 🙌 Credits

- Dataset sourced from [TMDB on Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata).
- Inspired by personal love for film and machine learning.
