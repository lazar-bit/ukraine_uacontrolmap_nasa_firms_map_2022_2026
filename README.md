# Ukraine UAControlMap + NASA FIRMS 2022–2026

## Overview

This repository contains an **interactive Kepler.gl-based geospatial visualization** combining:

- **UAControlMap frontline and territorial control data**
- **NASA FIRMS fire detection data (MODIS/VIIRS)**

covering Ukraine from **2022 to 2026**.

The objective of this project is to support **OSINT research and spatial-temporal analysis of conflict dynamics**, enabling the exploration of correlations between:

- frontline movement and territorial control changes  
- satellite-detected thermal anomalies (fire activity)  
- spatial clustering of high-intensity events over time  

The result is a **multi-layer geospatial analytical map** designed for exploratory and research use.

---

## Live Map

Access the interactive visualization here:

👉 https://lazar-bit.github.io/ukraine_uacontrolmap_nasa_firms_map_2022_2026/index.html

> **Note:** The visualization is optimized for desktop browsers. Due to WebGL rendering constraints, performance on mobile devices may be limited.

---

## Features

- **Dual geospatial data integration**
  - UAControlMap frontline and territorial control polygons
  - NASA FIRMS satellite fire detection points

- **Spatio-temporal analysis**
  - Multi-year dataset (2022–2026)
  - Time-enabled filtering and exploration

- **High-density visualization techniques**
  - Hexbin aggregation for FIRMS data
  - Polygon overlays for territorial dynamics

- **Interactive exploration**
  - Zoom, pan, and layer toggling
  - Temporal navigation of fire detections

- **Desktop-optimized performance**
  - Designed for analytical workloads rather than mobile usage

---

## Data Sources

### NASA FIRMS

NASA FIRMS provides near real-time satellite-based fire detection using MODIS and VIIRS instruments.

- Fire detection (thermal anomalies)
- Global coverage with high temporal frequency
- Used here for spatial-temporal clustering analysis

🔗 https://firms.modaps.eosdis.nasa.gov/

---

### UAControlMap

UAControlMap is an open-source OSINT conflict mapping project providing territorial control and frontline datasets related to the war in Ukraine.

- Frontline geometry updates
- Territorial control visualization
- Open-source geospatial conflict mapping

🔗 https://uacontrolmap.com/

---

## Usage

### Web Access

Simply open the live map:

- https://lazar-bit.github.io/ukraine_uacontrolmap_nasa_firms_map_2022_2026/index.html

No installation or setup required.

---

### Local Usage

To run locally:

```bash
git clone https://github.com/lazar-bit/ukraine_uacontrolmap_nasa_firms_map_2022_2026.git
cd ukraine_uacontrolmap_nasa_firms_map_2022_2026
```

Then open:

`index.html`

in a modern browser (Chrome recommended).

---

## Technical Notes

- **Visualization engine:** Kepler.gl  
- **Rendering stack:** WebGL (deck.gl + Mapbox GL JS)  
- **Hosting:** GitHub Pages  
- **Data format:** Preprocessed GeoJSON / CSV  
- **Map type:** Multi-layer spatio-temporal analytical dashboard  

---

## Performance Considerations

Due to dataset scale and rendering complexity:

- Initial loading may take time  
- High memory usage in browser is expected  
- Performance depends on GPU/WebGL support  

### Recommended setup

- Desktop browser (Chrome or Firefox)  
- Hardware acceleration enabled  

---

## Limitations

- FIRMS data represents satellite-detected thermal anomalies, not confirmed causes  
- Spatial correlation does not imply operational attribution  
- UAControlMap data reflects OSINT-based interpretations of frontline conditions  

---

## Disclaimer

This project is intended strictly for academic, OSINT, and research purposes.

It does not provide operational intelligence and does not verify causal relationships between fire detections and military activity. FIRMS data should be interpreted as remote sensing observations only.

---

## Acknowledgements

- NASA FIRMS for open satellite fire detection data  
- UAControlMap contributors for open-source geospatial conflict mapping  
- Kepler.gl / Uber for open-source geospatial visualization tools  
