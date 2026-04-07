# Kigali-Global-Flood-Models

Reliable flood models are critical for early warning systems in data-scarce urban environments. This repository contains data and Jupyter notebooks supporting the report:

Zuetell, E., Tetero, F., Mutoni, A., Bwirayesu, G.,\& Busogi, M. (2026). Enabling Urban Flood Models and Flood Early Warning Systems in Kigali City – Rwanda: A Review and Audit of Hydrometeorological Data and Models.

Notebooks analyze hydrometeorological observations and compare outputs from global flood forecasting models against locally-calibrated HEC-HMS/HEC-RAS simulations across four flood hotspots in Kigali, Rwanda.

1. Karuruma: The Nyabugogo River at the Karuruma Bridge
2. Rugunga: the Rwampara river at Rugunga
3. Mpazi: The Mpazi River at RN3
4. Ruliba: The Nyabarongo River at Ruliba Bridge
   
---
 
## Data Sources
 
| Dataset | Source | Access |
|---|---|---|
| CHIRPS satellite rainfall | [Climate Hazards Center, UCSB](https://www.chc.ucsb.edu/data/chirps) | Public |
| Streamflow gage records | [Rwanda Water Resources Board-Water Portal](https://waterportal.rwb.rw/data/surface_water) | Public - Rwanda Water Portal |
| Rainfall station records | Meteo Rwanda | Request Required |
| Google Flood Hub | [Google Flood Hub](https://sites.research.google/floods/) | Public API |
| GEOGloWS Flood Forecasts | [GEOGloWS ECMWF Streamflow](https://geoglows.ecmwf.int/) | Public API |
| HEC-HMS / HEC-RAS outputs | Developed as part of this study | Included in `Model Data/` |
 
---
## Notebooks

### Data Access and Preparation

**`CHIRPS_Data_Download.ipynb`**  
Downloads Climate Hazards Group InfraRed Precipitation with Station data (CHIRPS) for the Kigali region.

**`RWRB_Hydrology_Station_Data.ipynb`**  
Processes streamflow records from Rwanda Water Resources Board (RWRB) gauge stations. Includes data cleaning, gap identification, and summary statistics for stations used in model calibration and validation.

**`Rainfall_Station_Summary.ipynb`**  
Summarizes and visualizes rainfall records from ground-based stations across Kigali. Produces station-level statistics and comparison plots used in the hydrometeorological data audit.

**`Kigali_Flood_Sensors.ipynb`**  
Maps Kigali flood hotspots alongside local sensors and global model prediction points.

### Case Studies

**`Case_Study_01_Karuruma.ipynb`**  
Develops continuous and event-based rainfall-runoff models for the Karuruma catchment using weather station precipitation data. Compares modeled inundation extents against globally available Sentinel-2 derived flood extents.

**`Case_Study_02_Rugunga.ipynb`**  
Validates the use of CHIRPS satellite rainfall as an input to local rainfall-runoff models in HEC-HMS/HEC-RAS.

**`Case_Study_03_FloodModelIntercomparison.ipynb`** / **`Flood_Model_Intercomparison.ipynb`**  
Compares GEOGloWS and Google Flood Hub streamflow predictions against observed discharge records at the Ruliba site. 

---

## Acknowledgments
This work was produced as part of the Kigali Flood Modeling Working Group and comprised of researchers from Rwanda Young Water Professionals and Carnegie Mellon University - Africa. Collaborators include Francois Tetero (RYWP/GWP), Moise Busogi (CMU-Africa), Emily Zuetell (CMU), Alice Umutoni (RYWP), Gustave Bwirayesu (CMU), Hussein Bizimana (UoR). Alice Umutoni led the HEC-HMS/HEC-RAS Flood Model Development.

[![DOI](https://zenodo.org/badge/1086020014.svg)](https://doi.org/10.5281/zenodo.19463101)
