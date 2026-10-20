# Animated Series Sentiment Analysis — Streamlit Prototype

## Files

- `app.py` — Streamlit application
- `Sentiment Collection_Expanded(3).csv` — expanded project dataset
- `requirements.txt` — Python dependencies

## Run locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

The application trains the same final model used in the project notebook:
- 80/20 stratified train/test split
- Random oversampling on training data only
- Unigram TF-IDF
- Logistic Regression with `C=0.5`

The test set is not used by the Streamlit prediction interface.

## Deployment

Upload `app.py`, `Sentiment Collection_Expanded(3).csv`, and `requirements.txt`
to the hosting repository, then deploy `app.py` as the Streamlit entry point.
