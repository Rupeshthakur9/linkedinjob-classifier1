# linkedinjob-classifier

This project uses web scraping, natural language processing (NLP), and machine learning models to classify LinkedIn job descriptions into categories like **Data Scientist**, **Data Engineer**, and **Data Analyst**.

## Features
- Data collection (generic scraper + CSV dataset)
- Data preprocessing and cleaning
- Baseline ML pipeline (TF-IDF + Logistic Regression)
- Transformer-based pipeline (DistilBERT fine-tuning)
- REST API with FastAPI for predictions

## Folder structure
```
linkedinjob-classifier/
├── data/                  # Sample datasets (CSV, Excel)
├── models/                # Saved trained models
├── notebooks/             # Jupyter notebooks for exploration
├── src/                   # Source code (training, preprocessing, API)
├── README.md              # Project documentation
└── requirements.txt       # Python dependencies
```

## Usage
1. Install dependencies: `pip install -r requirements.txt`
2. Train baseline model: `python src/train.py`
3. Run API: `uvicorn src.app:app --reload --port 8000`
