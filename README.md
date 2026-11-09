# Selah-Anya-Grid
**An offline-first geospatial resilience engine for microclimate rainfall mapping, topographic catchment optimization, and off-grid solar budgeting.**

**Author:** Inez Thomas  
**License:** All Rights Reserved (Proprietary / Closed to Derivative Works)  
**Status:** In Active Specification & Development  

---

## Overview
Selah Anya Grid is a zero-cloud Progressive Web App (PWA) engineered to operate in resource-constrained island regions, mountainous terrain, and off-grid environments without active internet connectivity. 

The engine processes client-side spatial precipitation models, topographic elevation profiles, and household utility consumption data to guide users on optimal rainwater collection zones, localized water/hardware sourcing, and off-grid solar storage requirements.

---

## Key Features

### 1. Topographic Microclimate & Rainfall Geolocator
- **Orographic Lift & Elevation Modeling:** Factors local slope, altitude, and windward/leeward exposure to calculate localized precipitation shifts across island microclimates.
- **High-Yield Spot Finder:** Pinpoints optimal physical locations on a property or local area for maximum rainfall collection based on topographic data.
- **Offline Community Resource Mapping:** Caches local water sources, community supply nodes, and regional hardware sourcing directories directly in browser storage for grid-down utility navigation.

### 2. Rainwater Catchment & Longevity Engine
- **Client-Side Spatial Math:** Calculates monthly catchment yield based on roof surface area, slope efficiency, and localized historical rainfall matrix data.
- **Water Telemetry:** Calculates "Days of Water Remaining" dynamically based on household consumption patterns and cached weather layers.

### 3. Off-Grid Solar & Storage Budgeting
- **Load Sizing Calculator:** Maps appliance energy draws against battery bank capacities ($Ah / kWh$).
- **Safety & Wiring Schematics:** Recommends electrical fuse dimensions, wire gauges (AWG), and charge controller specs for DIY off-grid builds.
- **State-of-Charge (SoC) Tracker:** Enables manual voltage logging and battery health monitoring completely offline.

---

## System Architecture 
[ GPS / Coordinate Input ] ──> [ Service Worker Cache ] ──> [ Client-Side Math Engine ]
│                              │
▼                              ▼
[ IndexedDB Storage ]        [ Leaflet/Turf.js GIS ]

- **Interface & Logic:** Vanilla JavaScript / TypeScript (Installable PWA)
- **Geospatial Engine:** Leaflet.js & Turf.js (Offline client-side vector GIS & topographic spatial interpolation)
- **Local Storage Layer:** Browser `IndexedDB` via Dexie.js (Zero external server or cloud dependency)
- **Offline Caching:** Web Service Workers (Pre-cached vector tiles & matrix data)

---

## Project Roadmap
- [x] Architecture Specification & Spatial Data Model Design
- [ ] Core Rainwater Yield & Topographic Math Engine (MVP)
- [ ] Offline Leaflet Map Tile Caching & Vector Overlay
- [ ] Off-Grid Solar Load & Battery Sizing Module
- [ ] Service Worker PWA Packaging & Local State Persistence

---

## Copyright & Legal Notice
Copyright (c) 2026 Inez Thomas. All Rights Reserved.  
No part of this repository, including the architectural designs, software code, documentation, or mathematical models, may be reproduced, distributed, modified, or transmitted in any form or by any means without the prior written permission of the copyright holder.
