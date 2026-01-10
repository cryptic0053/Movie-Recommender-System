
# 🎬 Movie Recommender System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue) ![Streamlit](https://img.shields.io/badge/Streamlit-App-red) ![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Content%20Based-green)

A machine learning-based recommendation engine that suggests movies similar to a user's selection. This project utilizes **Content-Based Filtering** to analyze movie tags (genres, overview, cast, director) and compute similarity scores.

---

## 🚀 Features

* **Smart Recommendations:** Suggests 5 movies based on content similarity.
* **Content-Based Filtering:** Uses metadata (keywords, genres, cast, crew) rather than user ratings.
* **Interactive UI:** Built with **Streamlit** for a smooth user experience.
* **Real-time Data:** Fetches movie posters and details dynamically using the **TMDB API**.

---

## 🛠 Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Language** | Python |
| **Libraries** | Pandas, NumPy, Scikit-Learn, NLTK |
| **Frontend** | Streamlit |
| **API** | TMDB (The Movie Database) API |

---

## 📂 Project Structure

```bash
.
├── app.py                # Main Streamlit application
├── movie_recommender.ipynb # Jupyter Notebook for data processing & model building
├── tmdb_5000_movies.csv  # Dataset (Movies)
├── tmdb_5000_credits.csv # Dataset (Credits)
├── movies.pkl            # Pickled dataframe (generated)
├── similarity.pkl        # Pickled similarity matrix (generated)
├── requirements.txt      # Python dependencies
└── README.md             # Documentation

```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone [https://github.com/cryptic0053/Movie-Recommender-System.git](https://github.com/cryptic0053/Movie-Recommender-System.git)
cd Movie-Recommender-System

```

### 2. Install Dependencies

```bash
pip install -r requirements.txt

```

### 3. Generate Models (First Run Only)

If `movies.pkl` and `similarity.pkl` are not present, run the notebook or python script to generate them:

```bash
# Open the notebook and run all cells
jupyter notebook movie_recommender.ipynb

```

### 4. Run the App

```bash
streamlit run app.py

```

---

## 🧠 How It Works

1. **Data Preprocessing:** Merges credits and movies datasets; extracts relevant tags (genres, keywords, top 3 actors, director).
2. **Vectorization:** Converts text tags into vectors using `CountVectorizer` (Bag of Words).
3. **Similarity Calculation:** Computes the **Cosine Similarity** between all movie vectors.
4. **Recommendation:** When a user selects a movie, the system finds the 5 closest vectors (movies) with the highest similarity scores.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo.
2. Create a feature branch.
3. Commit your changes.
4. Push to the branch and open a Pull Request.

---

## 👤 Author

* GitHub: [@cryptic0053](https://github.com/cryptic0053)

---

*This project is for educational purposes and uses the TMDB dataset.*
