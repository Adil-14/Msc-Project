# Sportswashing-Sentiment-NLP

This repository contains the code, datasets, and notebooks for my MSc thesis project:

**Analysing and Predicting Sentiment Around Sportswashing Narratives: A Comparative Study of Gulf Investments in Global Sports Using NLP**

The project uses YouTube comments and transcripts to study how people discuss sportswashing. It applies preprocessing, LLM-assisted annotations (OpenAI + Azure Bing Grounding), and predictive models (including DistilBERT) to analyse sentiment, claims, temporal trends, and network structures.

---

## Repository structure

├── Claim_Detection_BingGrounding/ # claim detection and verification with Bing grounding
├── Datasets/ # cleaned and final datasets
├── DistilBERT_Prediction/ # transformer-based sentiment prediction
├── Network_Analysis_Gephi/ # exports for Gephi network analysis
├── OpenAI_Submissions/ # OpenAI batch prompts and classification scripts
├── Sentiment/ # classical ML sentiment baselines
├── Temporal_Tagging/ # temporal trend analysis
├── Youtube_Data_Scraper/ # YouTube comment and transcript collection


---

## Packages Used
pandas
numpy
scikit-learn
matplotlib
tqdm
requests
transformers
torch

## API Keys
YOUTUBE_API_KEY=...
OPENAI_API_KEY=...
AZURE_OPENAI_ENDPOINT=...
AZURE_OPENAI_KEY=...
BING_SEARCH_KEY=...

## Workflow

### Scraping
- Collect YouTube comments and transcripts using notebooks in **`Youtube_Data_Scraper/`**.

### Preprocessing
- Clean and merge into **`Datasets/All_YouTube_Comments.csv`**  
  → final processed dataset in **`Datasets/Final_Merged_Results_Processed.csv`**.

### Annotation
- Sentiment, claim detection, factuality, etc. via **`OpenAI_Submissions/`**  
  and **`Claim_Detection_BingGrounding/`**.

### Modelling
- Classical baselines in **`Sentiment/`**.  
- DistilBERT implementation in **`DistilBERT_Prediction/`**.

### Temporal + Network
- **`Temporal_Tagging/`** for time-aware analysis.  
- **`Network_Analysis_Gephi/`** for network structure and community detection.

## Results

- **Sentiment prediction**: Achieved strong baseline and transformer performance.  
- **Claim detection**: Implemented hybrid LLM + Bing pipeline for fact verification.  
- **Temporal + network insights**: Identified peaks in discussion and influential nodes.  

*(Full results and discussion available in the MSc thesis document.)*
