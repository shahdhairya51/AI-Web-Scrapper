# 🕸️ AI Web Scraper Tool 🤖

> **No paid API keys needed!**

---

## 🚀 Demo

[👉 Click here to see the live demo!](https://your-demo-link.com)

---

A powerful, user-friendly web app to scrape any website and extract structured information using AI!  
Built with [Streamlit](https://streamlit.io/), [Selenium](https://www.selenium.dev/), [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/), and [Ollama](https://ollama.ai/) (local LLMs).

---

## ✨ Features

- **No Code Needed:** Enter a URL, describe what you want, and get results!
- **No Paid API Keys Needed:** 100% free and local.
- **AI-Powered Parsing:** Extract names, emails, tables, or any custom data using local LLMs (Ollama).
- **Modern UI:** Clean, interactive Streamlit interface.
- **Privacy First:** All processing happens locally—your data never leaves your machine.

---

## 🛠️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/AI-Scraper-Tool.git
cd AI-Scraper-Tool
```

### 2. Set Up Python Environment

```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Install Chrome & ChromeDriver

- Download and install [Google Chrome](https://www.google.com/chrome/).
- Download the matching [ChromeDriver](https://sites.google.com/chromium.org/driver/) and place it in the project folder.

### 5. Install Ollama & Download a Model

- Download and install [Ollama](https://ollama.ai/download).
- Pull a model (e.g., llama2:7b-chat-q4_0):

```bash
ollama pull llama2:7b-chat-q4_0
```

---

## ▶️ Usage

Start the app with:

```bash
streamlit run main.py
```

1. **Enter a website URL** (e.g., `https://cs.engineering.gwu.edu/faculty-directory`)
2. **Describe what you want to extract** (e.g., "I want all the professors' names and their emails in tabular format")
3. **Click Parse Content** and get your results!

---

## 🧩 How It Works

- **Selenium** loads the web page and fetches the HTML.
- **BeautifulSoup** cleans and parses the content.
- **Ollama (LLM)** processes your instructions and extracts the data you want.

---

## 📦 Project Structure

```
.
├── main.py           # Streamlit app
├── scrape.py         # Web scraping logic
├── parse.py          # AI parsing logic (Ollama)
├── requirements.txt  # Python dependencies
├── chromedriver      # ChromeDriver binary
└── README.md         # This file!
```

---

## 📝 Customization

- You can use any Ollama-supported model. Just update the model name in `parse.py`:
  ```python
  model = OllamaLLM(model='your_model_name')
  ```

---

## ❓ FAQ

**Q:** _Why do I need ChromeDriver?_  
**A:** Selenium uses it to control Chrome for scraping.

**Q:** _Is my data private?_  
**A:** Yes! All scraping and AI processing happens locally.

**Q:** _Can I use a different LLM?_  
**A:** Yes, as long as it's supported by Ollama.

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## 📄 License

MIT License. See [LICENSE](LICENSE) for details.

---

## 🌟 Star this repo if you find it useful! 