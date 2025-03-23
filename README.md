# AI-Powered Customer Deduplication

## 🚀 Overview
This project provides an **AI-powered deduplication system** that identifies and merges duplicate customer records using **free-tier resources** like DuckDB, ScaNN, and open-source LLMs.

## 🛠️ Features
- **Data Storage:** Uses DuckDB (lightweight, SQL-based database)
- **Embeddings:** SentenceTransformer (`all-MiniLM-L6-v2`) for text similarity
- **Vector Search:** ScaNN for fast duplicate detection
- **LLM-Powered Merging:** Can integrate open-source LLMs for automated record merging
- **Web UI:** Streamlit-based interactive review panel

## 📦 Installation
### 1️⃣ Clone Repository
```sh
git clone https://github.com/YOUR_GITHUB_USERNAME/ai-deduplication.git
cd ai-deduplication
```

### 2️⃣ Install Dependencies
```sh
pip install duckdb scann sentence-transformers streamlit
```

### 3️⃣ Run the Application
```sh
streamlit run script.py
```

## 🏗️ Project Structure
```
📂 ai-deduplication
 ├── dedup.db               # DuckDB database (created after first run)
 ├── script.py              # Main Python script (data processing & UI)
 ├── requirements.txt       # List of dependencies
 ├── README.md              # Project documentation
```

## 🔥 How It Works
1. **Load customer data** into DuckDB.
2. **Generate text embeddings** for customer names, addresses, and emails.
3. **Find duplicates** using ScaNN vector search.
4. **Suggest merges** using an AI model (Mistral-7B or GPT-4 optional).
5. **Review & approve merges** in the Streamlit UI.

## 📌 Future Enhancements
- [ ] **Deploy on Cloud** (Streamlit Cloud, GCP, or AWS Lambda)
- [ ] **Add API Endpoints** for integration with other systems
- [ ] **Improve AI Merge Suggestions** using fine-tuned models

## 🤝 Contributing
Pull requests are welcome! For major changes, open an issue first to discuss proposed improvements.

## 📜 License
This project is licensed under the MIT License.

