# Motor Vehicle Collisions in NYC - Streamlit Dashboard

This Streamlit dashboard is designed to analyze motor vehicle collisions in New York City (NYC). It provides interactive visualizations and insights into the collision data from the specified CSV file.

## Data Source
The data used for this analysis is sourced from the data located at the website https://www.nyc.gov/site/nypd/stats/traffic-data/traffic-data-collision.page.

## Usage
To use this dashboard, make sure you have the required dependencies installed. You can run the application by executing the script containing the code.

```bash
streamlit run app.py
```

## Features

### 1. Map Visualization - Injured People
- Use the slider to select the number of people injured in vehicle collisions.
- The map will display the locations of collisions where the number of injured people is greater than or equal to the selected value.

### 2. Collisions by Time of Day
- Use the sidebar slider to select the hour to analyze.
- The map will show the vehicle collisions that occurred during the selected hour.
- The HexagonLayer visually represents the collision density in the area.

### 3. Breakdown by Minute
- The bar chart displays the number of collisions that occurred each minute during the selected hour.

### 4. Top 5 Dangerous Streets by Affected Type
- Choose between Pedestrians, Cyclists, and Motorists to view the top 5 streets with the highest number of injuries for the selected affected type.

### 5. Show Raw Data
- Check this box to view the raw data used for the visualizations.

## Data Processing
The data from the CSV file is preprocessed using the `load_data` function to handle missing values, rename columns, and parse dates for better analysis.

## Visualization Libraries Used
- `streamlit`: Used to create the interactive web application.
- `pandas`: Used for data manipulation and analysis.
- `numpy`: Used for numerical computations.
- `pydeck`: Used for creating 3D visualizations.
- `plotly`: Used for creating interactive visualizations and charts.

## Note
Please ensure that the `data.csv` file is available at the specified location before running the application.

Feel free to explore the dashboard and gain valuable insights into motor vehicle collisions in NYC. This app was created when studying the course "Build a Data Science Web App with Streamlit and Python" https://www.coursera.org/projects/data-science-streamlit-python.
For any questions or feedback, please contact me. Happy analyzing!
