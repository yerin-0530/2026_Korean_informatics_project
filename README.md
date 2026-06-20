# A Corpus-Based Comparative Study on the Usage of “Controversy”, “Issue”, and “Topic of Interest” in Korean News Discourse (2018–2025)

## Project Overview
This project analyzes how three key expressions in Korean news discourse—“controversy” (논란), “issue” (이슈), and “topic of interest” (화제)—are used in social news articles published between 2018 and 2025.

Using a large-scale news corpus, this study applies computational linguistics methods to examine differences in frequency, collocational behavior, sentiment distribution, and discourse framing. The goal is to understand how lexical choices in media contribute to the construction and framing of social reality.

---

## Research Objectives
This study aims to:

- Compare the frequency trends of the three expressions across time (2018–2025)
- Identify and compare their collocational (co-occurrence) patterns
- Analyze evaluative and emotional characteristics using sentiment analysis
- Examine discourse framing structures and boundary relations among the three expressions
- Investigate how media language shapes social interpretation of events

---

## Data Description
- **Time span:** 2018–2025  
- **Data source:** BigKinds Korean News Corpus  
- **Media outlets:** 12 major national newspapers in South Korea  
- **Target expressions:** 논란 (controversy), 이슈 (issue), 화제 (topic of interest)  
- **Unit of analysis:** Sentence-level extraction of news articles containing target keywords  

---

## Methodology

### 1. Frequency Analysis
Annual frequency counts of each keyword were computed to examine temporal trends.  
Visualization was performed using Pandas, Matplotlib, and Seaborn.

---

### 2. Collocation Analysis
Morphological analysis was conducted using **KoNLPy (Okt)**.

- Extraction window: ±3 tokens around each keyword  
- Separation of:
  - Noun collocations  
  - Predicate (verb/adjective) collocations  
- Visualization: word clouds and frequency plots  

---

### 3. Sentiment Analysis
Sentiment classification was performed using:

- **KR-FinBERT-SC (HuggingFace Transformers)**  

Each sentence was classified into:
- Positive
- Neutral
- Negative

Probability scores were also used for comparative analysis.

---

### 4. Discourse Framing & Boundary Analysis
To examine semantic and structural differences between the three expressions:

- Jaccard similarity → collocation overlap  
- Cosine similarity → sentiment distribution similarity  
- Jensen–Shannon Divergence (JSD) → distributional distance  
- Year-by-year comparison of framing shifts
  
---

## Tools & Libraries
- Python 3.x  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- KoNLPy (Okt morphological analyzer)  
- WordCloud  
- HuggingFace Transformers  
- PyTorch  

---

## Key Findings

### 1. Semantic Roles
- **Controversy:** strongly associated with conflict, verification, and escalation narratives  
- **Issue:** functions as an agenda-setting and structural discourse category  
- **Topic of interest:** associated with media attention and narrative-driven content  

---

### 2. Structural Patterns
- Strong overlap in noun collocations across all three expressions  
- Clear divergence in predicate (verb/adjective) usage patterns  
- “Issue” functions as a mediating category between the other two expressions  
- “Topic of interest” shows the most independent discourse structure  

---

### 3. Sentiment Patterns
- “Issue” and “Topic of interest” show highly similar sentiment distributions  
- “Controversy” shows a more neutral-than-expected distribution  
- Sentiment is primarily determined by context rather than lexical meaning alone  

---

## Limitations
- Some news URLs were inaccessible, resulting in missing data  
- Corpus contains noise and duplicate records due to web extraction  
- Sentiment model may not fully capture journalistic domain-specific semantics  

---

## Data Source
- BigKinds News Corpus: https://www.bigkinds.or.kr/

---

## AI Assistance
This project was supported by AI tools:

- Google Gemini 2.5 Flash: Python code generation, debugging, preprocessing support  
- ChatGPT (OpenAI): research design feedback, linguistic interpretation, code refinement, and writing assistance  

All final interpretations and conclusions are the responsibility of the author.

---

## Repository
https://github.com/yerin-0530/2026_Korean_informatics_project
