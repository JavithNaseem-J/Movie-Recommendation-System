
# Movie Recommendation System

This project implements a **content-based movie recommendation system** using Python. It leverages movie metadata such as genres, keywords, cast, crew, and overviews from the TMDB 5000 Movies dataset to recommend similar movies based on cosine similarity. The system processes the data, transforms it into a suitable format, and uses natural language processing (NLP) techniques and machine learning to generate recommendations.


## Overview
The recommendation system takes a movie title as input and suggests five similar movies based on their content similarity. It uses the following steps:
1. Data preprocessing (merging datasets, cleaning, and feature extraction).
2. Text processing (stemming, removing spaces, and vectorization).
3. Cosine similarity computation to find similar movies.

This project is ideal for learning about content-based filtering, NLP, and basic machine learning techniques.

## Features
- Recommends movies based on content similarity (genres, keywords, cast, crew, and overview).
- Uses NLTK for text stemming to normalize words.
- Employs `CountVectorizer` for feature extraction and `cosine_similarity` for similarity computation.
- Exports the processed data and similarity matrix as pickle files for easy deployment.

## Dataset
The system uses two datasets from TMDB:
- `tmdb_5000_credits.csv`: Contains movie credits (cast and crew).
- `tmdb_5000_movies.csv`: Contains movie metadata (genres, keywords, overview, etc.).


## Requirements
- Python 3.x
- Libraries:
  - `pandas`
  - `numpy`
  - `matplotlib` 
  - `seaborn`
  - `nltk`
  - `scikit-learn`
  - `pickle`

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-system.git
   cd movie-recommendation-system
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the datasets (`tmdb_5000_credits.csv` and `tmdb_5000_movies.csv`) and place them in a `data_folder` directory within the project root. You can find these datasets on [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata).

4. Run the Jupyter notebook (`movie_recommendation.ipynb`) to preprocess the data and generate the recommendation model.


   # Example usage
   
   recommend("The Dark Knights Rises")

  **Output:**
   
   The Dark Knights Rises
   Batman
   Batman Begins
   Batman Returns


## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.



![image](https://github.com/user-attachments/assets/b9c15cb9-0d54-4399-9aaa-3d3e1c662bf7)
