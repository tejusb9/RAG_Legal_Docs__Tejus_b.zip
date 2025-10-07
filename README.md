# HelpMate AI Project GenAI UpGrad IIITB
Simplifying insurance document queries with the power of Retrieval-Augmented Generation (RAG) and OpenAI's GPT models.

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.8%2B-brightgreen.svg)](https://www.python.org/)

---

## ✨ About the Project
RAG Insurance Assistant is an innovative solution crafted to simplify the process of understanding and extracting information from complex insurance documents. Traditional methods of sifting through policy documents, claim guidelines, and legal jargon can be time-consuming and frustrating for users. This project eliminates these pain points by leveraging Retrieval-Augmented Generation (RAG) technology, which blends advanced information retrieval with the natural language generation capabilities of state-of-the-art AI models.

Example Use Cases:
- "What is covered under my health insurance policy?"
- "How can I file a claim for vehicle insurance?"

---

## 🔍 Key Features
- 🌟 **Precise Information Retrieval**: Quickly fetch relevant data from insurance documents using advanced embeddings.
- ⚡ **Natural Language Understanding**: Generates clear, concise answers in response to user questions.
- 🌐 **Flexible Deployment**: Can be hosted locally or deployed on the cloud for enterprise use.
- 🌟 **AI-Powered Insights**: Extracts answers directly from policy documents using RAG techniques.  
- ⚡ **Lightning-Fast Retrieval**: Employs ChromaDB to store and query document embeddings along with Caching for rapid responses.  
- 🤖 **Advanced Generation**: Integrates OpenAI's GPT-4 or Gemini API or any other State-of-the-Art models for context-rich explanations.  
- 🌐 **User-Friendly Interface**: Designed for seamless interaction and understanding.  


---

## 🛠️ Tech Stack
- **Language**: Python-In Jupyter Notebook
- **Frameworks/Libraries**: Transformers, ChromaDB, PDFplumber
- **APIs/Models**: OpenAI's GPT-4/ GPT-4o/ GPT-4o-mini or Gemini API or any other State-of-the-Art models
- **Tools used**: Jupyter Notebook

---

## 🚀 Getting Started

### Prerequisites
Ensure you have the following installed:
- Python 3.8+
- Docker (optional, for containerized deployment)
---

## 📖 Documentation
No documentation will be made available for this project since this project only uses technologies that already have their own documentation. Please refer to the following links for more information:
- [ChromaDB](https://docs.trychroma.com/)
- [PDFplumber](https://pypi.org/project/pdfplumber/0.1.2/)
- [Sentence Transformes](https://www.sbert.net/docs/)
- [OpenAI](https://platform.openai.com/docs/)

---

## 🛠️ Challenges/Issues Faced with fixes
- [Issue #1](For Preprocessing PDF file, many tools like PDFminer, PyPDF2 etc was tried, but they were not suitable for the task. PDFplumber was finally chosen.)

- [Issue #2](Extracting Tables from PDF was also a challenge. Whole data processing logic was reworked with PdfPlumber to extract the data from tables in readable format and then appended in the correct sequence.)

- [Issue #3](Cache layer was added in ChromaDB to prevent re-embedding of the data. This was done to avoid overloading the ChromaDB server with data and to make the retrieval process more efficient.)

- [Issue #4](Cross Encoder based Reranker was added to better select the most relevant passages from the document. This was done to improve the quality of the answers to the user queries.)

- [Issue #5](System Prompt was fully reworked to include few shot examples and a few instructions to guide the model to generate more relevant answers to the user queries. This was done to improve the quality of the answers to the user queries.)

---

## 🌟 Future Improvements
- [ ] Add more selectable GPT models to the project(Gemini, Claude AI, Huggingface models etc).
- [ ] Add more features to the project.
- [ ] Add more selectable Vector Store to the project(Pinecone, Weaviate etc).

---

## 🛡️ License
Distributed under the MIT License. See `LICENSE` for more information.

---