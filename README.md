# 🌦️ Smart Weather Assistant

An AI-powered assistant built with Hugging Face LLMs, LangChain, FAISS, and Open-Meteo API. It provides smart, real-time weather-based advice on what to wear or do based on your location and current conditions — all through a simple Gradio interface.

---

## ✨ Features

✅ Extracts locations from natural language queries  
✅ Fetches real-time weather (temperature, wind, conditions)  
✅ Embeds and searches a clothing & activity PDF guide using FAISS  
✅ Uses LLM to generate final recommendations  
✅ Gradio web interface for easy interaction  
✅ Built to run entirely in Google Colab or locally

---

## 🧠 How It Works

1. **LLM** extracts a location from your query (e.g., “What should I wear in Luxor?”)
2. **Open-Meteo API** provides real-time weather data for that location.
3. A **semantic search query** is generated based on the weather + question.
4. **FAISS vector DB** returns relevant PDF content (clothing, activities, safety tips).
5. **LLM** writes a smart final response based on all the above.
