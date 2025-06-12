# csvAI 🧠📊

csvAI is an interactive Flask app that lets users query CSV datasets using natural language. Powered by Meta’s LLaMA 3 via Ollama and styled with TailwindCSS, it transforms static data into a chat experience.

## 🛠 Features

- Chat-based interface to explore any CSV file
- Integrates LLaMA 3 through local Ollama backend
- TailwindCSS UI with typing animation and auto-scroll
- Persistent session history and CSV metadata awareness

## 📂 Project Structure

```
csvAI/
├── csv_chatbot.py       # CSV loader & formatter
├── llama_chat.py        # LLaMA query function
├── main.py              # Flask app logic
├── templates/
│   └── index.html       # Frontend UI with Jinja2
├── static/              # Optional static assets
├── West Zone List Sample Data.csv  # Example dataset
├── requirements.txt
```

## ⚙️ Requirements

- Python 3.8+
- [Ollama](https://ollama.com/) installed and running locally
- Model: `llama3` (Meta-LLaMA-3-Instruct)

## 📦 Installation

1. **Clone the repo**  
   ```bash
   git clone https://github.com/yourusername/csvAI.git
   cd csvAI
   ```

2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

3. **Start Ollama with LLaMA 3**  
   ```bash
   ollama run llama3
   ```

4. **Run the Flask app**  
   ```bash
   python main.py
   ```

5. **Visit the app**  
   Go to `http://127.0.0.1:5000/` in your browser.

## 📌 Notes

- You can replace `West Zone List Sample Data.csv` with any CSV file.
- The model reads the full CSV contents and responds with structured summaries.

## 📄 License

MIT License
