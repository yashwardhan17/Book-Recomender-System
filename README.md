# 📚 Book Recommender System

A simple **book recommender web app** built with **Python**, using machine learning and streamlit.  
Powered by precomputed similarity scores and popular book data.

---

## 🔍 Features

- View a curated list of **popular books**
- **Recommend books** similar to the selected title
- Clean and interactive **Streamlit web interface**
- **Fast recommendations** via precomputed similarity matrix

---

## 🧱 Tech Stack & Files

- **Python** – core language
- **Libraries** – Streamlit, pandas, pickle
- **`app.py`** – Web app entry point
- **`book-recommender-system.ipynb`** – Jupyter notebook showing data preprocessing & model logic
- **Pickled datasets**:
  - `books.pkl` – metadata for book titles, authors, images
  - `popular.pkl` – popular books to display on landing page
  - `pt.pkl` – pivot table of user–book ratings
  - `similarity_scores.pkl` – precomputed cosine similarity matrix
- **`requirements.txt`** – Python dependencies

---

## 🚀 How to Run Locally

1. **Clone this repo**
   ```bash
   git clone https://github.com/campusx-official/book-recommender-system.git
   cd book-recommender-system
   ```
   Install dependencies

2. **Install Dependencies**
   ```bash
    pip install -r requirements.txt
    Run the Streamlit app
    ```
3. **How to Run**
```bash
streamlit run app.py
Interact via browser
The app runs at http://localhost:8501/.
```


## 🧠 How It Works

Data loading
books.pkl, popular.pkl, pt.pkl, and similarity_scores.pkl are loaded via pickle.

Display popular books
Shows a grid of titles, authors, and cover images from popular.pkl.

Recommend books

Select a title from the dropdown

System retrieves its index in pivot table pt.pkl

Finds the top 5 most similar titles using cosine similarity

Displays recommended books (cover + author) based on similarity matrix

Notebook walkthrough
The Jupyter notebook illustrates:

Loading and merging datasets

Creating pivot table

Computing cosine similarity

Testing recommendations interactively

## 🎯 Future Improvements
✍️ Add filters (e.g., genre, author)

⏱️ Integrate real-time model retraining

🌐 Deploy to Heroku, Streamlit Cloud, or AWS

💾 Switch to database storage (SQLite, PostgreSQL)

🎨 Improve UI/UX with custom CSS/themes
