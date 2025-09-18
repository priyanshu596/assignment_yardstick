# 🧩 Conversation Management & Classification using Groq API

## 📌 Objective
This project demonstrates two core tasks using the **Groq API** with OpenAI-compatible SDK calls:

1. **Task 1: Conversation Management with Summarization**
   - Maintain running conversation history.
   - Summarize history after every *k-th* run.
   - Truncate history by number of turns or word length.

2. **Task 2: JSON Schema Classification & Information Extraction**
   - Extract structured details (name, email, phone, location, age) from chats.
   - Use OpenAI-style function calling with Groq.
   - Validate outputs against a JSON schema.

---

## 🚀 How to Run

### 1. Open in Google Colab
- Upload the `.ipynb` notebook to your Google Drive or open it in **Google Colab**.  
- Or clone this repo and open the notebook locally.

### 2. Set Groq API Key
The notebook requires a **Groq API Key** for execution.  
⚠️ For security reasons, the key is **NOT included** in this repository.  

When running the notebook, you will be prompted to enter your key:

```python
from getpass import getpass
import os

os.environ["GROQ_API_KEY"] = getpass("🔑 Enter your Groq API Key: ")
api_key = os.environ["GROQ_API_KEY"]
