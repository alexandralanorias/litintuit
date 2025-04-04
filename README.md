# **Litintuit**  
An intelligent book recommendation system powered by **DistilRoBERTa and vector embeddings**.
![litintuit dashboard](https://github.com/alexandralanorias/litintuit/blob/master/litintuit-dashboard.png)

## **Overview**  
**Litintuit** is a **semantic book recommender** that provides **genre- and emotion-based** book suggestions. Unlike traditional recommendation systems that rely on collaborative or content-based filtering, LitIntuit uses a **pure LLM-driven approach** to understand the emotional tone and themes of books, allowing for more intuitive and nuanced recommendations.

## **Key Features**  
- **LLM-Powered Understanding** – Uses **DistilRoBERTa** to analyze books and user queries at a semantic level.  
- **Free-Text Query Support** – Users can describe their reading preferences naturally (e.g., *"I want a hopeful and introspective coming-of-age novel"*).  
- **Emotion & Tone Matching** – Beyond genre, LitIntuit recommends books based on their **mood**.  
- **Vector Search for Similarity** – Utilizes **embeddings** to find books that closely align with user preferences.  
- **Simple CSV-Based Metadata Storage** – No external APIs or databases—just efficient local data handling.  

## **How It Works**  
1. **User Input:** The user enters a free-text query describing their ideal book.  
2. **Text Embedding & Vector Search:** The system converts both the user query and book metadata into vector representations.  
3. **LLM-Powered Matching:** Using **DistilRoBERTa**, the system identifies books with similar themes, tones, and genres.  
4. **Recommendation Output:** The results are displayed in a **ranked gallery grid**, with up to **16 recommendations** per query.  

## **Technology Stack**  
- **Natural Language Model:** [Hartmann's Emotion English DistilRoBERTa-base](https://huggingface.co/j-hartmann/emotion-english-distilroberta-base) for semantic text analysis.  
- **Vector Embeddings:** Used to represent book data and user queries in a similarity-based retrieval system.  
- **Data Storage:** **CSV files** for storing book metadata, ensuring lightweight and flexible data handling.  
- **Frontend & Backend:** Built as a **web application** for a user-friendly experience using Python and Gradio.  

## **Getting Started**  
To run Litintuit locally:  
- Clone this repo.
- Run `python gradio-dashboard.py` in your terminal.
- The server will take some time to load due to data chunking. Wait for approximately 3 minutes.
- After some time, the server will display the local url where it is hosted. Open the web app in your browser and start discovering books! 📚  