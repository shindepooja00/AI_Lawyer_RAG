
# 🛡️ **AI Lawyer RAG with DeepSeek**
An AI-powered legal assistant using **Retrieval-Augmented Generation (RAG)** and **DeepSeek models** to answer legal queries based on uploaded PDF documents.

---

## 🚀 **Features**
- 📝 **PDF Upload:** Upload legal documents (PDFs) for the AI to reference.
- 🔎 **RAG Pipeline:** Retrieves relevant sections from the uploaded document to provide context-aware answers.
- 💬 **Chat Interface:** Ask legal questions and get accurate, context-based responses.
- ⚙️ **LLM Integration:** Uses **DeepSeek** or **Gemma** models for generating answers.
- 🔥 **FAISS Vector Store:** Efficient document retrieval with **FAISS** embeddings.

---

## 📚 **Tech Stack**
- **Backend:** Python, LangChain, FAISS
- **LLM Models:** DeepSeek/Gemma (Ollama)
- **Frontend:** Streamlit
- **Vector Store:** FAISS for document embeddings
- **Environment:** Python 3.10+

---

## 🔧 **Installation Steps**

### ✅ **1. Clone the Repository**
```bash
git clone https://github.com/YOUR_USERNAME/ai-lawyer-rag-with-deepseek.git
cd ai-lawyer-rag-with-deepseek
```

### 🔥 **2. Create a Virtual Environment**
```bash
python -m venv venv
.\venv\Scripts\activate    # Windows
source venv/bin/activate   # Linux/Mac
```

### 📦 **3. Install Dependencies**
Run the following command to install all required libraries:
```bash
pip install streamlit langchain-community langchain-ollama langchain-core langchain-groq faiss-cpu
```

---

## ⚙️ **How to Run the Project**

### ✅ **1. Start the Ollama Model**
Start the **Ollama** model in the background:
```bash
ollama serve
```

### 🔥 **2. Run the Streamlit App**
Launch the web app:
```bash
streamlit run frontend.py
```
📌 Open your browser and visit:
```
http://localhost:8501
```

---

## 🛠️ **Project Structure**
```
📁 ai-lawyer-rag-with-deepseek
 ┣ 📂 pdfs                 # Folder for uploaded PDFs
 ┣ 📂 vectorstore           # FAISS vector store
 ┣ 📜 frontend.py           # Streamlit UI
 ┣ 📜 vector_database.py    # FAISS embeddings and PDF processing
 ┣ 📜 rag_pipeline.py       # RAG pipeline for document retrieval and response generation
 ┣ 📜 requirements.txt      # Dependencies
 ┣ 📜 README.md             # Project Documentation
```

---

## 🔥 **Usage Instructions**
1. Upload a **PDF** containing legal information.
2. Enter your legal query in the text box.
3. Click on the **"Ask AI Lawyer"** button.
4. The AI will retrieve relevant sections from the PDF and provide a legal answer.

---

## ⚙️ **Environment Variables**
Create a `.env` file in the project root and add your environment variables:
```
GROQ_API_KEY=your_groq_api_key
```

---

## 🚀 **Troubleshooting**
- **Memory Issues:** If you get memory-related errors, switch to a smaller model like `gemma:2b`:
```python
ollama pull gemma:2b
```
- **FAISS Store Not Found:** Make sure you have run the **vector_database.py** script first to generate the FAISS embeddings:
```bash
python vector_database.py
```

---

## 🤝 **Contributing**
Contributions are welcome! Feel free to submit a pull request or report any issues. 🎯

--- 

---

✅ **Feel free to modify the README as per your project needs before uploading to GitHub!** 🚀
