This repository contains the code developed during the 2025 NII Internship for the spatial analysis of solar power plant (SPP) siting in Japan.

The project investigates potential tensions between techno-economic suitability for solar power development and socio-environmental sensitivity. Multiple geospatial datasets are integrated into a common H3 spatial framework and combined using the Analytic Hierarchy Process (AHP). Spatial statistical methods are then used to identify and visualize potential areas of conflict.

This work builds on the previous NII internship project and its implementation of Hex2Vec / SRAI for solar power plant analysis.

Repository Structure
NII-Solar-Power-AHP/
│
├── data_processing/
│   ├── techno_economic/
│   │   ├── irradiation/
│   │   ├── slope/
│   │   ├── aspect/
│   │   ├── roads/
│   │   └── land_cover/
│   │
│   └── socio_environmental/
│       ├── biodiversity/
│       ├── sediment_risk/
│       ├── protected_areas/
│       └── land_cover/
│
├── ahp/
│   ├── techno_economic/
│   └── socio_environmental/
│
├── spatial_analysis/
│
├── visualization/
│
└── README.md
data_processing/

Contains notebooks used to prepare the individual spatial variables before their integration into the AHP models.

Techno-economic variables
Solar irradiation
Slope
Aspect
Road accessibility/density
Land cover

Socio-environmental variables
Biodiversity / Satoyama Index
Sediment and landslide risk
Protected areas
Land cover

ahp/
Contains the implementation of the Analytic Hierarchy Process (AHP) and the construction of the two main spatial indices:
Techno-economic suitability
Socio-environmental sensitivity


spatial_analysis/
Contains spatial statistical analyses used to investigate relationships and spatial mismatches between solar power development, techno-economic suitability, and socio-environmental sensitivity.
This includes analyses using Moran's I, Bivariate Moran's I, and Local Indicators of Spatial Association (LISA).

visualization/
Contains code used to produce static and interactive visualizations of the results, including interactive Folium maps.

Data
Due to the size and format of the geospatial datasets, this repository primarily contains processing and analysis code rather than the complete datasets.

Main Tools

The project primarily uses:
Python
GeoPandas
H3
SRAI / Hex2Vec
PySAL / ESDA
Folium
Matplotlib
QGIS

Previous Work

This project builds on the previous NII internship work on solar power plant detection and spatial representation learning in Japan:
Jae-Domain/Japan-GIS-Data
Jae-Domain/Japan-PV-Plant-Probability-Scoring

Author
Elisabeth Viau
NII Internship, 2025
National Institute of Informatics, Tokyo, Japan
