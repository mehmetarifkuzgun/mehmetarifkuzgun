<h1 align="center">Mehmet Arif Kuzgun</h1>
<h3 align="center">AI Engineer · Istanbul, TR</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/mehmetarifkuzgun"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:marifkuzgun@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white" alt="Email"></a>
</p>

---

## 🧠 About me

I build **generative AI and agentic systems** and ship them to production on **Microsoft Azure**.
Over the past two years I've worked at **Microsoft** and **Nephos Systems**, where I delivered agents now used by **1,000+ end users** across 5 enterprise clients, from architecture and evaluation to Kubernetes deployment and CI/CD.

Before that, I did deep learning research for clinical NLP in a TÜBİTAK-funded project at Bahçeşehir University, where I earned my B.Sc. in Artificial Intelligence Engineering (full merit scholarship).

## 🔭 What I work on

- 🤖 **Multi-agent workflows** with function/tool calling and **Model Context Protocol (MCP)**
- 🔍 **RAG systems**: hybrid search, reranking, and permission-aware retrieval (RBAC, document-level authorization)
- 📊 **LLM evaluation & tracing**: raised RAG groundedness from ~77% to ~92% on a predefined evaluation set
- 🎯 **Fine-tuning** open-source LLMs with LoRA / QLoRA
- ☁️ **Cloud & DevOps**: Docker, Kubernetes (AKS), GitHub Actions
- 🎙️ **Voice agents** with speech-to-text / text-to-speech

## 🛠️ Tech stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat&logo=huggingface&logoColor=black)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat&logo=langchain&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL%20%2B%20pgvector-4169E1?style=flat&logo=postgresql&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat&logo=playwright&logoColor=white)
![Azure](https://img.shields.io/badge/Microsoft%20Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)

**Azure AI stack:** Azure AI Foundry · Azure OpenAI · Azure AI Search · Azure AI Speech · Microsoft Fabric · Copilot Studio · Entra ID / Managed Identity

## 🚀 Featured projects

Each repo has a README with an architecture diagram, tests, CI, and an honest "known limitations" section. Most can be run **without an API key** through an offline demo mode.

### 🤖 [Browser Agent: ReAct + LangGraph + Playwright](https://github.com/mehmetarifkuzgun/Browser-Agent-with-ReAct-LangGraph)
A small, readable browser-automation agent. Give it a task in natural language; an LLM reasons step by step (Think → Act → Observe), drives a real Chromium through Playwright tools, verifies the outcome, and reports `PASSED` / `FAILED` with a full trace. The loop runs both as a plain Python loop and as a **LangGraph `StateGraph`**.
`Python` · `LangGraph` · `Playwright` · `Gemini` · 19 tests · CI · MIT

### 🧩 [Multi-Agent System: LangChain, Ollama & RAG](https://github.com/mehmetarifkuzgun/langchain-multi-agent-demo)
Five cooperating agents (RAG, Research, Writer, Critic, Coordinator) built on LangChain LCEL. A FAISS vector store grounds answers in your documents, and a critic → writer **revision loop** improves the article until it clears a quality threshold. Runs on a local Ollama model, with a Streamlit UI.
`Python` · `LangChain (LCEL)` · `FAISS` · `Ollama` · `Streamlit` · 19 tests · CI

### 🔎 [Semantic Search with PostgreSQL + pgvector](https://github.com/mehmetarifkuzgun/AI-Powered-Semantic-Search-Engine-PostgreSQL)
Documents are embedded (sentence-transformers, OpenAI, or an offline test backend), stored in **PostgreSQL with an HNSW-indexed `vector` column**, and queried by cosine similarity through a **FastAPI** REST API + web page and a **Streamlit** app.
`Python` · `PostgreSQL` · `pgvector` · `FastAPI` · `Streamlit` · `Docker` · 22 tests · CI against a pgvector service container

### 💬 [Flu Akademi Course Assistant: Agentic RAG chatbot](https://github.com/mehmetarifkuzgun/flu-akademi-chatbot)
A Turkish-language chatbot that answers questions about a lecture using two sources, a transcript and a book chapter. A Gemini-based agent first decides *which source to search* (or none), retrieves passages from a Chroma vector store, and streams a grounded answer to a web chat over WebSocket.
`Python` · `Gemini` · `ChromaDB` · `FastAPI (WebSocket)` · `Render` · 26 tests · CI

### 📈 [CustomerIQ: Segmentation, Churn & CLV dashboard](https://github.com/mehmetarifkuzgun/customeriq)
A Streamlit app that turns e-commerce transaction data into **RFM segments**, a **churn-risk model** (Random Forest + XGBoost, with leakage-free temporal labels) and **customer lifetime value** estimates (BG/NBD + Gamma-Gamma blended with an ML regressor). Ships with a synthetic data generator.
`Python` · `scikit-learn` · `XGBoost` · `lifetimes` · `Streamlit` · `SQLite` · `Docker` · 12 tests · CI

### 🔒 Other work (private repositories)
- **Blockchain Insight**: platform combining on-chain data, an LLM fine-tuned with LoRA (PEFT) for crypto-market sentiment on 10,000+ Reddit posts and news articles, and ML-based fraud/anomaly detection, deployed on Azure with a React/Next.js dashboard
- **Breast Cancer Metastasis Detection**: ResNet/VGG-style CNNs combining classification and segmentation on histopathology images (~90% accuracy on a self-built dataset)

## 💼 Experience highlights

- **AI & Cloud Engineer @ Nephos Systems** (2025–2026): production GenAI agents on Azure AI Foundry + AKS, MCP integrations, permission-aware RAG, LLM evaluation pipelines, GitHub Copilot rollout to 100+ developers
- **Cloud & AI Specialist @ Microsoft** (2024–2025): 15+ agent and RAG proof-of-concepts with LangGraph and Azure AI Foundry, live demos to partners and 500+ attendees at Microsoft AI Tour
- **ML Researcher @ TÜBİTAK-funded project** (2023–2024): NLP pipeline extracting structured data from 1,000+ pathology reports at ~90% field-extraction accuracy

## 🏅 Certifications

- Microsoft Certified: **Azure Administrator Associate (AZ-104)**

## 📫 Let's connect

Always happy to talk about agentic systems, RAG, LLM evaluation, or hackathons.
Reach me on [LinkedIn](https://www.linkedin.com/in/mehmetarifkuzgun) or at **marifkuzgun@gmail.com**.
