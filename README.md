# 🏠 HomeMatch: AI-Powered Real Estate Assistant

HomeMatch is an AI-driven application that transforms the real estate search experience. Instead of scrolling through endless listings, users can chat with a conversational agent that learns their preferences and recommends properties tailored specifically to them.  

🔗 **Built for:** *Future Homes Realty*  
📌 **Use Case:** Personalized property discovery powered by Generative AI  

---

## ✨ Features

- **Conversational Search** – Find homes through natural dialogue rather than filters.  
- **Personalized Recommendations** – Matches listings to your unique preferences (e.g., size, amenities, neighborhood style).  
- **Contextual Memory** – Stores user responses in a vector database for tailored, evolving recommendations.  
- **Dynamic Listing Descriptions** – Uses an LLM to generate persuasive, human-like property write-ups.  

---

## 🛠️ Tech Stack

- **Language Models:** OpenAI GPT-3.5 via `langchain-openai`  
- **Framework:** [LangChain](https://www.langchain.com/)  
- **Vector Database:** [ChromaDB](https://www.trychroma.com/) with `OpenAIEmbeddings`  
- **Data Processing:** `pandas` for CSV ingestion & formatting  
- **Environment:** Jupyter Notebook (`HomeMatch.ipynb`)

---

## 📂 Repository Structure

```
HomeMatch/
│── HomeMatch.ipynb       # Main notebook with full pipeline
│── listings.csv          # Sample real estate dataset
│── requirements.txt      # Dependencies
│── README.md             # Project documentation
```

---

## ⚙️ How It Works

1. **Data Ingestion**  
   - Listings from `listings.csv` are preprocessed into rich text features.  

2. **Vectorization**  
   - Listings + user answers are embedded into numerical vectors.  
   - Stored in a Chroma vector database.  

3. **Conversational Interface**  
   - Users answer guided questions (size, amenities, location style, etc.).  
   - Preferences are saved into the vector DB.  

4. **Recommendation Engine**  
   - The system retrieves the most relevant listings.  
   - The LLM generates unique, human-friendly property descriptions personalized to the user.  

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/HomeMatch.git
cd HomeMatch
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Set your API keys
Add your OpenAI key:
```bash
export OPENAI_API_KEY="your_api_key"
```

### 4. Run the notebook
```bash
jupyter notebook HomeMatch.ipynb
```

---

## 📊 Example Interaction

**User:** *“I want a suburban home, around 1200 sqft, with a backyard and pool, close to schools.”*  
**HomeMatch:**  
*“I’ve found a home in Suburban Sanctuary for $600,000. It has 4 bedrooms, 3 bathrooms, and a safe family-friendly neighborhood with nearby top-rated schools. The backyard includes space for gatherings and the area is known for its strong community watch.”*

---

## ✅ Future Improvements

- Integrate **real-time MLS feeds** for live data.  
- Deploy a **web UI** with Streamlit or React.  
- Add **multi-modal search** (images + text).  
- Extend to **rental listings** and **mortgage calculators**.  

---
