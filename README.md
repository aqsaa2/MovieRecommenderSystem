# Content-Based Movie Recommender System

## Overview
This project implements a **Content-Based Filtering** approach to recommend movies based on user preferences. It involves preprocessing and cleaning movie data, building a recommendation model using a custom similarity matrix, and deploying a user-friendly interface using **Streamlit** and **Flask**.

---

## Features
- 📽️ **Content-Based Filtering**: Recommends movies by analyzing the similarity between movie features.
- 🧹 **Data Cleaning**: Ensures clean and consistent data for accurate recommendations.
- ⚡ **Custom Similarity Matrix**: Utilizes a pre-computed `similarity.pkl` file for efficient recommendations.
- 🖥️ **Interactive Interface**: Built with Streamlit and Flask for easy interaction and visualization.
- 🚀 **Scalable Design**: Suitable for integration with larger datasets and additional features.

---

## Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/aqsaa2/MovieRecommenderSystem.git
2. Navigate to the project directory:
   
 cd Content-Based-Movie-Recommender
3. Install the required dependencies:

pip install -r requirements.txt

## Usage

**Note:** The `similarity.pkl` file is not included in the repository due to file size limitations.
1. **Launch the application:**
   ```bash
   streamlit run app.py
## Project Workflow

### **1. Data Preparation**
- Cleaned raw movie data for inconsistencies and missing values.
- Generated a new DataFrame with movie features relevant for recommendations.

### **2. Model Creation**
- Implemented content-based filtering using vectorized movie features.
- Computed cosine similarity and saved the similarity matrix in `similarity.pkl`.

### **3. Interface Development**
- Created a user interface using **Streamlit**.
- Integrated **Flask** for seamless backend processing.

---

## **Dependencies**
- **Python** 3.8+
- **Flask**
- **Streamlit**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Pickle** (for saving and loading the similarity matrix)


## Project Structure
MovieRecommenderSystem/│ ├── app.py # Main Streamlit app script ├── movie-recommendation-system.ipynb # Jupyter notebook for data preprocessing and model creation ├── movies.pkl # Serialized movies data ├── movies_dict.pkl # Serialized movies dictionary ├── procfile # Heroku deployment configuration ├── requirements.txt # List of dependencies ├── setup.sh # Setup script for deployment ├── README.md # Project documentation ├── .gitignore # Git ignore file

## Examples
Input: User selects a favorite movie from the list.
Output: A list of movies similar to the selected one, ranked by similarity score.

## Future Enhancements
Integrate additional filtering methods such as collaborative filtering.
Add support for user ratings and preferences.
Enhance the UI with more visualizations and interactivity.

