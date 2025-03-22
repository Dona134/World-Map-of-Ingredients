# World Food Map Project

This project aims to analyze and visualize the ingredients used in recipes from different countries. The analysis includes generating TF-IDF scores for ingredients and mapping the top ingredients for each country.

## Project Structure

- `countries.cpg`: Country data file.
- `countries.dbf`: Country data file.
- `countries.html`: Country data file.
- `countries.prj`: Country data file.
- `countries.shp`: Country data file.
- `countries.shx`: Country data file.
- `countries.txt`: Country data file.
- `demonyms.csv`: CSV file containing demonyms for countries.
- `main_tf_idf.ipynb`: Jupyter notebook for TF-IDF analysis.
- `main_top15.ipynb`: Jupyter notebook for analyzing the top 15 ingredients.
- `recipes.csv`: CSV file containing recipe data. Link: https://www.kaggle.com/datasets/irkaal/foodcom-recipes-and-reviews
- `specific_ingredients_map_upd.html`: HTML file for specific ingredients map.
- `top_ingredients_map.html`: HTML file for top ingredients map.
- `.vscode/settings.json`: VS Code settings file.

## Notebooks

### main_tf_idf.ipynb

This notebook focuses on analyzing recipe ingredients using the TF-IDF (Term Frequency-Inverse Document Frequency) method to identify the most specific ingredients associated with each country. The steps involved are:

1. **Import Libraries**: The necessary libraries such as `pandas`, `numpy`, and `os` are imported to handle data manipulation and file operations.

2. **Load Data**: The recipe data is loaded from a CSV file named `recipes.csv`.

3. **Preprocess Data**: Unnecessary columns are removed from the dataset, and the data is cleaned to ensure consistency.

4. **Clean Text**: A function is defined to clean and convert list or set columns to strings, making the data easier to work with.

5. **Apply Cleaning Function**: The cleaning function is applied to relevant columns in the dataset.

6. **Extract Country Tags**: The `demonyms.csv` file is loaded and cleaned to create a dictionary that maps country names and adjectives. This helps in identifying country mentions in the text.

7. **Detect Country Mentions**: A function is defined and applied to detect mentions of countries in the text fields of the dataset.

8. **Clean Ingredients Column**: The ingredients column is normalized by lemmatizing the ingredients and removing duplicates to ensure uniformity.

9. **Expand Data**: The dataset is expanded by splitting country tags and ingredients into multiple rows, facilitating detailed analysis.

10. **Count Ingredient Occurrences**: The occurrences of each ingredient per country are counted to understand the distribution of ingredients.

11. **TF-IDF Analysis**: The TF-IDF scores for ingredients are computed to identify the most specific ingredients for each country.

12. **Extract Specific Ingredients**: The most specific ingredients for each country are extracted based on their TF-IDF scores.

13. **Map Ingredients**: The specific ingredients are mapped to countries on a world map using the `folium` library, providing a visual representation of the data.


## Data

- `recipes.csv`: Contains the recipe data with columns such as ingredients, country, etc.
- `demonyms.csv`: Contains demonyms for countries to help in mapping country names to their respective demonyms.

## Visualizations

- [`top_ingredients_map.html`](https://dona134.github.io/World-Map-of-Ingredients/top_ingredients_map.html): An interactive map showing the top ingredients used in different countries.
- [`specific_ingredients_map_upd.html`](https://dona134.github.io/World-Map-of-Ingredients/specific_ingredients_map_upd.html): An interactive map showing specific ingredients using TF-IDF.


## Setup

1. Clone the repository.
2. Install the required dependencies.
3. Open the Jupyter notebooks (`main_tf_idf.ipynb` and `main_top15.ipynb`) and run the cells to perform the analysis.

## Requirements

- Python 3.x
- Jupyter Notebook
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## Usage

1. Open `main_tf_idf.ipynb` to perform TF-IDF analysis on the recipe ingredients.
2. Open `main_top15.ipynb` to analyze the top 15 ingredients used in recipes from different countries.
3. View the generated maps (`specific_ingredients_map_upd.html` and `top_ingredients_map.html`) for visual insights.


