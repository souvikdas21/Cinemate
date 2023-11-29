# CINEMATE Movie Recommendation System

This is a movie recommendation system based on content-based recommendations using the TMDB 5000 movie dataset. The system utilizes cosine similarity for generating recommendations and is implemented as a web app using Streamlit.

## Data Source

The CSV files used in this project were downloaded from Kaggle. To replicate the dataset, visit [TMDB Movie Metadata on Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata/?select=tmdb_5000_credits.csv) and download the following files:
- [tmdb_5000_credits.csv](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata/?select=tmdb_5000_credits.csv)
- [tmdb_5000_movies.csv](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata/?select=tmdb_5000_movies.csv)

Place these CSV files in the `Data` folder of your project.

## Project Structure

- `app.py`: The main script for the Streamlit web app.
- `Recommender system.ipynb`: Jupyter Notebook file containing the code for building the recommendation system.
- `Data/tmdb_5000_credits.csv`: Dataset containing movie credits information.
- `Data/tmdb_5000_movies.csv`: Dataset containing movie details.
- `artifacts/movie_list.pkl`: Pickle file containing movie information.
- `artifacts/similarity.pkl`: Pickle file containing precomputed cosine similarity scores.

## Generating Pickle Files

To generate the required pickle files for the Movie Recommendation System, follow these steps:

1. Open the Jupyter Notebook file `Recommender system.ipynb`.

2. Run the cells in the notebook to execute the code for building the recommendation system.

3. After running the notebook, two pickle files will be generated in the `artifacts` directory:
   - `movie_list.pkl`: Contains movie information.
   - `similarity.pkl`: Contains precomputed cosine similarity scores.

## How to Run the Project

Now that you have generated the pickle files, you can proceed to run the Movie Recommendation System:

1. **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. **Run the Streamlit app:**

    ```bash
    streamlit run app.py
    ```

3. **Open your web browser and go to [http://localhost:8501](http://localhost:8501) to use the Movie Recommendation System.**

## Usage

1. Select or type the name of a movie in the provided dropdown menu.
2. Click the "Show recommendation" button to get a list of the top 5 recommended movies.
3. The top 5 recommended movies will be displayed with their names and posters.

## Credits

- TMDB API: [https://www.themoviedb.org/documentation/api](https://www.themoviedb.org/documentation/api)

## Notes

- Ensure you have an internet connection to fetch movie posters from the TMDB API.
