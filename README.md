# AUSO capacity building

Various partners have indicated that capacity building is an important goal of AUSO. In this repo we will collect some existing capacity building materials for various AUSO related topics. The materials are clustered around typical steps in the soil data organization workflow.

We welcome you to verify the materials and provide feedback on lacking details or ideas via [github issues](https://github.com/soil-data-of-africa/auso-capacity-building/issues).

## Field work

Field studies require careful preparation, to be as effective as possible.

### Sampling design

Any campaign starts with a careful analysis, where samples can best be collected.

- [Brus et al, 2022](https://dickbrus.github.io/SpatialSamplingwithR/) provides guidance using the R tooling.

### Sampling organisation

A SDMT tool can support the organisation of a sampling campaign.

- [Soils for Africa - SDMT manual](https://doi.org/10.3030/862900)

### Field work and soil sampling

Various approaches and guidances exist on how to execute the field work

- [WRB Fieldguide (Annex 1)](https://wrb.isric.org/documents.html) 
- [USDA fieldbook](https://www.nrcs.usda.gov/sites/default/files/2022-09/field-book.pdf)
- [AfSIS LSDF field guide](https://www.landscapealliance.org/publications/pdf/guide/45871-LDSF-Field-Guide-2025.pdf)
- [Soils 4 Africa; fieldwork guidance](https://africasis.isric.org/res/files/Soils4Africa_D3.3_Guidance_Fieldwork_v01_FINAL.pdf)

A [series of videos](https://www.youtube.com/@soils4africa373/videos) in various languages has been produced by the Soils for Africa project for field work and sample treatment

### Sample Preparation and Shipment 

Careful preparation and shipment of samples prevents quality loss.

- [Sample Preparation and Shipment](https://doi.org/10.3030/862900)
  
### Soil Classification

During a field work, soils are typically classified according to local and/or global classification systems

- [WRB classification](https://wrb.isric.org/documents.html)
- [Classification using USDA taxonomy](https://www.nrcs.usda.gov/sites/default/files/2022-06/Soil%20Taxonomy.pdf)

## Laboratory

Alignment of laboratory procedures is key for interoperability

- [Guidance_Laboratory_Analysis](https://africasis.isric.org/res/files/Soils4Africa_D3.4_Guidance_Laboratory_Analysis_v01.pdf)
- [FAO Glosolan - Standard Operating Procedures](https://www.fao.org/global-soil-partnership/Scientific-and-technical-support/networks/the-glosolan/standard-operating-procedures-(sops)/en)

## Data processing

This section describes various steps in data processing

### Data cleaning and archiving

During and after a campaign data arriving from the field and lab (wet-chem, physical properties, and NIR) need to be properly linked and archived.
Data is best archived following the FAIR principles in persistent repositories, assigning a PID (DOI, Handle) to each publication to facilitate referencing the data from publications.

- [Soilwise - FAIR strategy for Soil data en knowledge](https://soilwise-he.github.io/soilwise-fair-strategy/)

### Observation data harmonization 

To bring data from various sources together into a single dataset, it is important to align data formats as well as data for different observed properties, units and analysis methods. A pH value measured in a 1:2.5 suspension is typically not the same as measured in a 1:10 suspension. Some transfer functions are described to transform between various method alternatives.

- [iso28258 database](https://github.com/ISRICWorldSoil/iso-28258) ISRIC maintains a PostGreSQL database model, set up according to the iso28258 standard, to capture soil observation data with full metadata
- [Soilwise - Observation data encodings](https://soilwise-he.github.io/soil-observation-data-encodings/)
- [Soilharmony - Transfer functions](https://github.com/soilharmony) the project is currently in starting phase but is expected to provide good overview of existing knowledge on transfer functions

### (Digital) Soil Mapping

Traditionally soil maps are created by experts in the field. Alternatively Digital Soil Mapping is a technology 
which predicts the distribution of soil properties in space and time, using existing soil observation data and covariates, such as Digital elevation, 
Leaf area index, geology, hydrology.

- [Data preparation for DSM](https://resources.isric.org/tutorial/dsm_data_preparation/)
- [Geostatistics for soil mapping](doi.org/10.17027/isric-fdtz-ma12)
- [Machine Learning for Digital Soil Mapping](doi.org/10.17027/isric-krcc-9045)
  
## Data usage for decision support 

Soil maps can be used to support decision making. For optimal reuse make your maps available to various communities.

- [Basic Raster Styling and Analysis (QGIS3)](https://www.qgistutorials.com/en/docs/3/raster_styling_and_analysis.html)
- [Cloud Optimized GeoTiff in OpenLayers](https://github.com/openlayers/workshop/blob/main/doc/en/cog/README.md)
- [Introduction to rasters with terra (R)](https://emlab-ucsb.github.io/intro-terra/)

