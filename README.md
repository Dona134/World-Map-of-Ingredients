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



## Data

- `recipes.csv`: Contains the recipe data with columns such as ingredients, country, etc.
- `demonyms.csv`: Contains demonyms for countries to help in mapping country names to their respective demonyms.

## Visualizations

- [`specific_ingredients_map_upd.html`](https://dona134.github.io/World-Map-of-Ingredients/specific_ingredients_map_upd.html): An interactive map showing specific ingredients used in different countries.
- [`top_ingredients_map.html`](https://dona134.github.io/World-Map-of-Ingredients/top_ingredients_map.html): An interactive map showing the top ingredients used in different countries.

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


