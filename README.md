Automated News Mining & Monitoring Pipeline

# 🗳️ Global Media Framing of the Trump Assassination Attempt: Sentiment and Topic Analysis

### 📋 Project Overview
This project analyzes the global media reaction to the assassination attempt on Donald Trump (July 2024).
Using **Natural Language Processing (NLP)** techniques, I processed over **3,700 news articles** collected via NewsAPI and GDELT to understand how the narrative evolved in the immediate aftermath, identifying key themes and sentiment polarization across different media outlets.

The goal was to move beyond simple frequency analysis and uncover the **underlying emotional tone** and **thematic structures** of the news coverage using Deep Learning (BERT) and Probabilistic Modeling (LDA).

### 🚀 Key Findings
* **Collected 3.7K multilingual news articles**.
* **Sentiment Shift:** Analysis identified a distinct temporal shift from initial "Shock/Fear" to "Political Analysis/Blame" within 48 hours.
* **Topic Polarization:** LDA modeling revealed clear clusters around *Security Failure*, *Political Rally dynamics*, and *International Reactions*.
* **Model Performance:** Sentiment was classified using **BERT (Transformers)**, achieving superior contextual granularity compared to lexicon-based approaches.

---

### 🧠 Methodology

#### 1. Data Collection & Preprocessing
* **Source:** NewsAPI and GDELT.
* **Cleaning:** Removed duplicates, handled missing values, and performed advanced text normalization (Lemmatization, Stop-words removal using NLTK and Spacy).

#### 2. Sentiment Analysis (BERT) 🤖
* Leveraged **Hugging Face Transformers** to implement a pre-trained **BERT** model for sequence classification.
* The BERT model captures contextual nuances (e.g., sarcasm, double negatives) essential for political text analysis.
* **Output:** Classified articles into *Positive*, *Negative*, and *Neutral* sentiment categories.

#### 3. Topic Modelling (LDA) 📊
* Applied **Latent Dirichlet Allocation (LDA)** using `Gensim` to discover abstract topics within the corpus.
* Optimized the number of topics ($k$) based on Coherence Score ($C_v$).

---

### 🛠️ Tech Stack
* **Language:** Python
* **NLP & ML:** HuggingFace Transformers (BERT), Gensim (LDA), NLTK, Scikit-learn
* **Data Handling:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn, WordCloud

---

### 📂 Repository Structure
* `notebook/`: Contains the Jupyter Notebook with the full analysis pipeline.
* `report/`: Detailed PDF report explaining the theoretical background and business insights.
* `data/`: Raw and processed datasets (CSV).

---
*Author: Lorenzo D'Amico*
