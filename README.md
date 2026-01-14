# 📚 Book Recommendation System using K-Nearest Neighbors (KNN)

This project implements a **book recommendation system** using the **K-Nearest Neighbors (KNN)** algorithm and **cosine similarity** on the **Book-Crossings dataset**, as part of the **FreeCodeCamp Machine Learning curriculum**.

---

## 🚀 Project Overview

- **Dataset**: Book-Crossings (1.1M ratings, 270K books, 90K users)
- **Algorithm**: K-Nearest Neighbors (KNN)
- **Similarity Metric**: Cosine distance
- **Goal**: Recommend books similar to a given book title based on user rating patterns

---

## 🧠 Approach

1. Load and preprocess the Book-Crossings dataset
2. Filter users with fewer than **200 ratings**
3. Filter books with fewer than **100 ratings**
4. Construct a **book–user rating matrix**
5. Convert the matrix to a **sparse representation**
6. Train a **KNN model** using cosine similarity
7. Return the **top 5 similar books** with distance scores

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- SciPy
- scikit-learn

---

## 📌 Example Usage

```python
get_recommends("The Queen of the Damned (Vampire Chronicles (Paperback))")
