Movie Recommender System with Python
This project implements a Movie Recommender System using Python, Pandas, and correlation-based filtering techniques. The goal is to provide personalized suggestions to users based on movie similarity and user rating patterns.

 Project Overview
The system analyzes a movie dataset (titles and ratings) to identify preference patterns. It uses statistical correlation to find movies that are most similar to a specific user-selected title.

Key Features:
Exploratory Data Analysis (EDA): Visualization of rating distributions and the relationship between the number of ratings and the average score.

Correlation-Based Recommendation: Suggests similar movies by calculating the Pearson correlation between user rating profiles.

Data Processing: Cleaning and structuring user-movie matrices using Pandas pivot_table.

🛠️ Technologies Used
Python 3.x

Pandas: For data manipulation and analysis.

NumPy: For numerical computations.

Matplotlib & Seaborn: For creating statistical visualizations and plots.

Jupyter Notebook: Development environment.

📊 Visualizations
The notebook includes detailed analysis through:

Histograms: Showing how ratings are distributed across the dataset.

Jointplots: Visualizing data density and the trend between a movie's popularity (number of ratings) and its quality (average rating).

📋 Requirements & Installation
To run this project locally, ensure you have the following libraries installed:

Bash

pip install pandas numpy matplotlib seaborn
Clone the repository:

Bash
git clone https://github.com/Andr3sSanch2z/Movie-recomender-system-with-python.git
Launch the project: Open the Movie Recommender System with Python.ipynb file in Jupyter Notebook, JupyterLab, or VS Code.

Datasets: Make sure the u.data and Movie_Id_Titles.csv files are in the same directory as the notebook.

💡 How It Works
Data Loading: The system imports datasets containing user IDs, movie IDs, ratings, and movie titles.

Matrix Creation: A pivot table is created where columns represent movie titles, indices represent user IDs, and values represent ratings.

Similarity Calculation: By selecting a specific movie (e.g., Star Wars), the system calculates its correlation with all other movies in the matrix.

Filtering: Results are filtered to ensure recommendations have a significant number of ratings, avoiding outliers or niche movies with skewed scores.
