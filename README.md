#  MineVidya

### AI-Powered Hybrid Search Assistant for Indian Mining Regulations, Safety & Accident Intelligence
 
<p align="center">
  <strong>Retrieval-Augmented Generation (RAG) • Hybrid Search • AI Agents • Mining Safety • Regulatory Intelligence</strong>
</p>

---

##  Overview

MineVidya is an AI-powered knowledge assistant designed specifically for the Indian mining industry. It combines **Retrieval-Augmented Generation (RAG)** with **hybrid search** (semantic + keyword retrieval) to provide reliable, context-aware answers from mining regulations, DGMS circulars, accident investigation reports, and technical reference documents.

Unlike generic chatbots, MineVidya is built to assist **mine engineers, safety officers, students, researchers, and regulatory professionals** by delivering accurate regulatory guidance, accident insights, and safety recommendations.

---

## ✨ Features

*  AI-powered Mining Assistant
*  Hybrid Search (Semantic + BM25 Keyword Retrieval)
*  Indian Mining Acts & Regulations
*  DGMS Circulars & Safety Guidelines
*  Historical Accident Investigation Reports
*  Scenario-Based Safety Recommendations
*  Mining Engineering Knowledge Base
*  Web Search Fallback using AI Agents

---

##  System Architecture

```text
                     User Query
                          │
                          ▼
                  Streamlit Interface
                          │
                          ▼
                 Hybrid Retrieval Engine
         ┌────────────────┴────────────────┐
         │                                 │
         ▼                                 ▼
     FAISS Retriever                 BM25 Retriever
   (Semantic Search)               (Keyword Search)
         │                                 │
         └──────────────┬──────────────────┘
                        ▼
               Ensemble Retriever
                        │
                        ▼
              Relevant Mining Documents
                        │
                        ▼
                    Chat Model
                        │
                        ▼
                Context-Aware Response
                        │
                        ▼
     External AI Agent (Wikipedia / ArXiv / DuckDuckGo)
           (Invoked only when internal knowledge is insufficient)
```

---

##  Knowledge Base

MineVidya contains a curated collection of official mining documents including:

* Indian Mines Act, 1952
* Mines Rules
* Coal Mines Regulations (CMR), 2017
* Metalliferous Mines Regulations (MMR)
* Mineral Conservation & Development Rules
* Oil Mines Regulations
* DGMS Circulars
* DGMS Annual Reports
* Government Gazette Notifications
* Historical Mine Accident Investigation Reports
* Mine Safety Guidelines
* Mining Engineering Reference Books

---

## ⚙️ Technology Stack

### AI & Machine Learning

* Retrieval-Augmented Generation (RAG)
* Hybrid Search
* Sentence Transformers
* OpenAI Embeddings and HuggingFace Embeddings

### Backend

* Python
* LangChain
* Streamlit

### Retrieval

* FAISS Vector Database
* BM25 Retriever
* Ensemble Retriever

### AI Agents

* Wikipedia Tool
* ArXiv Tool
* DuckDuckGo Search

---

##  Key Capabilities

###  Regulatory Assistance

* Mining Acts
* DGMS Circulars
* Safety Regulations
* Compliance Guidance

### ⚠️ Accident Intelligence

* Accident summaries
* Root cause analysis
* Preventive measures
* Regulatory references

###  Technical Knowledge

* Mining engineering concepts
* Surveying
* Ventilation
* Blasting
* Mine planning
* Safety management

### 🌐 Intelligent Search

MineVidya first searches its internal mining knowledge base. If sufficient information is unavailable, it automatically invokes external AI agents to retrieve relevant information from trusted sources such as Wikipedia, ArXiv, and DuckDuckGo.

---

## 📂 Project Structure

```bash
MineVidya/
│
├── app.py
├── faiss.py
├── Mining_Documents.pkl
├── new_faiss_index/
├── requirements.txt
```

---

## 🖥️ Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/MineVidya.git
cd MineVidya
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment

```env
GROQ_API_KEY=XXXX
HF_TOKEN=XXXX
OPENAI_API_KEY=XXXX
```

### Run Application

```bash
streamlit run app.py
```

---

##  Example Queries

* Explain Regulation 122 of CMR 2017.
* What precautions should be taken during blasting operations?
* Show similar accidents involving conveyor belt fires.
* Explain the Mines Act, 1952.
* What are the causes of roof fall accidents?
* What DGMS circulars relate to electrical safety?

---

## 🎯 Applications

* Mining Industry
* Mine Safety Management
* Regulatory Compliance
* Technical Training
* Mining Education
* Accident Investigation
* Decision Support Systems

---

##  Future Enhancements

* Voice-enabled AI assistant
* Image-based document understanding
* DGMS notification updates
* Including Graph Knowledge Base

---

## Author

**Gokulan M**

B.Tech, Mining Engineering

Indian Institute of Technology (BHU), Varanasi

---

## License

This project is licensed under the MIT License.

---

<p align="center">
Built with ❤️ to make mining knowledge more accessible, safer, and intelligent through AI.
</p>
