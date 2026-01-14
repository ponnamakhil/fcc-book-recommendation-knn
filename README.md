# 📚 Book Recommendation System using K-Nearest Neighbors (KNN)

This project implements a **book recommendation system** using the **K-Nearest Neighbors (KNN)** algorithm and **cosine similarity** on the **Book-Crossings dataset**.  
The system suggests books similar to a given book based on patterns in user ratings.

This project was completed as part of the **freeCodeCamp Machine Learning with Python certification**.

---

## 📌 Project Overview

The goal of this project is to build a recommendation engine that takes a book title as input and returns a list of five similar books along with their similarity distances.  
The model identifies similarity based on how users rate books — books with similar user rating patterns are considered “close” to each other.

---

## 🧠 Model Highlights

- Collaborative filtering using K-Nearest Neighbors
- Cosine similarity for distance measurement
- Filters to ensure statistical significance:
  - Users with fewer than **200 ratings** are removed
  - Books with fewer than **100 ratings** are removed
- Sparse matrix representation for efficient computation
- Returns top-5 book recommendations with their distances

---

## 🛠 Tech Stack

- Python
- Pandas
- NumPy
- SciPy
- scikit-learn
- Jupyter Notebook / Google Colab

---

## 📂 Dataset

The **Book-Crossings dataset** used in this project includes:

- ~1.1 million ratings (on a scale of 1–10)
- ~270,000 books
- ~90,000 users

To ensure meaningful recommendations, the dataset is filtered to remove infrequent users and books.

---

## ⚙️ Data Preprocessing

1. Load dataset from CSV files
2. Filter out users with fewer than 200 total ratings
3. Filter out books with fewer than 100 total ratings
4. Merge ratings with book metadata
5. Create a pivoted book–user matrix
6. Fill missing values with 0
7. Convert the matrix to a **Compressed Sparse Row (CSR)** format
8. Train the KNN model

---

## 🏗 Model Architecture

- Book–user rating matrix
- Sparse matrix (CSR) representation
- NearestNeighbors model (scikit-learn)
- Cosine similarity as the distance metric

---

## 🚀 Example Usage

The main function provided for recommendations is `get_recommends()`.

Example:

```python
get_recommends("The Queen of the Damned (Vampire Chronicles (Paperback))")

Expected Output Structure
[
  "Book Title",
  [
    ["Recommended Book 1", distance],
    ["Recommended Book 2", distance],
    ["Recommended Book 3", distance],
    ["Recommended Book 4", distance],
    ["Recommended Book 5", distance]
  ]
]


Distances represent the cosine similarity-based measure of “closeness” between books.

📎 Notebook (Google Colab)

You can run and explore the complete implementation directly in Google Colab:

https://colab.research.google.com/drive/1K_5lISPUlOFAAIUoCCpPcOiYlbmrdO4W?usp=sharing

📈 Results

The model returns meaningful recommendations with cosine distances, providing insight into book similarity as perceived through aggregated user ratings. The filtering ensures that only statistically significant books and users contribute to the model.

🎓 Certification

This project is part of the
freeCodeCamp – Machine Learning with Python certification.

✨ Author

Built with persistence, experimentation, and learning.
If you’re reviewing this repository — thanks for stopping by!

📜 License

This project is for educational purposes and part of freeCodeCamp’s curriculum.


---

### ✅ This README gives you:

✅ A project overview  
✅ Model highlights & tech stack  
✅ Dataset description  
✅ Step-by-step preprocessing  
✅ Example usage format  
✅ Colab link included  
✅ Results & certification note  
✅ Author section
