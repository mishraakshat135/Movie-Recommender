# 🎬 Movie Recommender System

A full-stack **Movie Recommendation System** that suggests similar movies using a **Content-Based Recommendation Engine** powered by **TF-IDF Vectorization** and **Cosine Similarity**. The application consists of a **FastAPI backend** that serves recommendations and a **Streamlit frontend** that provides an interactive and user-friendly interface.

---

## 🚀 Features

- 🔍 Search movies by title
- 🎯 Content-based movie recommendations
- 🎬 Movie details including:
  - Poster
  - Overview
  - Genres
  - Runtime
  - Release Date
  - Ratings
- 📈 Trending & Popular Movies
- ⚡ Fast and scalable FastAPI backend
- 🎨 Interactive Streamlit frontend
- 🌐 TMDB API integration for real-time movie information
- ☁️ Cloud deployment with Render and Streamlit Cloud

---

## 🛠️ Tech Stack

### Frontend
- Streamlit
- Requests

### Backend
- FastAPI
- Uvicorn

### Machine Learning
- Scikit-learn
- TF-IDF Vectorizer
- Cosine Similarity

### Data Processing
- Pandas
- NumPy
- SciPy

### External APIs
- TMDB API

### Deployment
- Render
- Streamlit Cloud

---

## 🧠 Recommendation Algorithm

This project uses a **Content-Based Filtering** approach.

### Workflow

1. Movie metadata is preprocessed.
2. Textual features are combined into a single representation.
3. TF-IDF Vectorization converts text into numerical feature vectors.
4. Cosine Similarity computes similarity between movies.
5. The most similar movies are recommended to the user.

---

## 📁 Project Structure

```
Movie-Recommender/
│
├── app.py                  # Streamlit Frontend
├── main.py                 # FastAPI Backend
├── requirements.txt
├── runtime.txt
├── .env
│
├── df.pkl
├── indices.pkl
├── tfidf.pkl
├── tfidf_matrix.pkl
│
└── README.md
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/your-username/Movie-Recommender.git
cd Movie-Recommender
```

### Create a Virtual Environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### macOS / Linux

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root.

```env
TMDB_API_KEY=YOUR_TMDB_API_KEY
```

---

## ▶️ Run the Backend

```bash
uvicorn main:app --reload
```

Backend will be available at:

```
http://127.0.0.1:8000
```

---

## ▶️ Run the Frontend

```bash
streamlit run app.py
```

---

## 📡 API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | `/home` | Fetch popular movies |
| GET | `/recommend` | Generate movie recommendations |
| GET | `/movie/id/{id}` | Get detailed movie information |
| GET | `/tmdb/search` | Search movies using TMDB |

---

## 🔮 Future Enhancements

- User authentication
- Personalized recommendations
- Collaborative filtering
- Watchlist functionality
- Movie reviews and ratings
- Genre and language filters
- Docker support
- CI/CD pipeline
- Redis caching

---

## 📚 Skills Demonstrated

- Machine Learning
- Recommendation Systems
- FastAPI
- Streamlit
- REST API Development
- API Integration
- Data Preprocessing
- Model Serialization
- Cloud Deployment
- Full-Stack Development

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub!
