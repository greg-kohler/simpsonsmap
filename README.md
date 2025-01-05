# Web Scraping - Simpsons Guest Characters Map

This project visualizes the birthplaces of guest stars from The Simpsons as a cluster map with donut icons representing the number of guest voices from each city or town. The map is generated by scraping Wikipedia for guest star birthplaces, geocoding their birth city or town, and clustering the results. The final map is saved as an HTML. 

---

## Features
- **Web Scraping:** Collects guest star data from Wikipedia pages.
- **Geocoding:** Converts birthplace names into latitude and longitude using a geocoding API.
- **Clustering:** Groups nearby cities to prevent overcrowding on the map using DBSCAN.
- **Dynamic Visualization:** Creates a Folium map with custom donut icons sized according to the number of guest voices.

---

## Requirements

### Python Libraries
- `requests`
- `BeautifulSoup4`
- `urllib`
- `csv`
- `collections`
- `time`
- `pandas`
- `folium`
- `sklearn`
- `numpy`
- `geopy`
- `math`

### Additional Files
- `donut.png`: A donut image used as custom icons on the map.

---

## Usage
1. Run the notebook to generate the map

2. The script performs the following steps:
   - Scrapes guest star data from Wikipedia.
   - Finds birthplaces and cleans the data.
   - Geocodes the birthplaces to obtain latitude and longitude.
   - Clusters nearby cities and creates a Folium map with custom donut icons.

3. Open the generated map

---

## Output
- **`simpsons_map.html`**: A fully interactive map displaying clustered birthplaces of guest stars. Each marker shows the number of guest voices from the corresponding city.


