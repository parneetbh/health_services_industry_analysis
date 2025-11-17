# 🌐 Health Services Industry Analysis  
### Financial Analytics and NLP Applied to US Public Firms

This project combines financial analysis and text based methods to study the US Health Services industry. It integrates structured financial datasets with unstructured 10-K filing text to uncover sector patterns, map firm similarity, and evaluate the competitive position of Amedisys Inc through a mix of quantitative and narrative based insights.

---

## 📌 Objectives

- Analyze long term financial trends in the Health Services sector  
- Clean and process Item 1 text from 10-K filings  
- Extract and visualize sector keywords using frequency and TF-IDF  
- Train embeddings to explore semantic relationships in filings  
- Identify similar firms based on narrative content  
- Assess Amedisys Inc using revenue, ROA, and market share trends  

---

## 📊 Datasets Used

- **public_firms.csv** – financial and accounting data  
- **major_groups.csv** – SIC major group mappings  
- **2020_10K_item1_full.csv** – Item 1 text from 2020 10-K filings  

**Note:**  
The full datasets used for this analysis are not included in this repository due to GitHub file size limits.  
A small sample file (`2020_10K_item1_sample.csv`) is provided to illustrate the text processing workflow.  
The complete analysis was performed locally using the full files.

---

## 📈 1. Industry Level Exploration

The Health Services sector was identified using SIC major group codes.  
Key insights include:

- Leading firms by stock price and total sales  
- Geographic distribution of company headquarters  
- Average stock price trends  
- Sensitivity to the 2008 financial crisis  
- Long term ROA patterns for US based firms  

These results provide a financial overview of the sector.

---

## ✍️ 2. Text Processing and Keyword Insights

Item 1 text was cleaned using standard NLP steps:

- Lowercasing  
- Punctuation removal  
- Stopword filtering via NLTK  

Keyword analysis included:

- Frequency based ranking  
- TF-IDF scoring  
- Wordcloud visualizations  

This highlights common patterns in how Health Services firms describe their operations and risks.

---

## 🤖 3. Embeddings and Similarity Patterns

Embeddings were trained on the cleaned Item 1 text to capture semantic patterns.

### Applications:

- Finding words related to selected sector concepts  
- Embedding each firm’s keyword set  
- Creating aggregated firm level vectors  
- Identifying similarity between firms based on narrative content  

This bridges qualitative business text with quantitative modeling.

---

## 🏥 4. Focal Firm: Amedisys Inc

Amedisys was selected for deeper evaluation based on its strong stock performance in 2020.

### Competitor Identification  
Firms were compared using similarity in their embedded narrative representations to identify the closest competitors with complete financial data.

### Financial Benchmarking  
Amedisys was analyzed against these peers based on:

- Revenue growth  
- ROA performance  
- Market share trends  

The company demonstrates steady growth, strong operational efficiency, and increasing competitive presence.  
Full results and visualizations are available in the notebook.

---

## 🛠 Tools and Libraries

- Python  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- nltk  
