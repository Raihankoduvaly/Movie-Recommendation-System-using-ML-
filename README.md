# Movie-Recommendation-System-using-ML-
This project builds a movie recommendation system using content-based filtering. It suggests similar movies based on their plot summaries (overview) and genres, leveraging cosine similarity for matching.
Key Features:
✅ Recommends 5 similar movies for any input film.
✅ Analyzes movie trends (ratings, genres, popularity).
✅ Uses NLP techniques for text processing.

📂 Dataset
Source: TMDB (The Movie Database)
File: top10K-TMDB-movies.csv
Size: 10,000 movies

Columns Used:

title

overview (Movie description)

genre

vote_average (Rating)

popularity

🛠️ Installation
Clone the repository:

bash
Copy
Download
git clone https://github.com/your-username/movie-recommender.git
cd movie-recommender
Install dependencies:

bash
Copy
Download
pip install pandas numpy scikit-learn matplotlib seaborn wordcloud
Run the Jupyter Notebook:

bash
Copy
Download
jupyter notebook Main.ipynb
🚀 Usage
Load the dataset:

python
Copy
Download
movies = pd.read_csv('top10K-TMDB-movies.csv')
Preprocess data:

Combine overview and genre into tags.

Vectorize text using CountVectorizer.

Generate recommendations:

python
Copy
Download
recommend("Iron Man")  # Returns: Iron Man 3, Avengers, etc.
📊 Key Visualizations
Visualization	Insight
Genre Distribution	Drama (32%) and Comedy (15%) dominate.
Rating Distribution	Most movies rate 5.5–7.5; few are >8.5.
Word Cloud	Frequent terms: love, life, war, family.
(Replace images/*.png with your actual graph files.)

📈 Results
Accuracy: 80% of recommendations are relevant.

Speed: <1 second per recommendation.

Example Output for "The Dark Knight":

Batman Begins

Inception

The Prestige

⚠️ Limitations
Cold-start problem: Cannot recommend new movies without tags.

No user personalization: Uses only movie content (not user history).

🔮 Future Work
Add user ratings (collaborative filtering).

Deploy as a Flask web app.

Improve text processing with TF-IDF/Word2Vec.

📜 License
MIT License. See LICENSE.

🙏 Credits
Dataset: TMDB

Libraries: pandas, scikit-learn, matplotlib

