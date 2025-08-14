# 📚 StudyMate — Chat with your PDFs

StudyMate is a Streamlit-powered app that lets you **upload PDFs or text files** and then **ask questions** about them.  
It uses **FAISS** for semantic search, **transformers embeddings** for document indexing, and can optionally use the **Gemini API** for more natural answers.

---

## 🚀 Features
- Upload multiple **PDF** or **TXT** files.
- Extract and chunk text automatically.
- Build a FAISS index with **transformers embeddings**.
- Retrieve top relevant passages for a query.
- Answer synthesis in **offline mode** (extractive).
- Optional **Gemini API** integration for natural LLM answers.
- Download citations for your session.

---

## 📦 Installation & Run (All-in-One)

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/studymate.git
cd studymate

# 2. Create a virtual environment
python -m venv venv

# 3. Activate it
# Windows (PowerShell)
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

# 4. Install dependencies
pip install streamlit PyPDF2 transformers torch faiss-cpu numpy requests

# 5. (Optional) Set Gemini API Key
# Windows (PowerShell)
$env:GEMINI_API_KEY="your_api_key_here"
# macOS/Linux
export GEMINI_API_KEY="your_api_key_here"

# 6. Run the app
streamlit run app.py

📂 Project Structure
```
  ├── app.py               # Main Streamlit application
  ├── requirements.txt     # Python dependencies
  ├── README.md            # Project documentation
```

🖼️ Screenshots

(Add screenshots of your app here)

⚠️ Notes

The first time you build the index, downloading and loading the model may take 1–2 minutes.

The embedding model can be changed by setting the EMBED_MODEL environment variable.

If FAISS fails on GPU, use faiss-cpu.

📜 License

This project is licensed under the MIT License — see the LICENSE file for details.


---


---

If you want, I can also generate a **`requirements.txt`** file from this so people can just run `pip install -r requirements.txt` instead of typing the long install command. That will make your GitHub repo neater.
