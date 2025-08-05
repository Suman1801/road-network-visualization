````markdown
# Visualising Road Networks of Indian Metro Cities

This project visualises the road networks of selected Indian metropolitan cities using OpenStreetMap data via the [OSMnx](https://github.com/gboeing/osmnx) library.  
It produces both static maps and interactive maps, making it easier to analyse and compare urban road structures.

---

## Features

- Retrieves administrative boundaries for selected cities from OpenStreetMap
- Downloads and processes road network data using OSMnx
- Plots static visualisations with Matplotlib
- Generates interactive maps using Folium
- Calculates key network metrics for cross-city comparison

---

## Dataset Source

- All spatial data is obtained directly from OpenStreetMap via OSMnx’s API.
- No separate dataset download is required.

---

## Requirements

Ensure you have Python 3.8 or higher installed.  
Install dependencies with:

```bash
pip install osmnx networkx geopandas matplotlib folium pandas
````

---

## Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/Suman1801/road-network-visualization.git
   cd road-network-visualization
   ```

2. Open the notebook in Jupyter:

   ```bash
   jupyter notebook "Visualising Road Networks.ipynb"
   ```

3. Run all cells in order to:

   * Install required libraries
   * Fetch city boundaries
   * Download road network data
   * Plot maps (static and interactive)
   * Generate the network metrics table

---

## Step-by-Step Code Workflow

The notebook covers:

1. Installing and importing required libraries
2. Defining a list of cities for analysis
3. Downloading administrative boundaries
4. Plotting static boundary maps
5. Downloading road network graphs
6. Creating static road network visualisations
7. Building interactive maps with Folium
8. Calculating and summarising key network metrics

---

## Results and Interpretation

The main output is a road network metrics table and the corresponding visualisations.

### Network Metrics Summary

| City    | Total Street Length (km) | Street Density (km/km²) | Intersection Density (/km²) | Avg Streets per Node |
| ------- | ------------------------ | ----------------------- | --------------------------- | -------------------- |
| Delhi   | 32,879.51                | 22.25                   | 104.94                      | 2.87                 |
| Mumbai  | 4,520.59                 | 11.63                   | 38.06                       | 2.76                 |
| Chennai | 9,366.40                 | 28.60                   | 124.88                      | 2.67                 |
| Kolkata | 5,737.24                 | 29.96                   | 146.52                      | 2.66                 |

**Column definitions:**

* City → Name of the metropolitan city analysed.
* Total Street Length (km) → Combined length of all streets in the network.
* Street Density (km/km²) → Road length per unit area; indicates how dense the road network is.
* Intersection Density (/km²) → Number of intersections per unit area; higher values mean more connected streets.
* Avg Streets per Node → Average number of streets connected to each intersection or endpoint.

**Key insights:**

* Kolkata has the highest intersection density (146.52 /km²), showing a very connected and compact urban grid.
* Delhi has the largest total street length (32,879 km), reflecting its vast area and extensive road network.
* Mumbai has the lowest densities, likely due to its narrow coastal geography.
* Chennai combines high street density with high intersection density, indicating good local connectivity.

---

## Author

Suman Bhowmick

Email: [sumanbhowmick768@gmail.com](mailto:sumanbhowmick768@gmail.com)
GitHub: [https://github.com/Suman1801](https://github.com/Suman1801)

---
