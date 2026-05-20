# BhuNaksha Jharkhand - Offline Map Viewer

Jharbhunaksha portal ka offline map viewer for all 22 districts of Jharkhand.

## Features
- 22 districts, 247 circles, 1,697 halkas, 26,647 mouzas
- WMS-based village maps with plot boundaries and labels
- Hierarchical selectors (District → Circle → Halka → Mouza)
- Layer toggles (Village Map, Plot Boundaries, Labels) and opacity controls
- Print / Save as PDF support
- 24,491 GIS extents (92% coverage)
- Works offline (file://) and online

## Usage
### Single-page App
Open `index.html` → select district → circle → halka → mouza → click "खोलें"

### Standalone Maps
Open `maps/index.html` → browse district/circle/halka → click mouza for direct map view

## Structure
```
index.html              - Main single-page app
assets/
  css/main.css          - Styles
  js/main.js            - App logic
  data/
    jharkhand.js        - Hierarchy data (22 districts)
    extents.js          - GIS extents (24,491 entries)
maps/                   - Standalone HTML maps (26,435 files)
```

## Data Source
Jharbhunaksha Portal - https://jharbhunaksha.jharkhand.gov.in

## Tech
- OpenLayers 4.6.5
- Vanilla JavaScript
- WMS overlay layers (plot boundaries, labels via 6 overlay layer IDs)
# map
# map
