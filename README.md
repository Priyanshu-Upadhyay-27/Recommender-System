# Movie Recommender-System
# 🎬 Movie Recommender System

This is a **Content-Based Movie Recommender System** built using Python and Streamlit. The app recommends movies based on textual similarity between movie descriptions (overview, genres, keywords, cast, crew). It uses **TF-IDF** and **cosine similarity** to find the most similar movies.

> 📽️ Built by following CampusX’s excellent tutorial: [Watch here](https://www.youtube.com/watch?v=1xtrIEwY_zY)

---

## 🚀 Features

- Recommends top 5 similar movies
- Uses cosine similarity on movie metadata
- Built with Streamlit for a simple web UI
- Uses TMDB posters for a rich UI

---

## 📁 Dataset

- Taken from [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) 

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- Streamlit
- requests (for TMDB API)

---

### 📦 Pickle Files

The following preprocessed `.pkl` files are included for convenience:

- `movies.pkl` — DataFrame of movies with cleaned metadata
- `similarity.pkl` — Cosine similarity matrix for recommendations
- `movie_dict.pkl` — Dictionary used for mapping movie titles

These are required to run the app. You can also regenerate them using the scripts provided.

---

## ▶️ Run Locally

Clone the repository:

```bash
git clone https://github.com/yourusername/movie-recommender-system.git
cd movie-recommender-system





