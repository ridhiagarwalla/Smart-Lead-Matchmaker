# Smart-Lead-Matchmaker
An AI-based Smart Lead Matchmaker for Entrepreneurs &amp; Investors, with gamified onboarding and personalized partner suggestions.
# 🚀 SmartLead: AI-Powered Lead Matchmaker for Startups & Investors

**SmartLead** is a gamified, AI-powered web tool designed to help **entrepreneurs, investors, and operators** discover high-quality business leads. Built a rapid prototyping challenge, it combines user-friendly onboarding, smart matchmaking, and insightful visualizations — all accessible via a simple Streamlit interface.

---

## 🌟 Summary

**“An AI-based Smart Lead Matchmaker for Entrepreneurs & Investors, with gamified onboarding and personalized partner suggestions.”**

---

## 🧠 Key Features

### 1. 🎲 Gamified Onboarding 
Collects and scores user data through an interactive form:

| Question                 | Type         | Options                                                                 |
|--------------------------|--------------|-------------------------------------------------------------------------|
| What’s your role?        | Dropdown     | Founder, Investor, Sales Lead, Operator                                |
| Business model?          | Dropdown     | B2B SaaS, E-commerce, Agency, Platform                                 |
| What are you looking for?| Multi-select | Clients, Investors, Resellers, Co-founders                             |
| Location preference?     | Dropdown     | Global, Local, Region-specific                                         |
| Stage / Revenue?         | Dropdown     | Pre-seed, Seed, Series A+, Profitable                                  |

> ✅ Users earn points for profile completeness and unlock rewards like **free premium leads**, increasing engagement.

---

### 2. 🤖 AI-Based Lead Matching 

Leverages **TF-IDF vectorization + cosine similarity** to match user profile with a curated dataset of companies.

**Matching logic includes:**
- Keyword-based text similarity
- Location and stage filters
- Smart scoring from 0–1

> ✅ Returns Top 5 Matches with similarity scores and tags like:
> - ✅ Industry Fit
> - ✅ Local Match
> - ⚠️ Early Stage

---

### 3. 📊 Visualization Dashboard

Visual comparison between **user profile** and **top lead matches** using:

- Horizontal bar graph for similarity scores
- Optional: Radar chart, Heatmap, Map view (future scope)

> ✅ Clean and readable charts built using **Matplotlib**.

---
![image](https://github.com/user-attachments/assets/28dbaaca-e14c-4368-b427-453359af5023)

## 🛠️ Tech Stack

| Tool           | Purpose                     |
|----------------|-----------------------------|
| **Python**     | Core logic and data matching|
| **Streamlit**  | UI for onboarding and demo  |
| **Scikit-learn**| TF-IDF and similarity calc |
| **Matplotlib** | Score and fit visualizations|
| **Pyngrok**    | Tunneling for public access (Colab) |

---

## 🚀 How to Run (in Google Colab)

1. Upload the repo or copy `app.py` code.
2. Install dependencies:
    ```bash
    !pip install streamlit pyngrok scikit-learn matplotlib
    ```
3. Start the app:
    ```python
    from pyngrok import ngrok
    import os
    os.system("streamlit run app.py &")
    public_url = ngrok.connect(8501)
    print("🔗 App URL:", public_url)
    ```
---

## 🎯 Future Enhancements

- Add database integration (Firebase/PostgreSQL)
- Build a multi-user backend for saving profiles
- Enable messaging between matched leads
- Advanced NLP (BERT/Embeddings)
- Expand dataset with real startup data

---
## 🙌 Team

**Built by:** Ridhi Agarwalla  
**Role:** Idea Lead, Backend Developer, UX Strategist

---
![image](https://github.com/user-attachments/assets/800eb7b4-130f-4053-9273-39876c31ad09)



