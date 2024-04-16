# Movie-Recommendation-System

### Importing Dependencies:
It imports necessary libraries like NumPy, Pandas, difflib, and scikit-learn's TfidfVectorizer and cosine_similarity functions.

### Data Collection and Pre-Processing:
- It loads movie data from a CSV file into a Pandas DataFrame.
- Selects relevant features like genres, keywords, tagline, cast, and director.
- Replaces any null values in these selected features with empty strings.
- Combines all selected features into a single string for each movie.
- Converts the combined text data into feature vectors using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization.

### Cosine Similarity:
- Calculates the similarity scores between movies using cosine similarity based on the feature vectors.

### Getting the Movie Name from the User:
- Asks the user to enter their favorite movie name.
- Creates a list of all movie titles in the dataset.
- Finds the closest match for the movie name entered by the user using difflib's get_close_matches function.

### Finding Similar Movies:
- Retrieves the index of the closest matched movie.
- Calculates similarity scores between the selected movie and all other movies.
- Sorts the movies based on their similarity scores in descending order.
- Prints the top similar movies as recommendations.

### Movie Recommendation System Prompt:
- It prompts the user again to enter their favorite movie name and repeats the recommendation process.
