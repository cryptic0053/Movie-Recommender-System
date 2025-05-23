
# 🎬 Movie Recommender System

An intelligent movie recommendation engine that suggests films based on content similarity, utilizing metadata such as cast, crew, genres, and keywords.

> **🔗 Live Demo:** [recom94.streamlit.app](https://recom94.streamlit.app)

---

## 📌 Features

- **🎯 Content-Based Filtering**: Recommends movies similar to a selected title by analyzing metadata.
- **🖥️ Interactive Web Interface**: Built with Streamlit for seamless interaction.
- **⚡ Precomputed Similarities**: Fast recommendations using cosine similarity scores.
- **🖼️ TMDB Integration**: Fetches movie posters and details using The Movie Database (TMDB) API.
- **🚀 Easy Deployment**: Ready to deploy on Streamlit Cloud or other hosting platforms.

---

## 🧠 How It Works

The system processes the TMDB 5000 Movies and Credits datasets to extract relevant features like genres, cast, crew, and keywords.

1. These features are combined into a textual format.
2. `CountVectorizer` transforms the text into vectors.
3. `cosine_similarity` finds similar movies.
4. When a user selects a movie, the top 5 most similar movies are recommended.

---

## ⚙️ Prerequisites

- Python 3.7 or higher
- `pip` package manager

---

## 📥 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/cryptic0053/Movie-Recommender-System.git
cd Movie-Recommender-System
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
streamlit run app.py
```

Access the app at: [http://localhost:8501](http://localhost:8501)

---

## 🧪 Usage

1. Launch the app using the steps above.
2. Select a movie from the dropdown menu.
3. Click the **"Recommend"** button.
4. View the top 5 recommended movies with posters.

---

## 📊 Datasets Used

- **TMDB 5000 Movies Dataset**: Contains details about 5000 movies.
- **TMDB 5000 Credits Dataset**: Contains cast and crew information.

> 📌 These datasets are publicly available on [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata).

---

## 🛠️ Technologies Used

- **Python**: Core language
- **Pandas, NumPy**: Data processing
- **Scikit-learn**: ML utilities for vectorization & similarity
- **Streamlit**: Frontend web app
- **TMDB API**: Poster and movie detail fetching

---

## 🚀 Deployment

This app is already deployed at 👉 [recom94.streamlit.app](https://recom94.streamlit.app)

To deploy your own:

- Make sure `requirements.txt` includes all dependencies.
- Push your code to GitHub.
- Deploy to [Streamlit Cloud](https://streamlit.io/cloud) or alternatives like Heroku or AWS.

---

## 📬 Contact

For questions or collaboration:

- GitHub: [@cryptic0053](https://github.com/cryptic0053)
