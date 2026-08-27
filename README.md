
# NII Solar Power AHP

This repository contains the code developed during the 2025 NII Internship for the spatial analysis of solar power plant (SPP) siting in Japan.

The project investigates potential tensions between **techno-economic suitability** for solar power development and **socio-environmental sensitivity**. Multiple geospatial datasets are integrated into a common H3 spatial framework and combined using the Analytic Hierarchy Process (AHP). Spatial statistical methods are then used to identify and visualize potential areas of conflict.

This work builds on the previous NII internship project and its implementation of Hex2Vec / SRAI for solar power plant analysis.


```text
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
```

## Data Processing

Contains notebooks used to prepare the individual spatial variables before their integration into the AHP models.

### Techno-economic variables

- Solar irradiation
- Slope
- Aspect
- Road accessibility/density
- Land cover

### Socio-environmental variables

- Biodiversity / Satoyama Index
- Sediment and landslide risk
- Protected areas
- Land cover

## AHP

Contains the implementation of the Analytic Hierarchy Process (AHP) and the construction of the two main spatial indices:

- **Techno-economic suitability**
- **Socio-environmental sensitivity**

## Spatial Analysis

Contains spatial statistical analyses, including Moran's I, Bivariate Moran's I, and Local Indicators of Spatial Association (LISA).

## Visualization



Author
Elisabeth Viau
NII Internship, 2025
National Institute of Informatics, Tokyo, Japan
