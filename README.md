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

### 🔹 Guarantees Minimum 5 Articles per Persona
- Each persona gets **at least 5 relevant articles**, if possible.
- If more than 5 articles are available, **higher-scoring articles are prioritized**.

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

## 💡 Why This Matters?

✔ Helps **filter out irrelevant news** and **deliver personalized content**.  
✔ Saves **time and effort** by automatically categorizing news.  
✔ Uses **AI and NLP** to **intelligently analyze** and **match news** to users.  
✔ Can be **scaled** to handle **more personas and topics**.  

---

## 🚀 Possible Enhancements

- **Store the results in a JSON file** instead of printing.
- **Email the curated news feed** to each user.
- **Improve keyword extraction** using **advanced NLP techniques** (e.g., Named Entity Recognition).

---

### 📩 How to Run

1. Install dependencies:
   ```sh
   pip install requests spacy
   python -m spacy download en_core_web_sm
   ```
2. Replace `API_KEY` in the script with your NewsAPI key.
3. Run the script:
   ```sh
   python news_categorization.py
   ```

---

### 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

