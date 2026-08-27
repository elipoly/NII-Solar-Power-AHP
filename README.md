
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
├── Bivariate Morans's I/
│
│
├── visuals and maps/
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

## Moran'I - Spatial Analysis

Contains spatial statistical analyses, including Moran's I, Bivariate Moran's I, and Local Indicators of Spatial Association (LISA).


## Data Sources

Several of the original geospatial datasets and downloading procedures used in this project were inherited from the previous NII internship project (see https://github.com/Jae-Domain/Japan-GIS-Data)

For original data sources and downloading scripts, see:

**[Japan-GIS-Data – Jae-Domain](https://github.com/Jae-Domain/Japan-GIS-Data)**

The main datasets reused or extended in this project include:

- **[Solar irradiation – MLIT National Land Numerical Information](https://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-G02-v3_0.html)** 
- **[Slope and aspect – MLIT National Land Numerical Information](https://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-G04-d.html)** 

- **[Land cover – JAXA High Resolution Land Cover Dataset](https://www.eorc.jaxa.jp/ALOS/en/dataset/lulc/lulc_v2312_e.htm)** 

- **[Biodiversity / Land Use – National Institute for Environmental Studies](https://www.nies.go.jp/biology/data/lu.html)** 

- **[Satoyama Index – National Institute for Environmental Studies](https://www.nies.go.jp/biology/data/si.html)** 

- **[Sediment risk – MLIT National Land Numerical Information](https://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-A33-v1_4.html)**

- **[Solar power plant locations – Electrical Japan](http://agora.ex.nii.ac.jp/)**


Additional datasets and processing procedures introduced during the 2025 internship are documented separately in the relevant processing folders.


## Acknowledgements 
https://github.com/kraina-ai/srai


Author
Elisabeth Viau
NII Internship, 2025
National Institute of Informatics, Tokyo, Japan
