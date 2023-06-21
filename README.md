# Chile Recent Earthquakes
Albert Lleida, 18th June 2023

This project focuses on analyzing recent earthquake data in Chile. It includes web scraping earthquake data from the sismologia.cl website, performing data transformations to enhance the dataset, conducting exploratory data analysis, and visualizing the results using Tableau.

## Libraries Used
The following Python libraries were used in this project:

- `pandas` for data manipulation and analysis
- `numpy` for numerical computations
- `matplotlib.pyplot` and `seaborn` for data visualization
- `requests` for sending HTTP requests
- `BeautifulSoup` for parsing HTML content
- `datetime` and `timedelta` for working with dates and times
- `random` and `time` for incorporating random sleep durations
- `IPython.display` for displaying formatted output
- `plotly.graph_objects` and `plotly.express` for interactive visualizations

## Project Steps

### Step 1: Web Scraping Earthquake Data from Sismologia.cl

In this step, earthquake data is scraped from the sismologia.cl website. The script sends HTTP requests, parses the HTML content using BeautifulSoup, and extracts relevant details. To avoid overwhelming the server, a random sleep duration is included between requests. Then the extracted data is stored in a pandas DataFrame.

### Step 2: Data Transformation and Cleaning

After the web scraping process, data transformations are applied to improve the quality and usability of the earthquake dataset. This involves splitting the 'Fecha Local / Lugar' column into separate 'Fecha Local' (Local Date) and 'Lugar' (Location) columns. The 'Magnitud' (Magnitude) column is refined by extracting the numerical value, and a new 'Magnitude Unit' column is added to indicate the measurement unit. Additionally, the 'Profundidad' (Depth) column is renamed as 'Depth (km)' for clarity. Any necessary data cleaning steps are performed to ensure the dataset is ready for analysis.

### Step 3: Exploratory Data Analysis

The exploratory data analysis phase involves gaining insights from the earthquake dataset. Various aspects of the earthquakes are examined, including their frequency, magnitudes, depths, and occurrence times. Visualizations are created using `matplotlib.pyplot`, `seaborn`, and `plotly` to explore the distributions and relationships between these variables. This analysis provides a better understanding of seismic activity in Chile and serves as a basis for further investigation.

## Tableau Visualization

To complement the exploratory data analysis, an interactive visualization of the earthquake data in Chile is available through Tableau. You can access the visualization by clicking on the following link: [Recent Earthquakes in Chile - Tableau Visualization](https://public.tableau.com/app/profile/albert1030/viz/RecentEarthquakesinChile/Historia1?publish=yes)

## Repository Contents

- `Chile_Recent_Earthquakes.ipynb`: Jupyter Notebook containing the project code and analysis.
- `Datasets/`: Folder containing the extracted and cleaned earthquake datasets.

