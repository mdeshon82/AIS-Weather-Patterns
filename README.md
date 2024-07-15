# Marine Weather, Sea State, Ocean Current, and Route Optimization Project

## Project Overview
This project analyzes weather, Marine AIS, sea state, and ocean current data to predict safe ocean crossing routes. It involves data acquisition via APIs, cleaning, merging datasets, loading into an SQLite database, developing predictive and optimization models, and visualizing the results using Tableau and PowerBI.

## Features
- Weather data from OpenWeatherMap API
- Marine AIS data from Parquet
- Sea state data from NOAA/NASA API
- Ocean current data from NOAA API
- Data cleaning and merging
- Predictive model using Random Forest
- Optimization model using linear programming
- SQLite database for storage
- Visualizations using Matplotlib, Tableau, and PowerBI
- Map of optimal ocean crossing routes

## Setup Instructions
1. Create a virtual environment and install dependencies.
    ```bash
    python -m venv env
    source env/bin/activate
    pip install pandas requests sqlite3 matplotlib seaborn scikit-learn pulp geopandas shapely contextily
    ```
2. Run the data acquisition and cleaning scripts.
    ```bash
    python data_acquisition.py
    python data_cleaning.py
    python data_merging.py
    ```
3. Load the cleaned data into SQLite.
    ```bash
    python load_to_sqlite.py
    ```
4. Develop the predictive and optimization models.
    ```bash
    python predictive_model.py
    python optimization_model.py
    ```
5. Generate and visualize the optimal routes.
    ```bash
    python generate_routes.py
    ```
6. Export the merged data and optimal route for visualization.
    ```bash
    python export_data.py
    ```

## Running the Visualizations
- Use the exported `merged_data.csv` and `optimal_route.csv` to create dashboards in Tableau and PowerBI.
