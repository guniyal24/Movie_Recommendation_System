# Movie Recommendation System

A content-based movie recommendation system using TMDB dataset and Natural Language Processing techniques. The system suggests top 5 similar movies based on movie content.

## Features

- Content-based movie recommendations using NLP techniques
- Interactive web interface built with Streamlit
- Movie poster integration using TMDB API
- Cosine similarity-based movie matching
- Top 5 movie recommendations for each query

## How It Works

The recommendation system processes movie data through several steps:

1. **Data Processing**: Combines important movie features into a single 'tags' column:
   - Genre
   - Movie ID (for poster fetching)
   - Keywords
   - Overview
   - Title
   - Cast
   - Director (from crew)

2. **Text Processing**:
   - Applied Porter Stemming for word normalization
   - Created Bag of Words representation for text vectorization

3. **Similarity Calculation**:
   - Implemented cosine similarity to measure movie similarities
   - Ranks movies based on similarity scores

4. **Web Interface**:
   - Built using Streamlit for user interaction
   - Integrates TMDB API for fetching movie posters
   - Displays top 5 movie recommendations

## Technologies Used

- Python
- Pandas for data manipulation
- NLTK for text processing
- Scikit-learn for vectorization and similarity calculation
- Streamlit for web framework
- TMDB API for movie data and posters

## Installation

1. Clone the repository:
```bash
git clone https://github.com/guniyal24/Movie_Recommendation_System.git
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Set up your TMDB API key:
   - Get your API key from [TMDB website](https://www.themoviedb.org/documentation/api)
   - Add it to your environment variables or configuration file

4. Run the Streamlit app:
```bash
streamlit run app.py
```

## Usage

1. Launch the web application
2. Select a movie from the dropdown menu
3. Click the 'Recommend' button
4. View the top 5 recommended movies with their posters

## Future Improvements

- Implement collaborative filtering
- Add user ratings and reviews
- Enhance UI/UX
- Include more movie metadata
- Add movie trailers and links

## Contributing

Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.
