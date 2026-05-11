# Angling Intelligence: Rolleston Base

A specialized web application designed for anglers based in Rolleston, New Zealand, providing a strategic reference for freshwater fishing across the North Canterbury and Central South Island regions.

## Purpose
The primary goal of this project is to consolidate essential angling data into a single, mobile-responsive dashboard. It simplifies trip planning by calculating travel distances from a Rolleston base and providing quick access to seasonal status, species identification, and tactical rigging techniques.

> ### ⚠️ Disclaimer
> The information provided in this application is populated to the best of the developer's abilities and knowledge. However, fishing regulations are subject to change and interpretation. **This page is for reference only.** Every angler MUST consult the official National and Local Fish & Game regulations before heading out. The developer takes no responsibility for any inaccuracies or regulatory breaches resulting from the use of this tool.

---

## Functionality

### 📍 Strategic Map
*   **Distance Calculation:** All locations are sorted by their driving distance from Rolleston.
*   **Real-Time Status:** Sites are automatically flagged as **OPEN** or **CLOSED** based on the current date and specific regional season dates (including complex "First Saturday of November" high-country starts).
*   **Interactive Filtering:** Toggle visibility of open/closed sites to focus on available targets.
*   **Detailed Intel:** Click any location to see bag limits, permitted methods, recommended lures, and "prime time" tips.

### 📜 Regulations
*   Integrated PDF viewers for official Fish & Game regulation booklets.
*   Quick-switch tabs for North Canterbury and Central South Island regions.

### 🐟 Species ID
*   A visual guide to target species in the region, including Brown Trout, Rainbow Trout, Chinook Salmon, Perch, and Tench.
*   Provides identification markers, habitat notes, and suggested lures for each species.

### 🪢 Tactical Knots
*   High-quality visual diagrams and step-by-step instructions for essential angling connections.
*   Covers terminal tackle (Palomar, Snell), line-to-line (Double Uni, Blood Knot, FG), and loop creation (Surgeon's Loop).

### 🔗 Useful Links
*   A curated list of external resources, including access point maps, licensing portals, and regional information.

---

## Technical Details

### Tech Stack
*   **Frontend:** HTML5, CSS3 (Tailwind CSS)
*   **Mapping:** [Leaflet.js](https://leafletjs.com/) with OpenStreetMap tiles.
*   **Data:** Vanilla JavaScript data structures for locations and resources.
*   **Hosting:** Designed to run in any modern web browser; works locally via `file://` or hosted on any static web server.

### License & Usage
This repository is **public** and available for anyone to clone, modify, and reuse for their own personal or community projects.

**No Warranty:**
The software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.
