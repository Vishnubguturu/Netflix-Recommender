# Netflix Content-Based Recommender

A content-based recommendation system that suggests Netflix movies and TV shows 
similar to a given title using TF-IDF vectorization and cosine similarity.

## Models Implemented
- **TF-IDF + Cosine Similarity** — primary model using text metadata
- **CountVectorizer + Cosine Similarity** — bag-of-words baseline
- **KNN on TF-IDF matrix** — nearest neighbor approach
- **Popularity-based** — recommends most frequent titles (baseline)
- **Random recommender** — trivial baseline

## Evaluation Metrics
- Precision@k
- Mean Average Precision (MAP)
- Coverage

## Key Findings
- TF-IDF cosine similarity produces semantically coherent recommendations
- Content-based filtering works well for cold-start scenarios (no user history)
- Model mirrors Netflix's "Similar to..." recommendation carousels

## Tech Stack
Python, pandas, numpy, scikit-learn, seaborn, matplotlib, nltk, wordcloud

## Dataset
Two Kaggle Netflix datasets (movies + TV shows) merged into a single DataFrame

## How to Run
1. Download the Netflix datasets from Kaggle
2. Place `netflix_movies.csv` and `netflix_tv_shows.csv` in `/content/`
3. Open `netflix_recommender.ipynb` in Google Colab or Jupyter Notebook
4. Run all cells in order