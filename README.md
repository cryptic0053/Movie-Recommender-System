🎬 Movie Recommender System
An intelligent movie recommendation engine that suggests films based on content similarity, utilizing metadata such as cast, crew, genres, and keywords. Built with Python and deployed via Streamlit, this application offers users personalized movie suggestions in an intuitive web interface.

🔗 Live Demo: recom94.streamlit.app

📌 Features
Content-Based Filtering: Recommends movies similar to a selected title by analyzing metadata attributes.

Interactive Web Interface: User-friendly UI built with Streamlit for seamless interaction.

Precomputed Similarities: Utilizes preprocessed similarity scores for swift recommendations.

TMDB Integration: Fetches movie posters and details using The Movie Database (TMDB) API.

Efficient Deployment: Ready for deployment on platforms like Streamlit Cloud.
GitHub
+1
arXiv
+1
GitHub
GitHub
+2
GitHub
+2
GitHub
+2

🧠 How It Works
The system processes the TMDB 5000 Movies and Credits datasets to extract relevant features. It combines attributes like genres, cast, crew, and keywords into a single textual representation. Using the CountVectorizer, it transforms this text into a matrix of token counts, and then computes cosine similarity scores between movies. When a user selects a movie, the system retrieves and displays the top 5 most similar movies based on these scores.
GitHub

Prerequisites
Python 3.7 or higher

pip package manager

Installation
Clone the Repository

bash
Copy
Edit
git clone https://github.com/cryptic0053/Movie-Recommender-System.git
cd Movie-Recommender-System
Create a Virtual Environment

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install Dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run the Application

bash
Copy
Edit
streamlit run app.py
Access the application at http://localhost:8501 in your web browser.

🧪 Usage
Launch the application using the steps above.

Select a movie from the dropdown menu.

Click the "Recommend" button.

View the top 5 recommended movies along with their posters.
GitHub
+1
GitHub
+1

📊 Datasets
TMDB 5000 Movies Dataset: Contains information about 5000 movies including genres, overview, and more.

TMDB 5000 Credits Dataset: Includes details about the cast and crew for each movie.

These datasets are sourced from Kaggle.
GitHub

🛠️ Technologies Used
Python: Core programming language.

Pandas & NumPy: Data manipulation and numerical operations.

Scikit-learn: Machine learning tools for vectorization and similarity computation.

Streamlit: Framework for building interactive web applications.

TMDB API: Fetching movie posters and additional information.
GitHub
+3
GitHub
+3
GitHub
+3

📌 Deployment
The application is deployed and accessible at: recom94.streamlit.app

To deploy your own version:

Ensure all dependencies are listed in requirements.txt.

Configure the Procfile and setup.sh for your deployment platform.

Use platforms like Streamlit Cloud, Heroku, or AWS to host the application.

📬 Contact
For any inquiries or feedback:

GitHub: cryptic0053

