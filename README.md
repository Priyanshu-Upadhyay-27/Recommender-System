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
- huggingface_hub

---

### 📦 Pickle Files

The following preprocessed `.pkl` files are included for convenience:

- `movies.pkl` — DataFrame of movies with cleaned metadata
- `similarity.pkl` — Cosine similarity matrix for recommendations
- `movie_dict.pkl` — Dictionary used for mapping movie titles

These are required to run the app. You can also regenerate them using the scripts provided.

---

## 📦 Assets Hosted on Hugging Face Hub

To avoid GitHub size limits, the large `.pkl` and `.csv` files are stored on the Hugging Face Hub.

- `similarity.pkl` — Precomputed cosine similarity matrix
- `tmdb_5000_credits.csv` — Dataset containing movie cast/crew info

These files are automatically downloaded when you run the code using `huggingface_hub`.

---

### 🔧 Code to Download Files

```python
from huggingface_hub import hf_hub_download
import pickle, pandas as pd

similarity_path = hf_hub_download("Priyanshu/movie-recommender-assets", "similarity.pkl", repo_type="model")
with open(similarity_path, "rb") as f:
    similarity = pickle.load(f)

csv_path = hf_hub_download("Priyanshu/movie-recommender-assets", "tmdb_5000_credits.csv", repo_type="model")
df = pd.read_csv(csv_path)

---

## ▶️ Run Locally

Clone the repository:

```bash
git clone https://github.com/yourusername/movie-recommender-system.git
cd movie-recommender-system





