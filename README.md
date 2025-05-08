# 🔎 LangChain - Chat with Search

This is a Streamlit application that integrates with LangChain and the Groq API to create a conversational chatbot capable of searching the web, Wikipedia, and Arxiv for accurate and up-to-date information. It uses the `ZERO_SHOT_REACT_DESCRIPTION` agent type and streams responses directly into the UI.

## 🚀 Features

- 🔍 Integrates **DuckDuckGo**, **Wikipedia**, and **Arxiv** search tools
- 🧠 Uses **LangChain Agents** to interpret queries and decide which tool to use
- 💬 Interactive chat interface using **Streamlit**
- ⚡ Fast inference with **Groq's LLaMA 3 (8B, 8192)** model
- 🧵 Streams intermediate thoughts and reasoning via `StreamlitCallbackHandler`

## 📦 Dependencies

Make sure to install the following Python packages:

pip install streamlit langchain langchain-groq langchain-community

## 🛠️ Setup
1. Clone the repository:
git clone https://github.com/rizwanchanna/Langchain-Search-Engine
cd langchain-search-agent

2. Install dependencies:
pip install -r requirements.txt

3. Run the app:
streamlit run app.py

4. Enter your Groq API key in the sidebar.

## 🧠 How It Works
The agent uses LangChain's initialize_agent with the ZERO_SHOT_REACT_DESCRIPTION type to intelligently select between the available tools (Arxiv, Wikipedia, DuckDuckGo) based on your query. The responses are streamed into a conversational interface using Streamlit.

## ✅ Example Query
What is machine learning?
The agent will analyze the question and may decide to use Wikipedia for a quick definition, Arxiv for scholarly sources, or DuckDuckGo for broader results.

## 🔐 Note on API Keys
This app uses your personal Groq API key. Keep it secure and do not share it publicly.
