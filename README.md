
# Movie Recommendation System 🎬

A content-based movie recommendation system that suggests similar movies
based on your favorite movie using cosine similarity.

## How It Works
1. User inputs a favorite movie name
2. Fuzzy matching finds the closest title in the dataset (handles typos)
3. Selected features are combined into a single text representation
4. TF-IDF vectorization converts text to numerical data
5. Cosine similarity compares movies to find the most similar ones
6. Returns top 30 recommendations

## Technique
- **Content-Based Filtering** using cosine similarity
- **TF-IDF Vectorization** to convert text features to numbers
- **Fuzzy Matching** via difflib to handle inexact movie title inputs

## Features Used for Similarity
| Feature | Description |
|---------|-------------|
| `genres` | Movie genre (Action, Comedy, Drama etc.) |
| `keywords` | Plot keywords |
| `tagline` | Movie tagline |
| `cast` | Lead actors |
| `director` | Director name |

## Libraries
- pandas, numpy, scikit-learn, difflib

## Dataset
[movies.csv]([./movies.csv](https://drive.google.com/file/d/1cCkwiVv4mgfl20ntgY3n4yApcWqqZQe6/view))

## Example
```
Enter your favorite movie name: The Dark Knight
Movies suggested for you:

1. Batman Begins
2. The Dark Knight Rises
3. Iron Man
...
```

## Files
| File | Description |
|------|-------------|
| `movie_recommendation.ipynb` | Main notebook |
| `movies.csv` | Movies dataset |
