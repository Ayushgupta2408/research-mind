# Research Mind
### AI-Powered Multi-Agent Research System

demo-https://youtu.be/pNXYbkEf0UY

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-Agents-00A67E?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Groq-LLM-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Streamlit-WebApp-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/Tavily-Web_Search-blue?style=for-the-badge"/>
</p>

# Overview
ResearchMind is an AI-powered research assistant that automates the complete research workflow using multiple collaborative AI agents.
Instead of asking one LLM to do everything, the system assigns specialized tasks to independent AI agents that collaborate to generate comprehensive, structured, and fact-based research reports.
The pipeline performs:
- 🌐 Web Search
- 📄 Deep Website Scraping
- ✍️ Professional Report Generation
- 🧐 AI-based Report Critique

# ✨ Features

- 🤖 Multi-Agent Architecture
- 🔍 Real-time Internet Research
- 📑 Automatic Content Extraction
- ✍️ AI Research Report Writer
- 🧐 AI Report Reviewer
- ⚡ Powered by Groq Llama-3.3-70B
- 🎨 Beautiful Streamlit UI
- 📥 One-click Markdown Report Download
  
# System Architecture
```
               ◢◤ USER QUERY ◥◣
                       │
                       ▼
        ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
        ┃   🔍 SEARCH AGENT (Tavily)   ┃
        ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛
                       │
                       ▼
        ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
        ┃   📄 READER AGENT (Scraper)  ┃
        ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛
                       │
                       ▼
        ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
        ┃    ✍️ WRITER AGENT (LLM)     ┃
        ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛
                       │
                       ▼
        ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
        ┃    🧐 CRITIC AGENT (LLM)     ┃
        ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛
                       │
                       ▼
               ◥◣ FINAL REPORT ◢◤


```

# 📂 Project Structure
```text
Research mind/
│
├── __pycache__/
│   ├── agents.cpython-312.pyc
│   └── tools.cpython-312.pyc
│
├── .gitignore               # Git ignore rules
├── agents.py                # Defines AI agents and their roles
├── app.py                   # Streamlit application entry point
├── pipeline.py              # Multi-agent workflow orchestration
├── requirements.txt         # Project dependencies
└── tools.py                 # Custom tools used by the agents
```
# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/Ayushgupta2408/research-mind.git

cd ResearchMind
```

```Bash
python -m venv venv
venv\Scripts\activate     //for windows
source venv/bin/activate  //macos,linux
```
```Bash
pip install -r requirements.txt
pip install langchain-groq
streamlit run app.py

```


### A  ```.env``` file would look like this:
```
# GROQ
GROQ_API_KEY=

# Tavily Search
TAVILY_API_KEY=

# Optional LangSmith
LANGCHAIN_API_KEY=
LANGCHAIN_TRACING_V2=
LANGCHAIN_PROJECT=Multi-
```
