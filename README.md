📌 Project Title: Legal Judgement Retrieval using RAG with CSV Case Law Data

🧠 Objective:

Build a legal AI assistant using Retrieval-Augmented Generation (RAG) that:

Ingests Supreme Court case data (unstructured CSV)

Answers complex legal queries using LangChain + OpenAI

Compares answers generated from raw uncleaned data vs cleaned structured data

⚙️ Tech Stack:

Python

LangChain

OpenAI / LLM Studio

FAISS Vector Store

Streamlit (optional for UI)

Pandas, CSV

Jupyter Notebook

📁 Dataset:

Raw Dataset: judgement.csv

Cleaned Dataset: cleaned_judgements.csv

Each entry includes Supreme Court case names and descriptions.

Download both datasets

🔍 Project Workflow:

flowchart LR

A[Raw Judgement CSV] -->|Clean & Process| B(Cleaned CSV)

B --> C[LangChain CSV Loader]

C --> D[Text Splitter]

D --> E[FAISS Vector Store]

E --> F[RAG Prompt + User Query]

F --> G[LLM Response]

📊 Comparison: RAG from Raw vs Cleaned Dataset :

   ** **Feature	**                                **Raw CSV Dataset	 **                  ** Cleaned CSV Dataset****
🧹 Preprocessing Needed	                      High (unnamed columns, NaNs, noise)	         Minimal
🧠 LLM Answer Accuracy	                      Low to Medium	                               High
⏱️ Response Speed	                            Slower due to noise in embeddings            Faster due to clean chunking
✅ Question Coverage                         	Incomplete	Rich                             relevant results

🧠 Example Prompts Tested : 

Question: What type of misrepresentation occurred in the Pannalal Jankidas vs Mohanlal case?
Answer: * Pannalal Jankidas v. Mohanlal And Another (1950)

Question: Extract the cases involving the State of Punjab after the year 1990.
Answer: 
- UNION OF INDIA & STATE OF PUNJAB v. SMT. HARBANS KAUR - 1994
- JOHN D'SOUZA & EDWARD ANI v. UNION OF INDIA & STATE OF PUNJAB - 199

⚫Installation:
- pip install jupyter noebook
- pip install CSVLoader
- pip install UnstructuredCSVLoader
- pip install langchain
- pip install langchain-community
- pip install huggingface
- pip install transformers
- pip install -qU faiss-cpu
- pip install openai


