# WithKids (ウィズキッズ)

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

[WithKids](https://code4fukui.github.io/withkids/) is an app for finding child-friendly activities in Ikeda Town, Fukui, Japan. It allows users to filter local attractions and facilities by age group.

The main interface presents a list of activities as collapsible cards. A side navigation menu allows filtering by age, and an interactive map shows points of interest in the area.

## Features
- **Age-Based Filtering:** Recommends activities for specific age groups (0-3, 4-10, and 11+ years).
- **Interactive Map:** The "今どこ?池田マップ" (Where am I? Ikeda Map) displays various points of interest, including:
    - Tourist Spots & Vending Machines
    - Gas Stations & Bus Stops
    - Public Toilets, AEDs, WiFi Hotspots
    - Emergency Facilities
- **Open Data Integration:** Fetches location data by sending SPARQL queries to the `odp.jig.jp` endpoint.
- **Google Maps Integration:** Provides static map previews and links to Google Maps for directions.
- **Responsive Design:** A mobile-first interface built with Materialize CSS that works on desktop and mobile devices.

## Technology Stack
- **Frontend:** HTML5, CSS3, JavaScript
- **Frameworks/Libraries:**
    - [jQuery](https://jquery.com/) (v2.1.1 & v3.1.1)
    - [Materialize](http://materializecss.com/) (v0.97.7)
- **APIs & Data Sources:**
    - **Google Maps JavaScript API:** Powers the interactive map, static map generation, and directions.
    - **SPARQL Endpoint:** Queries against `https://sparql.odp.jig.jp` for open data on civic facilities and points of interest.

## Getting Started
1.  Clone the repository.
    ```bash
    git clone https://github.com/code4fukui/withkids.git
    ```
2.  A Google Maps API key is required. The project uses a hardcoded key found in `js/main.js` and `map/index.html`.
3.  Serve the project files using a local web server.
4.  Open `index.html` to view the main application. The map is available at `/map/`.

## Credits and Special Thanks
This project is based on [AKIJIKAN](https://github.com/howml/akijikan/), which was itself based on [OGARUCO](http://ogaruco.net/).

We extend our deepest gratitude to Mr. Kawahito of Code for Sabae (aka [Dappi Studio](http://www.dappi.jp)).

## License
This project is licensed under the MIT License.