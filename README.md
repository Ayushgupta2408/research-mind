# Research Mind

demo-https://youtu.be/pNXYbkEf0UY

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
