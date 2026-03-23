import streamlit as st
import ollama
import requests
from bs4 import BeautifulSoup
import json

# Web search function (your original, improved)
@st.cache_data(ttl=3600)  # Cache for 1 hour
def fetch_web_text(query):
    url = f"https://www.google.com/search?q={query}"
    headers = {"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36"}
    try:
        r = requests.get(url, headers=headers)
        soup = BeautifulSoup(r.text, "html.parser")
        texts = [g.get_text().strip() for g in soup.select("div") if len(g.get_text()) > 100]
        return " ".join(texts[:3])  # Top 3 snippets
    except:
        return "No web data available."

# Initialize session state for memory (chat history)
if "messages" not in st.session_state:
    st.session_state.messages = []

# UI: ChatGPT-like interface
st.title("🔥 Local ChatGPT Clone with Memory & Web Search")
st.caption("Powered by LLaMA (Ollama). Remembers conversations. Type 'exit' or clear chat to reset.")

# Display chat history
for message in st.session_state.messages:
    with st.chat_message(message["role"]):
        st.markdown(message["content"])

# Chat input
if prompt := st.chat_input("Ask anything..."):
    # Add user message
    st.session_state.messages.append({"role": "user", "content": prompt})
    with st.chat_message("user"):
        st.markdown(prompt)

    # Fetch web data
    with st.chat_message("assistant"):
        web_data = fetch_web_text(prompt)
        if web_data:
            st.info("🔍 Web context fetched.")
        
        # Streaming response with memory
        message_placeholder = st.empty()
        full_response = ""

        # Build messages with history (memory)
        messages = [{"role": "system", "content": "You are a helpful AI assistant. Use web context if relevant. Be concise and engaging."}]
        messages.extend(st.session_state.messages)

        # Add web context to last user message
        if web_data:
            messages[-1]["content"] += f"\n\nWeb context: {web_data[:2000]}..."  # Truncate for tokens

        stream = ollama.chat(
            model="llama3.2:latest",  # Or "llama3.1:8b" for better quality
            messages=messages,
            stream=True,
            options={"temperature": 0.7, "num_predict": 500}
        )

        for chunk in stream:
            if "message" in chunk and "content" in chunk["message"]:
                content = chunk["message"]["content"]
                full_response += content
                message_placeholder.markdown(full_response + "▌")
        
        message_placeholder.markdown(full_response)

    # Add assistant response to memory
    st.session_state.messages.append({"role": "assistant", "content": full_response})

    # Keep only last 20 messages for memory efficiency
    if len(st.session_state.messages) > 40:  # 20 exchanges
        st.session_state.messages = st.session_state.messages[-40:]

# Sidebar: Controls
with st.sidebar:
    st.header("Memory & Controls")
    if st.button("🗑️ Clear Memory"):
        st.session_state.messages = []
        st.rerun()
    st.info(f"Memory size: {len(st.session_state.messages)//2} exchanges")
