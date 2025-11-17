# 🌐 Health Services Industry Analysis  
### Financial Analytics, NLP, and Word Embeddings Applied to US Public Firms

This project combines financial analysis, keyword extraction, and modern NLP techniques to study the US Health Services industry. It integrates structured financial datasets with unstructured 10-K filing text to uncover sector patterns, map firm similarity, and evaluate the competitive position of Amedisys Inc through a mix of quantitative and text based methods.

---

## 📌 Objectives

- Analyze long term financial trends in the Health Services sector  
- Clean and process Item 1 text from 10-K filings  
- Extract and visualize sector keywords using frequency and TF-IDF  
- Train a Word2Vec model to explore semantic relationships in filings  
- Build firm level embeddings and identify similar competitors  
- Assess Amedisys Inc using revenue, ROA, and market share trends  

---

## 📊 Datasets Used

- **public_firms.csv** – financial and accounting data  
- **major_groups.csv** – SIC major group mappings  
- **2020_10K_item1_full.csv** – Item 1 text from 10-K filings  

All datasets are included in the data folder.

---

## 📈 1. Industry Level Exploration

The Health Services sector was isolated using SIC major group codes.  
Key insights include:

- Leading firms by stock price and total sales  
- Geographic distribution of company headquarters  
- Average stock price trends across time  
- Identification of firms most impacted during 2008  
- Long term ROA patterns for US based firms  

These findings establish the financial landscape of the industry.

---

## ✍️ 2. Text Processing and Keyword Insights

Item 1 text was cleaned using:

- Lowercasing  
- Punctuation removal  
- Stopword filtering via NLTK  

Keyword analysis included:

- Frequency based ranking  
- TF-IDF scoring  
- Wordcloud visualizations highlighting sector vocabulary  

This revealed common themes in how Health Services firms describe operations and risk.

---

## 🤖 3. Word Embeddings and Semantic Patterns

A Word2Vec model was trained on all cleaned Item 1 text.

### Model applications:

- Identifying the closest words to sector representative keywords  
- Converting firm keywords into embeddings  
- Aggregating those embeddings to create firm level vectors  
- Computing similarity between firms based on narrative content  

This bridges qualitative business text with quantitative modeling.

---

## 🏥 4. Focal Firm: Amedisys Inc

Amedisys was selected due to its strong 2020 stock performance.

### Competitor Identification  
Firm level embeddings were compared using cosine similarity to find closest competitors with available financial data.

### Financial Benchmarking  
Amedisys was analyzed against its peers for:

- Revenue growth  
- ROA strength  
- Market share trends  

The firm demonstrates steady growth, high operational efficiency, and increasing competitive presence.

Detailed results and visualizations are available in the notebook.

---

## 🛠 Tools and Libraries

- Python  
- pandas  
- numpy  
- matplotlib  
- wordcloud 
- nltk  
- gensim (Word2Vec)  
