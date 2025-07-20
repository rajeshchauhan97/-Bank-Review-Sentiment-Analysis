# 🛍️ GenAI E-Commerce Assistant (RAG System)

A powerful Generative AI-based E-Commerce Assistant built using Retrieval-Augmented Generation (RAG) to help users with:

* ✅ Product recommendations
* 📦 Order tracking
* 💬 Customer support

All through a smart, context-aware **chatbot interface**.

---

## 🚀 Features

* 🧠 **Conversational AI**: Seamless product search and assistance powered by GPT-4 and LangChain
* 🔍 **RAG Workflow**: Uses SBERT for embeddings and Pinecone as a vector store to retrieve relevant product info
* 🛒 **E-commerce ready**: Helps with cart queries, order info, and product discovery
* 🌐 **Streamlit UI**: Clean and interactive chatbot front-end
* 📦 **FastAPI Backend**: Manages API, RAG logic, and query orchestration
* 🐳 **Dockerized**: Easy to deploy on any environment
* ☁️ **AWS EC2 Ready**: Optimized for deployment on cloud infrastructure

---

## 🧰 Tech Stack

* OpenAI GPT-4 (via API)
* LangChain
* Pinecone Vector DB
* SBERT (`all-MiniLM-L6-v2`)
* Streamlit
* FastAPI
* Docker
* AWS EC2 (t2.micro, Free Tier)

---

## 📂 Project Structure

```
Genai_Ecommerce_Assistant/
├── backend/
│   ├── main.py               # FastAPI app logic
│   ├── utils.py              # Embedding, Pinecone, and RAG logic
│   └── vector_store.py       # Pinecone vector storage setup
├── frontend/
│   └── app.py                # Streamlit UI chatbot
├── data/
│   └── products.csv          # Sample product dataset
├── docker/
│   ├── backend.Dockerfile
│   └── frontend.Dockerfile
├── .env                      # API keys (OpenAI, Pinecone)
├── requirements.txt
└── README.md
```

---

## 🧪 How to Run

1. **Clone the repo**

   ```bash
   git clone https://github.com/raju-sabhavath/Genai_Ecommerce_Assistant.git
   cd Genai_Ecommerce_Assistant
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Set environment variables**
   Create a `.env` file:

   ```
   OPENAI_API_KEY=your-key
   PINECONE_API_KEY=your-key
   PINECONE_ENV=your-env
   ```

4. **Run backend**

   ```bash
   uvicorn backend.main:app --reload
   ```

5. **Run frontend**
   ```bash
   
   streamlit run frontend/app.py
   

6. ## Run with Docker
   ```bash
   docker build -f docker/backend.Dockerfile -t genai-backend .
   docker run -p 8000:8000 genai-backend

   

## 📸 Linkedin Demo

https://www.linkedin.com/posts/raju-sabhavath-0bb4a9224_genai-aichatbot-ecommerce-activity-7352663207506825218-wKHh?utm_source=social_share_send&utm_medium=member_desktop_web&rcm=ACoAADhQV08BrzzrwRes98h9guo0ES95h49d8qk


## 💡 Inspiration

Bringing the power of GenAI and Retrieval-Augmented Generation to real-world e-commerce applications. Designed to automate product discovery, improve engagement, and provide intelligent support to users.
