````markdown
# Visualising Road Networks of Indian Metro Cities

This project visualises road networks of selected Indian metropolitan cities using **OpenStreetMap** data via the [OSMnx](https://github.com/gboeing/osmnx) library.  
It produces both **static maps** and **interactive maps** of the road networks, making it easier to analyse urban structures.

---

##  Features

- Fetches administrative boundaries for given cities from OpenStreetMap
- Downloads and processes road network data using OSMnx
- Plots static visualizations with **Matplotlib**
- Generates interactive maps using **Folium**
- Calculates key network metrics for comparison between cities

---

##  Dataset Source

- All spatial data is fetched directly from **OpenStreetMap** via OSMnx’s API.
- No separate dataset download is required.

---

##  Requirements

Make sure you have Python installed (>=3.8).  
Install dependencies with:

```bash
pip install osmnx networkx geopandas matplotlib folium pandas
````

---

## Usage

1. **Clone this repository**

   ```bash
   git clone https://github.com/Suman1801/road-network-visualization.git
   cd road-network-visualization
   ```

2. **Open the notebook in Jupyter**

   ```bash
   Jupyter Notebook "Visualising Road Networks.ipynb"
   ```

3. **Run all cells in order** to:

   * Install libraries
   * Fetch city boundaries
   * Download road network data
   * Plot maps (static and interactive)
   * Generate network metrics table

---

##  Step-by-Step Explanation of the Code

*(Includes installing libraries, defining cities, plotting boundaries, downloading graphs, generating static and interactive maps, and computing metrics)*

---

##  Results & Interpretation

This project generates the main outputs:

###  Road Network Metrics Table**

** Network Metrics Summary:**

| City    | Total Street Length (km) | Street Density (km/km²) | Intersection Density (/km²) | Avg Streets per Node |
| ------- | ------------------------ | ----------------------- | --------------------------- | -------------------- |
| Delhi   | 32,879.51                | 22.25                   | 104.94                      | 2.87                 |
| Mumbai  | 4,520.59                 | 11.63                   | 38.06                       | 2.76                 |
| Chennai | 9,366.40                 | 28.60                   | 124.88                      | 2.67                 |
| Kolkata | 5,737.24                 | 29.96                   | 146.52                      | 2.66                 |

**Column meanings:**

* **City** → Name of the metropolitan city analysed.
* **Total Street Length (km)** → Combined length of all streets in the network.
* **Street Density (km/km²)** → Road length per unit area; indicates how dense the road network is.
* **Intersection Density (/km²)** → Number of intersections per unit area; higher values mean more connected streets.
* **Avg Streets per Node** → Average number of streets connected to each intersection or endpoint.

**Interpretation:**

* **Kolkata** has the highest **intersection density** (146.52 /km²), showing a very connected and compact grid.
* **Delhi** has the highest **total street length** (32,879 km), reflecting its large geographic area and extensive road network.
* **Mumbai** has the lowest densities, partly due to its coastal constraints and elongated shape.
* **Chennai** combines a high **street density** with high **intersection density**, suggesting good local connectivity.

---

## 👤 Author

* **Suman Bhowmick**
  📧 [sumanbhowmick768@gmail.com](mailto:sumanbhowmick768@gmail.com)
  🌐 [GitHub Profile](https://github.com/Suman1801)

