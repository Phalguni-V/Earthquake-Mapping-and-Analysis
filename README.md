Earthquake Mapping and Analysis
Overview
This project charts global earthquake activity from 1970 to 2010 and displays the data in an interactive map. It combines historical data with real-time earthquake data from 2010 to 2024 to visualize earthquake patterns globally. The project aims to help analyze regions' vulnerability to earthquakes, understand their geographical spread, and assess the severity of past earthquakes.

Features
Historical Earthquake Analysis (1970-2010): Visualizes earthquake magnitudes over the years using line graphs.

Interactive Map: Displays earthquakes since 2010, categorized by magnitude, allowing users to explore earthquake data globally.

Categorized Data: Earthquakes are classified into three categories based on their magnitude:

Moderate Impact (Magnitude 4-6)
Major Impact (Magnitude 6-8)
Great Impact (Magnitude 8+)

Dynamic Markers: The map displays interactive markers with location, date, and magnitude information for each earthquake.

Installation
Clone this repository:

bash
Copy
Edit
git clone https://github.com/your-username/earthquake-mapping.git
Navigate to the project directory:

bash
Copy
Edit
cd earthquake-mapping
Install the required Python packages:

bash
Copy
Edit
pip install matplotlib pandas geopandas folium contextily requests
Download the dataset data_static.csv for historical earthquake data and place it in the project directory.

Usage
The script loads and processes earthquake data for the years 1970-2010 and visualizes the earthquake magnitudes.

The interactive map is generated using Folium, with markers representing earthquake locations. Markers are color-coded by severity:

Orange for Moderate Impact (Magnitude 4-6)

Red for Major Impact (Magnitude 6-8)

Blue for Great Impact (Magnitude 8+)

The map includes earthquake data from the past 10 years (2010-2024), retrieved via the RapidAPI service.

To run the script, execute the following in your terminal:

bash
Copy
Edit
python earthquake_mapping.py
Data Source
Historical earthquake data from 1970-2010 is stored in data_static.csv.

Real-time earthquake data (2010-2024) is retrieved from the EveryEarthquake API.

Output
A line graph showing earthquake magnitudes over the years 1970-2010.

An interactive map that plots earthquake locations, color-coded by magnitude:
Moderate Impact (orange markers)
Major Impact (red markers)
Great Impact (blue markers)