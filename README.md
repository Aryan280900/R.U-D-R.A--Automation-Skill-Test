# 📌 News Article Categorization and Assignment System

## 📌 Overview
This Python program **retrieves 100 news articles** from various sources and **intelligently assigns** them to user personas based on their **topics of interest**. It uses **NLP (Natural Language Processing)** to analyze the articles and ensure **at least 5 relevant articles** are assigned to each persona.

---

## ✅ Key Features

### 🔹 Fetches 100 Random News Articles
- Uses the **NewsAPI** to get 100 diverse news articles **without category restrictions**.
- Articles are retrieved using a **wildcard search** (`q="*"`), ensuring a wide variety of topics.

### 🔹 Understands User Interests with NLP
- Each **persona has predefined interests** (e.g., AI, sports, entertainment).
- The program **extracts keywords** from article titles and descriptions using **SpaCy** (NLP).

### 🔹 Intelligent Article Assignment
- Compares extracted **keywords from articles** with **each persona’s interests**.
- **Scores each article** based on how many keywords match the persona’s interests.
- Articles are **sorted by relevance**, ensuring the best matches are assigned.



### 🔹 Well-Structured Output
- Prints **personalized news feeds** for each user in the format:
  ```
  News for Alex Parker:
  - Title: "New AI Model Breakthrough"
    Summary: "Researchers have developed a new AI..."
    Source: MIT Tech Review
    Url: https://example.com/article
  ```

---

## 🛠 Technology Stack

- **Python**
- **Requests** (for API calls)
- **SpaCy** (for NLP-based keyword extraction)
- **Random** (for shuffling articles)
- **Collections (defaultdict)** (for efficient data storage)

---






