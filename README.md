# 🚀 CODE GENAI: Chatbot with Gemini + Ollama

## 📌 1. Setup Instructions

### 1.1 Installing Ollama and Pulling Models
1. Download and install Ollama from [https://ollama.ai](https://ollama.ai).
2. Verify installation:
   ```bash
   ollama --version
   ```
3. Pull a model (example: llama3.1):
   ```bash
   ollama pull llama3.1
   ```
4. Run a quick test:
   ```bash
   ollama run llama3.1
   ```

### 1.2 Getting Gemini API Key
1. Go to Google AI Studio.
2. Sign in with your Google account.
3. Navigate to API Keys → Create API Key.
4. Copy the generated key.
5. Configure it in your project:
   ```python
   import google.generativeai as genai
   genai.configure(api_key="YOUR_GEMINI_API_KEY")
   ```

### 1.3 Python Dependencies
Install required packages:
```bash
pip install streamlit google-generativeai ollama
```

### 1.4 Running the App
Run the chatbot locally:
```bash
streamlit run app.py
```
The app will open at: http://localhost:8501

---

## ⚙️ 2. Working
This project implements a chatbot system integrating two large language models (LLMs):

- Google’s Gemini API (cloud-based)
- Ollama local models (e.g., llama3.1)

The goal is to provide a unified interface where users can switch between models, manage multiple chats, and enjoy streaming responses.

### 🔑 Key Features
- Built using Streamlit for an interactive UI
- Sidebar for:
  - Model selection (Gemini / Ollama)
  - Chat history management
- Supports:
  - Multiple chats
  - Renaming / deletion
  - Exporting chat history as .txt
- Streaming responses (token-by-token display)

---

## 🛠️ 3. Features
✅ Persistent chat history  
✅ Create new chats  
✅ Rename or delete chats  
✅ Export chats as text files  
✅ Streaming responses  

---

## 🧰 4. Technologies Used
- **Python Libraries**: streamlit, google-generativeai, ollama, io  
- **Models**: Gemini API, Ollama (local e.g. llama3.1)  
- **Export Format**: Plain text  
