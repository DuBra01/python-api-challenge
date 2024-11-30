# python-api-challenge
# WeatherPy

This project analyzes weather data to explore the relationships between various weather variables (temperature, humidity, wind speed, cloudiness) and latitude. The data is visualized through scatterplots to identify trends and patterns.

## Project Overview
The purpose of this project is to:
- Gather weather data from cities around the world using the OpenWeatherMap API.
- Analyze the relationship between weather variables and latitude.
- Visualize the results through scatterplots and linear regression analysis.

## Technologies Used
- **Python 3.9+**
- **Jupyter Notebook**
- **Pandas**: For data manipulation and analysis.
- **Matplotlib**: For data visualization.
- **SciPy**: For performing linear regression.
- **OpenWeatherMap API**: For fetching real-time weather data.

## Files in This Repository
- `WeatherPy.ipynb`: The Jupyter notebook containing the full analysis.
- `.gitignore`: Ensures sensitive files (e.g., `api_keys.py`) are excluded from the repository.
- `output_data/cities.csv`: Contains weather data for the analyzed cities.

## Project Steps
1. **Generate Random Cities**: Using the `citipy` library to identify cities from randomly generated latitude and longitude values.
2. **Fetch Weather Data**: Using the OpenWeatherMap API to retrieve weather data for the identified cities.
3. **Analyze Weather Trends**:
   - Scatterplots for:
     - Latitude vs. Temperature
     - Latitude vs. Humidity
     - Latitude vs. Cloudiness
     - Latitude vs. Wind Speed
   - Linear regression for Northern and Southern Hemispheres.
4. **Document Observations**: Key takeaways from the data visualizations.

## Results
### Scatterplots
- **Latitude vs. Temperature**:
  - Observes the correlation between latitude and temperature, highlighting warmer temperatures near the equator.
- **Latitude vs. Humidity**:
  - Displays how humidity levels vary across latitudes.
- **Latitude vs. Cloudiness**:
  - Visualizes cloud cover distribution globally.
- **Latitude vs. Wind Speed**:
  - Analyzes wind speeds in different regions.

### Linear Regression
- Separate regression lines for the Northern and Southern Hemispheres provide deeper insights into trends.

## How to Run the Project
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/python-api-challenge.git
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Add your OpenWeatherMap API key to `api_keys.py`:
   ```python
   openweathermap_key = "your_api_key_here"
   ```
4. Run the `WeatherPy.ipynb` notebook using Jupyter Notebook or Jupyter Lab.

## Observations
- Temperatures decrease as you move further from the equator.
- Humidity, cloudiness, and wind speed show weaker correlations with latitude, but interesting patterns emerge when segmented by hemisphere.

## Author
This analysis was completed as part of a Python API challenge assignment.

# VacationPy

This project builds on weather data analysis to identify ideal vacation destinations based on specific weather conditions. It leverages the Geoapify API to locate nearby hotels for the selected destinations and visualizes them on an interactive map.

## Project Overview
The purpose of this project is to:
- Filter cities based on user-defined ideal weather conditions.
- Use the Geoapify API to find nearby hotels for these cities.
- Plot the selected vacation destinations on an interactive map.

## Technologies Used
- **Python 3.9+**
- **Jupyter Notebook**
- **Pandas**: For data manipulation and analysis.
- **hvPlot**: For interactive mapping.
- **Geoapify API**: For fetching hotel information and creating map visualizations.

## Files in This Repository
- `VacationPy.ipynb`: The Jupyter notebook containing the vacation destination analysis.
- `.gitignore`: Ensures sensitive files (e.g., `api_keys.py`) are excluded from the repository.
- `output_data/`: Contains any generated outputs from the analysis.

## Project Steps
1. **Filter Cities Based on Ideal Weather**:
   - Criteria include temperature, wind speed, and cloudiness.
   - Cities meeting these criteria are selected for further analysis.
2. **Fetch Hotel Data**:
   - Using the Geoapify API, hotels within a 10-kilometer radius of the selected cities are located.
3. **Create a Map**:
   - Plot the filtered cities on a map.
   - Include information about nearby hotels and city names in the hover tooltips.

## Results
- **Vacation Destinations Map**:
  - An interactive map displaying vacation destinations that meet the specified weather criteria.
  - Includes markers for cities, with hover functionality to show hotel names and city details.

## How to Run the Project
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/python-api-challenge.git
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Add your Geoapify API key to `api_keys.py`:
   ```python
   geoapify_key = "your_api_key_here"
   ```
4. Run the `VacationPy.ipynb` notebook using Jupyter Notebook or Jupyter Lab.

## Observations
- Vacation destinations are selected based on user-defined criteria, allowing tailored recommendations.
- Hotel data enriches the analysis by providing actionable insights for travelers.
- The interactive map enhances usability and visualization for destination planning.

## Author
This analysis was completed as part of a Python API challenge assignment.

