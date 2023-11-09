# Chile's Seismic Insights (2010-2023)
##  Web Scraping, Data Analysis, and exploration with Python and Tableau
**Albert Lleida, 18th June 2023** (Updated, 7th November 2023)

This project focuses on analyzing recent earthquake data in Chile. It includes **web scraping** earthquake data from the sismologia.cl website, performing **data transformations** to enhance the dataset, conducting **exploratory data analysis**, and **visualizing the results using Tableau**.

<div align="center">
  <img width="700" alt="Captura de pantalla 2023-11-07 a las 23 02 12" src="https://github.com/alleida23/Chile_Recent_Earthquakes/assets/124719215/d03b2eb4-a527-4076-9a3e-bc7639caa381">
</div>

## Libraries Used
The following Python libraries were used in this project:

- pandas for data manipulation and analysis
- numpy for numerical computations
- matplotlib.pyplot and seaborn for data visualization
- requests for sending HTTP requests
- BeautifulSoup for parsing HTML content
- datetime and timedelta for working with dates and times
- random and time for incorporating random sleep durations
- IPython.display for displaying formatted output
- plotly.graph_objects and plotly.express for interactive visualizations

## Project Steps
### Step 1: Web Scraping Earthquake Data from Sismologia.cl
In this step, earthquake data is scraped from the sismologia.cl website. The script sends HTTP requests, parses the HTML content using BeautifulSoup, and extracts relevant details. To avoid overwhelming the server, a random sleep duration is included between requests. Then the extracted data is stored in a pandas DataFrame.

### Step 2: Data Transformation and Cleaning
After the web scraping process, data transformations are applied to improve the quality and usability of the earthquake dataset. This involves splitting the 'Fecha Local / Lugar' column into separate 'Fecha Local' (Local Date) and 'Lugar' (Location) columns. The 'Magnitud' (Magnitude) column is refined by extracting the numerical value, and a new 'Magnitude Unit' column is added to indicate the measurement unit. Additionally, the 'Profundidad' (Depth) column is renamed as 'Depth (km)' for clarity. Any necessary data cleaning steps are performed to ensure the dataset is ready for analysis.

### Step 3: Exploratory Data Analysis
The exploratory data analysis phase involves gaining insights from the earthquake dataset. Various aspects of the earthquakes are examined, including their frequency, magnitudes, depths, and occurrence times. Visualizations are created using matplotlib.pyplot, seaborn, and plotly to explore the distributions and relationships between these variables. This analysis provides a better understanding of seismic activity in Chile and serves as a basis for further investigation.

## Tableau Visualization - Updated (7th November 2023)

<div align="center">
  <img width="700" alt="Captura de pantalla 2023-11-07 a las 22 29 53" src="https://github.com/alleida23/Chile_Recent_Earthquakes/assets/124719215/476ee5a4-09cc-4444-a199-5f0a9b365e3c">
</div>


To complement the exploratory data analysis, an interactive visualization of the earthquake data in Chile is available through Tableau. You can access the visualization by clicking on the following link: [Recent Earthquakes in Chile - Tableau Visualization](https://public.tableau.com/app/profile/albert1030/viz/HexBin-ChilesEarthquakes/Historia1?publish=yes).

The earthquake dataset has been significantly expanded, now covering records from 2010 to the current date, totaling almost 100k rows of earthquake data. As a result, the Tableau visualization has been extensively updated, incorporating HexBin Heat Maps, Scatter plots, Bar charts, and more interactive features, providing better insights into Chile's seismic activity. For a detailed breakdown of the visualization improvements and additional challenges faced, a separate repository has been created: [Tableau_Viz_Challenges](https://github.com/alleida23/Tableau_Viz_Challenges/tree/main/WOW22_W16_HexBin_Map).


This update section highlights the expansion of the dataset and the enhanced Tableau visualization while retaining the original structure and content.

---

## Repository Contents
- **Chile_Earthquakes_2010_2023.ipynb:** Jupyter Notebook containing the project code and analysis.
- **Datasets/:** Folder containing the extracted and cleaned earthquake datasets.
