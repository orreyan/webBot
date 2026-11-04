# webBot Streamlit and LangChain Experiments

An early exploration of building data and AI web apps in Python with **Streamlit**. The repository contains two small apps: an LLM-powered text assistant and an interactive geospatial data dashboard.

---

## Technology

| Area | Technology |
| --- | --- |
| Language | Python 3 |
| UI Framework | Streamlit |
| AI | LangChain with the OpenAI LLM API |
| Data | pandas, NumPy |

---

## Apps

### LLM Text Assistant (`src/streamlit_app.py`)
A form-based interface that sends a user's prompt to an OpenAI model through LangChain and shows the response. The user enters their API key securely in the sidebar (masked input), and the app validates it before sending any request.

### NYC Pickups Dashboard (`src/page1.py`)
An interactive dashboard built on a public dataset of New York City ride pickups:
- Loads and cleans the data with pandas, with results cached using `st.cache_data`
- Shows a histogram of pickups by hour of day
- Has an hour slider that filters the data
- Plots the filtered pickups on an interactive map

---

## Concepts Demonstrated

Rapid prototyping of web apps in Python, LLM integration through LangChain, safe handling of API keys, data loading and transformation with pandas, caching, and interactive data visualisation.

---

## Running Locally

```bash
pip install streamlit langchain openai pandas numpy
streamlit run websiteBot/src/streamlit_app.py   # LLM assistant
streamlit run websiteBot/src/page1.py           # Data dashboard
```

---

## Author

**Reyan Fethi**
