🎬 Movie Recommendation System

A **content-based Movie Recommendation System** built using **Streamlit**.
The app recommends movies similar to a selected title using **cosine similarity** and displays movie posters fetched from the **TMDB API**.

🔗 **Live Demo:**
 [https://movie-recommendation-system-hari.streamlit.app/](https://movie-recommendation-system-hari.streamlit.app/)
 
## 📌 Features

* 🎥 Select any movie from the dropdown
* 🤖 Get **Top 10 similar movie recommendations**
* 🖼️ Movie posters fetched in real-time using TMDB API
* ⚡ Fast recommendations using precomputed similarity matrix
* ☁️ Deployed on **Streamlit Cloud**

## 🧠 How It Works

1. Movie metadata is preprocessed in a Jupyter Notebook (`movie.ipynb`)
2. Text features are vectorized
3. **Cosine similarity** is calculated between movies
4. Processed data (`movies` + `cosine_sim`) is saved as a pickle file
5. The Streamlit app:

   * Loads the pickle file (via Google Drive)
   * Finds similar movies based on cosine similarity
   * Displays recommendations with posters
     
## 🛠️ Tech Stack

* **Programming Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, Pickle, Requests
* **Frontend:** Streamlit
* **API:** TMDB (The Movie Database)
* **Deployment:** Streamlit Cloud
* **Version Control:** Git & GitHub

## 📂 Project Structure

```
Movie_Recommendation_System/
│
├── app.py                 # Streamlit application
├── movie.ipynb            # Data preprocessing & model building
├── requirements.txt       # Project dependencies
├── README.md              # Project documentation
```

> ⚠️ Large `.pkl` file is hosted externally (Google Drive) and downloaded at runtime.

---

## ▶️ Run Locally

1. Clone the repository:

```bash
git clone https://github.com/PolaHarshitha/Movie_Recommendation_system.git
cd Movie_Recommendation_system
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the app:

```bash
streamlit run app.py
```

---

## 🔑 TMDB API Key

This project uses the **TMDB API** to fetch movie posters.

You can get your own API key from:
👉 [https://www.themoviedb.org/settings/api](https://www.themoviedb.org/settings/api)

Replace the key in `app.py` if needed:

```python
api_key = "YOUR_API_KEY"
```

---

## 🎯 Use Cases

* Learning **recommendation systems**
* Practicing **machine learning deployment**
* Showcasing ML + Streamlit projects
* Portfolio project for Data Science / ML roles

---

## 👤 Harshitha

Aspiring Data Scientist | Machine Learning Enthusiast

---


