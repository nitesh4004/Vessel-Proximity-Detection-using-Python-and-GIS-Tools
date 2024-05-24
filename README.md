Vessel Proximity Detection using Python and GIS Tools
This repository contains the source code for detecting vessel proximity events in a marine region using vectorized operations and spatial indexing techniques. The project leverages Python, Pandas, GeoPandas, and Matplotlib for data processing, spatial analysis, and visualization.

Overview
The goal of this project is to identify instances where a vessel comes into close proximity with another vessel in a designated marine region. This activity is referred to as ‘vessel proximity’. The proximity detection algorithm uses the Haversine formula for distance calculation and employs spatial indexing for efficiency.

Features

Data Loading: Load vessel position data from CSV files.
Vectorized Distance Calculation: Efficiently calculate distances between vessels using the Haversine formula.
Proximity Detection: Identify proximity events using spatial indexing techniques.
Data Visualization: Visualize vessel positions and proximity events on a map.

Tools and Technologies

Python: For data processing and analysis.
Pandas: For data manipulation.
GeoPandas: For spatial analysis and handling geospatial data.
Matplotlib: For data visualization.
Shapely: For geometric operations.
SciPy: For spatial indexing with cKDTree.

Installation

Clone the repository:

Copy code
git clone https://github.com/your-username/vessel-proximity-detection.git
cd vessel-proximity-detection
Create a virtual environment and activate it:

Copy code
python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
Install the required dependencies:

Copy code
pip install -r requirements.txt
Usage
Place your vessel position CSV file in the root directory.

Run the script to detect proximity events and export the results to a CSV file:

Copy code
python detect_proximity.py
The output CSV file containing the proximity events will be saved as proximity_events.csv.

To visualize the vessel positions and proximity events, run:


Copy code
python visualize_proximity.py
File Structure
detect_proximity.py: Script to detect vessel proximity events.
visualize_proximity.py: Script to visualize vessel positions and proximity events.
requirements.txt: List of required Python packages.
README.md: Project overview and instructions.
Import Data
The sample_data.csv file should contain the following columns:

mmsi: Maritime Mobile Service Identity number of the vessel.
timestamp: Timestamp of the vessel position.
lat: Latitude of the vessel position.
lon: Longitude of the vessel position.
