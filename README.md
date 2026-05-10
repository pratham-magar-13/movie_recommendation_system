# Movie Recommendation System 🎬

A content-based movie recommendation engine built with Python that suggests films based on metadata similarities such as genres, keywords, cast, and crew.

## 🚀 Overview
This project uses the **TMDB 5000 Movie Dataset** to analyze and recommend movies. By transforming text data into mathematical vectors, the system identifies movies that are conceptually similar to a user's favorite film.

## 🛠️ Tech Stack
- **Language:** Python
- **Data Analysis:** Pandas, NumPy
- **Machine Learning:** Scikit-Learn (CountVectorizer, Cosine Similarity)
- **Natural Language Processing:** NLTK (PorterStemmer)
- **Deployment Ready:** Pickle (for model serialization)

## ⚙️ How it Works
1. **Data Preprocessing:** Merges movie metadata with credits and cleans JSON-formatted columns.
2. **Feature Engineering:** Combines 'overview', 'genres', 'keywords', 'cast', and 'crew' into a single "tags" column.
3. **Text Vectorization:** Converts tags into 5,000-dimensional vectors using the "Bag of Words" technique.
4. **Similarity Calculation:** Uses **Cosine Similarity** to measure the distance between movie vectors. The closer the vectors, the more similar the movies.

## 📖 Usage
To get a recommendation, simply call the `recommend` function with a movie title:
recommend('Movie_name')
