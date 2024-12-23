🎥 Movie Recommendation System
This project implements a content-based movie recommendation system that suggests movies based on their similarities using a dataset of movies and their metadata. The application is built with Python and uses Streamlit for an interactive interface.

🛠️ Features
Content-Based Recommendations: Suggests movies based on their similarity to a given movie.
Streamlit UI: Provides a clean and simple interface to interact with the recommendation system.
Preprocessed Data: The system uses pickled data for quick computations.
📂 Project Structure
bash
Copy code
Movie-Recommendation-System/  
│  
├── tmdb_5000_credits.csv     # Original dataset containing movie credits  
├── tmdb_5000_movies.csv      # Original dataset containing movie metadata  
├── MovieRecSystem.py         # Core logic for creating and saving recommendation models  
├── app.py                    # Streamlit application  
├── movies.pkl                # Pickled preprocessed movie data  
├── similarity.pkl            # Pickled similarity matrix  
└── README.md                 # Project documentation  
🧑‍💻 How It Works
Dataset Preparation:

Data from tmdb_5000_credits.csv and tmdb_5000_movies.csv is preprocessed.
Relevant features (like genres, keywords, cast, crew) are extracted.
A similarity matrix is computed using cosine similarity.
Recommendation Logic:

When a user inputs a movie name, the system retrieves its index in the dataset.
The similarity matrix is used to find the most similar movies.
Web Application:

The app.py file creates a Streamlit-based interface for users to input their favorite movie.
The system displays recommended movies interactively.
🚀 Getting Started
Prerequisites
Python 3.7 or higher
Streamlit installed (use pip install streamlit)

🎯 Preprocessed Files
movies.pkl: Pickled file of preprocessed movie data for faster access.
similarity.pkl: Precomputed similarity matrix for recommendations.
These files speed up the recommendation process and eliminate the need to preprocess the data every time the app runs.

🛠️ Files Explained
tmdb_5000_credits.csv and tmdb_5000_movies.csv: Raw datasets used for preprocessing.
MovieRecSystem.py: Script for data preprocessing, feature engineering, and model creation.
app.py: Streamlit-based application for interacting with the recommendation system.
movies.pkl and similarity.pkl: Preprocessed data files used by the app.
💡 Future Enhancements
Add collaborative filtering or hybrid recommendation techniques.
Improve the user interface with enhanced visualizations.
Integrate a larger dataset for better recommendations.
