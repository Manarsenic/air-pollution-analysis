# Real-time and Historical Air Quality Analysis

This project is a Python-based analysis of air quality data, combining both real-time data from a live API and historical data from a CSV file. The goal is to fetch current air quality information for a specific city, visualize the pollutant levels, and analyze historical trends.

---

## Features

* **Real-time Data:** Fetches the current Air Quality Index (AQI) and individual pollutant levels from the waqi.info API.
* **Data Visualization:** Generates a pie chart to show the distribution of various pollutants and a time-series plot to visualize historical trends.
* **Geospatial Plotting:** Uses the `cartopy` library to plot the location of the air quality station on a world map.
* **Data Handling:** Utilizes the `pandas` library to clean and process historical data from a CSV file.

---

## Getting Started

To run this project, you will need to have Python and a few libraries installed.

### Prerequisites
* Python 3.x
* The project uses the following libraries:
    * `requests`
    * `pandas`
    * `matplotlib`
    * `cartopy`

### How to Run the Notebook

1.  **Clone the repository:**
    `git clone https://github.com/Manarsenic/air-pollution-analysis.git`

2.  **Install the libraries:**
    * It is recommended to use a virtual environment.
    * Install the required libraries with `pip install -r requirements.txt` (assuming you have a `requirements.txt` file).
    * The `cartopy` library may require additional system dependencies. The notebook includes `apt-get` commands for a Colab environment, which may need to be adapted for your local machine.

3.  **Get an API key:**
    * This project requires an API key for the real-time data. You can get one for free here: [https://aqicn.org/data-platform/token/#/](https://aqicn.org/data-platform/token/#/)
    * Replace `YOURAPIKEY` with your key in the notebook code.

4.  **Place the data file:**
    * The historical data analysis section reads from a CSV file. Ensure you have the `igi-airport terminal-3, delhi, delhi, india-air-quality.csv` file in the same directory as the notebook.

5.  **Run the notebook:**
    * Open `AIR_QUALITY.ipynb` in a Jupyter Notebook or Google Colab and run the cells in order.

---

## Analysis & Output

### Real-time Pollutant Graph
This pie chart visualizes the distribution of various pollutants fetched from the API.
![A pie chart showing the distribution of pollutants.](https://i.ibb.co/C0600Wq/pollutant-pie-chart.png)

### City Location Map
This map shows the location of the data source for real-time analysis.
![A map of the world with a dot over India.](https://i.ibb.co/R3Qd508/city-location-map.png)

### Historical Data Plot
This time-series plot visualizes the PM2.5 levels in Delhi over a period of time.
![A line chart showing PM2.5 values over time.](https://i.ibb.co/y4L2q4Y/historical-data-plot.png)

---

## Technologies Used

* **Python:** The core programming language for the project.
* **Pandas:** Used for data cleaning and manipulation of the historical CSV data.
* **Matplotlib:** Utilized for creating the pie charts and time-series plots.
* **Cartopy:** Used for geospatial plotting on the map.
* **Requests:** Fetches real-time data from the waqi.info API.
* **Google Colab:** The primary environment used for developing and running this project.
