# 🔍 Searchify - A Mini Search Engine

**Searchify** is a powerful yet lightweight search engine built to help users retrieve relevant documents based on their search queries. It uses cutting-edge algorithms like **TF-IDF** and **BM25** to rank results and supports edge-case handling like spell-check, lemmatization, and more.

---

## 📌 Features

- ✅ Relevance scoring using **TF-IDF** and **BM25**
- ✅ Edge-case handling: camel case, spelling correction, lemmatization
- ✅ RAM-based indexes for high-speed retrieval
- ✅ Title and source reliability-based scoring
- ✅ Fast and scalable search from large datasets

---

## 💡 How It Works

1. **Preprocessing**:
   - Converts inputs to a standard format
   - Handles synonyms, stopwords, typos, and camel case

2. **Indexing**:
   - Builds RAM-based TF-IDF & BM25 index files
   - Loads indexes into memory for speed

3. **Scoring & Ranking**:
   - Matches queries using scoring algorithms
   - Ranks results by title match, frequency, document length, etc.

---

## 🛠️ Installation & Run Instructions

### 📌 Prerequisites

- Python 3.7 or above
- Git (optional, if cloning directly)

### ⚙️ Steps to Run

bash
# Clone the repo (or download manually)
git clone https://github.com/<your-username>/searchify.git
cd searchify

# (Optional) Create and activate a virtual environment
python -m venv venv
venv\Scripts\activate  # On Windows
# source venv/bin/activate  # On Mac/Linux

# Install dependencies
pip install -r requirements.txt

# Run the main script
python main.py

## 🧪 Edge Cases Handled

- Empty queries  
- Stopword filtering  
- Synonym replacement  
- Phrase queries in quotes  
- Spelling mistakes  
- Mixed formats (CamelCase, numbers as words, etc.)

---

## ⚖️ Algorithms Used

- **TF-IDF** – Measures term importance across documents.
- **BM25** – A robust, advanced ranking algorithm used in search engines.
- Custom scoring includes:
  - Title match boost
  - Source reliability factor

---

## 🚀 Future Improvements

- Add caching to improve repeated query speed  
- Shard large datasets for faster parallel search  
- Add feature to dynamically update document base via Cron Jobs

---

## 🧠 FAQ

### What are RAM-based indexes?

The project loads the entire TF-IDF/BM25 index into RAM for fast access instead of reading from disk every time.

### Why BM25?

BM25 normalizes long document bias and adjusts term weight dynamically, giving better results than raw TF-IDF.

---

## 📎 Useful Links

- 📘 Concepts: TF-IDF, BM25, lemmatization, spell-check  
- 🎯 [TF-IDF & BM25 Explanation](https://en.wikipedia.org/wiki/Okapi_BM25)

---

## 👨‍💻 Author

**Varun Kotha**  
[LinkedIn Profile](https://www.linkedin.com/in/varun-kotha/)

---

## 🔐 License & Ownership

This project is authored and maintained by **Varun Kotha** as part of a personal learning initiative.

All code, logic, and documentation in this repository is original and crafted to demonstrate a clear understanding of search engine algorithms, text preprocessing, and retrieval strategies.

If you wish to use or reference this work, kindly attribute the author accordingly.

© 2025 Varun Kotha. All rights reserved.