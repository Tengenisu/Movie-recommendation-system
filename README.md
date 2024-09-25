# Movie Recommendation System

This project is a movie recommendation system that uses cosine similarity to suggest movies based on user preferences. The system processes movie data and compares it using cosine similarity to provide recommendations based on text-based features such as movie descriptions or genres.

## Features
- Recommends movies based on the similarity of movie features (e.g., genres, descriptions).
- Uses cosine similarity to compute the closeness of movies to each other.
- Handles user input with fuzzy matching to improve recommendation accuracy, even with slight errors.

## Tech Stack
- **Python**: Core programming language used for building the system.
- **pandas**: For data handling and manipulation.
- **numpy**: For numerical operations.
- **scikit-learn**: For implementing cosine similarity and text vectorization.
- **rapidfuzz**: For input matching and handling minor user errors.

## How it Works
1. **Data Handling**: The movie dataset is loaded and processed using pandas.
2. **Text Vectorization**: Movie features (such as genres or descriptions) are converted into numerical form using `CountVectorizer` from scikit-learn.
3. **Cosine Similarity**: The similarity between movies is calculated using `cosine_similarity` to find the closest matches to a given movie.
4. **Fuzzy Matching**: User inputs are handled using `rapidfuzz.process` to allow for slight errors in movie names.

## Installation
Clone the repository:

```bash
git clone https://github.com/yourusername/movie-recommendation-system.git
cd movie-recommendation-system
```

```bash 
python3 -m venv venv
source venv/bin/activate  # For Mac/Linux
venv\Scripts\activate     # For Windows
```

```bash 
python3 -m pip install -r ./setup.txt
```
