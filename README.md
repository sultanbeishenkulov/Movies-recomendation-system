# Movie Recommendation System

This project implements a simple movie recommendation system using collaborative filtering. The system suggests movies based on user ratings and similarities between users' preferences.

## Dataset
The project utilizes two datasets:
- **Movies Data:** Loaded from the "movies.csv" file, containing information about movies, including movieId, title, and genres.
- **Ratings Data:** Loaded from the "ratings.csv" file, consisting of user ratings for various movies, including userId, movieId, rating, and timestamp.

## Cleaning and Preprocessing
1. **Clean Title:** A function `clean_title` is applied to remove special characters from movie titles, creating a new column named "clean_title."

## Movie Similarity Calculation
1. **TF-IDF Vectorization:** Titles are transformed into TF-IDF vectors using the TfidfVectorizer from scikit-learn.
2. **Cosine Similarity:** Cosine similarity is calculated between the TF-IDF vectors to measure the similarity between movies.

## Movie Search Functionality
- A search function allows users to input a movie title, and the system returns the top 5 similar movies.

## Collaborative Filtering
- For a given movie, the system identifies users who gave high ratings to that movie.
- It then recommends other movies highly rated by those users, weighted by the frequency of ratings.

## Usage
1. Input a movie title using the provided widget.
2. The system will display the top 5 similar movies based on the movie title.
3. Additionally, it provides collaborative filtering recommendations based on user ratings.

## Technologies Used
- **Languages:** Python, SQL
- **Libraries:** Pandas, NumPy, scikit-learn
- **Tools:** Jupyter Notebook, ipywidgets

## How to Run
1. Clone the repository.
2. Ensure you have the required libraries installed (Pandas, NumPy, scikit-learn).
3. Run the Jupyter Notebook.
