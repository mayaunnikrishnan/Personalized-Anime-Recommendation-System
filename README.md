# Personalized Anime Recommendation System

## Overview

The **Personalized Anime Recommendation System** is a web application designed to recommend anime titles similar to a given input based on a predefined list of popular anime. The application uses text-based similarity techniques to suggest anime that users might enjoy based on their preferences.
To enjoy the Application Follow the [Link](https://personalized-anime-recommendation-system-qgjftvyh7shhategpcahy.streamlit.app/)
## Key Features

### User Interface

- **Anime Selection**: Users can select an anime title from a dropdown menu containing a curated list of popular anime.
- **Number of Recommendations**: Users can specify the number of similar anime they want to receive through a slider, allowing them to choose between 1 and 20 recommendations.

### Recommendation Engine

- **Data Processing**: The system processes data from an anime dataset, including information such as genre, type, and rating.
- **Feature Combination**: Text features are combined into a single feature set for each anime entry in the dataset.
- **Similarity Calculation**: Using TF-IDF (Term Frequency-Inverse Document Frequency) and cosine similarity, the system calculates how similar each anime is to the one selected by the user.

### Output

- **Recommendations**: Based on the calculated similarities, the system retrieves and displays anime titles that are most similar to the selected title. The number of recommendations is determined by the user’s input.

## How It Works

1. **Data Loading and Preprocessing**:
   - The dataset containing anime information is loaded and preprocessed to handle missing values and combine relevant features into a single text field.

2. **Feature Extraction**:
   - Combined features are transformed into numerical data using TF-IDF Vectorization, allowing the system to understand and compare textual data.

3. **Similarity Computation**:
   - The system calculates cosine similarity between the user-selected anime and all others in the dataset to find the most similar titles.

4. **User Interaction**:
   - Users interact with the web app by selecting an anime from the dropdown and adjusting the slider to specify how many recommendations they want. Upon clicking the recommend button, the app displays the suggested anime titles based on similarity scores.

## Technical Components

- **Streamlit**: Used to create the web interface and interactive elements.
- **Pandas**: Utilized for data manipulation and handling.
- **Scikit-learn**: Provides tools for TF-IDF Vectorization and calculating cosine similarity.

## Getting Started

1. **Install Dependencies**:
   Ensure you have the necessary Python packages installed. You can install them using pip:
   ```bash
   pip install streamlit pandas scikit-learn
