# Cleaning the shorebird survey data 


## The data set

ARCTIC SHOREBIRD DEMOGRAPHICS NETWORK [https://doi.org/10.18739/A2222R68W](https://doi.org/10.18739/A2222R68W)

Data set hosted by the [NSF Arctic Data Center](https://arcticdata.io) data repository 

Field data on shorebird ecology and environmental conditions were collected from 1993-2014 at 16 field sites in Alaska, Canada, and Russia.

![Shorebird, copyright NYT](https://static01.nyt.com/images/2017/09/10/nyregion/10NATURE1/10NATURE1-superJumbo.jpg?quality=75&auto=webp)

Data were not collected every year at all sites. Studies of the population ecology of these birds included nest-monitoring to determine the timing of reproduction and reproductive success; live capture of birds to collect blood samples, feathers, and fecal samples for investigations of population structure and pathogens; banding of birds to determine annual survival rates; resighting of color-banded birds to determine space use and site fidelity; and use of light-sensitive geolocators to investigate migratory movements. 

Data on climatic conditions, prey abundance, and predators were also collected. Environmental data included weather stations that recorded daily climatic conditions, surveys of seasonal snowmelt, weekly sampling of terrestrial and aquatic invertebrates that are prey of shorebirds, live trapping of small mammals (alternate prey for shorebird predators), and daily counts of potential predators (jaegers, falcons, foxes). Detailed field methods for each year are available in the `ASDN_protocol_201X.pdf` files. All research was conducted under permits from relevant federal, state, and university authorities.

See `01_ASDN_Readme.txt` provided in the [course data repository](https://github.com/UCSB-Library-Research-Data-Services/bren-meds213-spring-2024-class-data) for full metadata information about this data set.

### Purpose 
The purpose of this repository is to exercise data science techniques for data cleaning and metadata creation for the `ASDN_Snow_survey.csv` data. 

### File Structure

```
├── README.md
├── .gitignore
├── eds213_data_cleaning_assign_Tom_Gibbens-Matsuyama.qmd   # File for data cleaning
└── data/
    ├── processed/                                          # Processed data/
    │   ├── all_cover_fixed_Tom_Gibbens-Matsuyama.csv       # Fully cleaned snow survey data
    │   └── snow_cover.csv                                  # Partially cleaned
    │   └── species_present.csv                             # Species identified at site 
    └── raw/                                                # Prepprocessed data/
        ├── 01_ASDN_Readme.txt                              # Original metadata
        ├── ASDN_Daily_Species.csv                          # Species survey data
        └── ASDN_Snow_Survey                                # Snow cover survey data
```
Other data related data not contained within this repository are the following: `Bird_captures`, `Bird_eggs`, `Bird_nests`, `Bird_resights`, `Bird_sexes`, `Camp_info`, `Camp_assignment`, `Daily_pred_lemm`, `Daily_species`, `Daily_species_effort`, `Geodata`, `Inverts`, `Lemming_counts`,  `Lemming_nests`, `Lemming_trap`, `Pred_nests`, `Pred_point_counts`, `Study_Plot`, `Surface_water`, `Weather_HOBO`, `Weather_precip_manual`, `Weather_snow_manual`. 

Metadata for these files can be found on the `01_ASDN_Readme.txt` file located in the `raw` folder. 

#### Mutiple Versions
Data was processed from the MEDS EDS-213 Repository: [bren-meds213-data-cleaning](https://github.com/UCSB-Library-Research-Data-Services/bren-meds213-data-cleaning)

#### Metadata
Metadata for the `all_cover_fixed_Tom_Gibbens-Matsuyama.csv` file in this repository is as follows:

**Number of variables:** 11

**Number of rows:** 38,241

| Variable         | Description                        | Value               |
|---------------|------------------------------------|-----------------------|
| Site          | Four letter abbreviation for where data was collected                | char      |
| Source        | Where the data comes from          | Kaggle                |
| Size          | Number of records and fields       | 891 rows, 12 columns  |
| License       | Usage license                      | CC0: Public Domain    |
| Last Updated  | Date of last update                | 2025-05-01            |






