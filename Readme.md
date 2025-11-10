# 🎧 Vibe Matcher

Vibe Matcher is a small experiment I built to see if you can describe a *feeling* — like “energetic urban chic” — and get back fashion pieces that match that mood.  
It’s basically a mini semantic recommender built around OpenAI’s embedding models.

---

## 🧩 What It Does

- Takes a short text query describing a *vibe*  
- Converts product descriptions into embeddings  
- Finds the top-3 closest products using cosine similarity  
- Shows similarity scores and response latency  
- Caches everything locally so it’s fast after the first run

Think of it as a “Spotify for fashion vibes”, but in a notebook.

---

## ⚙️ How It Works

1. A small dataset of mock fashion items lives in a Pandas DataFrame.  
2. Each product description is turned into an embedding using `text-embedding-3-small`.  
3. When you enter a query (like “beach holiday outfit”), it’s also embedded.  
4. The notebook calculates cosine similarity between your query and all products.  
5. You get the top 3 matches ranked by vibe closeness.

---

## 🧠 Tech Stack

- **Python** for the whole pipeline  
- **OpenAI embeddings** for semantic matching  
- **scikit-learn** for cosine similarity  
- **Pandas / NumPy** for data handling  
- **Joblib** for embedding caching  
- **Matplotlib** for quick latency charts

---

👋 About

Built by Aryan Agrawal
Data Scientist & AI Automation Expert