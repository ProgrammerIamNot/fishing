Rolleston Angling Strategic Map

A lightweight, zero-build single-page application (SPA) providing geospatial intelligence, regulatory constraints, and tactical reference data for angling in the North Canterbury region, centered around Rolleston, NZ.

Architecture

This project is designed as a standalone static application requiring no backend infrastructure or build pipelines.

Core Logic: Vanilla JavaScript (ES6+).

Geospatial Rendering: Leaflet.js native canvas rendering.

Styling: Tailwind CSS via CDN for rapid utility-class UI generation.

Hosting: Configured for highly available, zero-cost deployment via GitHub Pages.

Core Capabilities

Strategic Map: Interactive spatial mapping of primary fishing targets relative to Rolleston.

Dynamic Status Engine: Real-time evaluation of "Open" or "Closed" season status. The engine parses complex string rules (e.g., cross-year wraps, High Country 1st-Saturday-of-November overrides) against the user's current system clock.

Species Identification Matrix: Visual and behavioral data for target species, including bite kinematics and suggested lures.

Tactical Knots: Structural diagrams and step-by-step methodologies for terminal tackle and line-to-line connections.

Local Execution

No local server is strictly required. Clone the repository and open index.html directly in any modern web browser.

git clone [https://github.com/YOUR_USERNAME/rolleston-angling-map.git](https://github.com/YOUR_USERNAME/rolleston-angling-map.git)
cd rolleston-angling-map
# Open index.html in your browser


Data Management

All spatial and regulatory data is stored in memory within the locations array inside the <script> tag of index.html.

To append a new location, insert a new object into the array using the established schema:

{ 
  id: "L13", 
  name: "New Location", 
  coords: [-43.1234, 172.5678], // [Latitude, Longitude]
  dist: "15", 
  distRaw: 15, // Used for ascending distance sort
  limit: "2 Trout", 
  season: "Oct 1 - Apr 30", // Use 3-letter month abbreviations
  fish: "Brown Trout", 
  methods: "FS", 
  lures: "Spinners", 
  times: "Evening" 
}


Asset Structure

Static image assets for Species ID and Knot diagrams should be placed in the /images/ directory. The DOM expects relative paths (e.g., ./images/brown_trout.jpg). Ensure filenames match exactly to prevent 404 errors during client-side rendering.