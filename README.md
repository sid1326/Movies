# Movies
recommending great movies
Built on Streamlit providing personalized movie recommendations based on user interests. The system employs a content-based filtering algorithm suggesting movies with similar attributes to the ones the user has shown interest in.

# Features:
This model uses a content-based filtering algorithm.

# Content-Based Filtering:
Content-based systems use item attributes (such as movie genres, cast, director, etc.) to make recommendations.
Systems like Twitter and YouTube use similar algorithms to suggest content based on user preferences.
The system forms embeddings (vectors) based on features, such as the movies you watch or the music you listen to.
Recommendation Approach: It creates a vector of item features and compares them with the user’s preferences to recommend similar items.
Advantages: Personalized suggestions based on past user behavior.
Limitations: This may lead to excessive specialization (i.e., the system might only recommend items from the same categories, missing out on other potentially interesting items).
Data:
Data is sourced from the TMDb Movie Metadata Dataset.

# Model Overview:
The model uses Cosine Similarity to compare movies:
  1. Cosine Similarity is a metric that measures the similarity between two vectors.
  2. Vectors are generated from movie features using a NumPy array.
  3. The cosine_similarity() function calculates the similarity between two vectors, with values ranging from [0,1].
        0: Completely dissimilar.
        1: Completely similar.
