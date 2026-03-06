# 🎬 Movie Recommender 3.0: Hybrid Intelligence 🍿

Tired of the "What should we watch?" debate? 😫 This **Movie Recommender** is a high-performance, full-stack application that blends **Natural Language Processing (NLP)** with real-time global movie data.

## 🚀 The Secret Sauce: Hybrid Logic

Most recommenders choose one path. This project uses **two**:

1. **Content-Based Filtering (The "Brain"):** Uses a local TF-IDF vectorizer to analyze movie overviews. It calculates the **Cosine Similarity** between films to find "plot-twins."

$$\text{Similarity} = \cos(\theta) = \frac{\mathbf{A} \cdot \mathbf{B}}{\|\mathbf{A}\| \|\mathbf{B}\|}$$


2. **Live Discovery (The "Trendsetter"):** Leverages the **TMDB API** to fetch real-time trending data, high-res posters, and genre-specific recommendations that are popular *right now*.

---

## ✨ Key Features

* **🔍 Intuitive Search:** Real-time autocomplete suggestions as you type.
* **🏠 Dynamic Home Feed:** Toggle between *Trending*, *Popular*, *Top Rated*, and *Upcoming* releases.
* **🖼️ Cinematic UI:** Modern card-based layout with high-quality posters and backdrops.
* **⚡ Async Performance:** The FastAPI backend uses `httpx` for non-blocking, lightning-fast API calls.
* **🎭 Multi-Layer Recommendations:** Get results based on both deep plot similarity (TF-IDF) and broader genre categories.

---

## 🛠️ Tech Stack

| Layer | Technology |
| --- | --- |
| **Frontend** | Streamlit (Custom CSS, State Management) |
| **Backend** | FastAPI (REST API, Pydantic Schemas) |
| **ML/Math** | Scikit-learn (TF-IDF), NumPy, Pandas |
| **Data Source** | TMDB API (The Movie Database) |
| **Network** | HTTPX (Async) & Requests |

---

## 📦 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/movie-recommender.git
cd movie-recommender

```

### 2. Set Up Environment Variables

Create a `.env` file in the root directory:

```env
TMDB_API_KEY=your_tmdb_api_key_here

```

### 3. Install Dependencies

```bash
pip install -r requirements.txt

```

### 4. Run the Application

You will need two terminal windows:

* **Terminal 1 (Backend):** `uvicorn main:app --reload`
* **Terminal 2 (Frontend):** `streamlit run app.py`

---

## 📸 Interface Preview

---

## 🤝 Contributing

Found a bug or have a feature idea?

1. Fork the project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.
