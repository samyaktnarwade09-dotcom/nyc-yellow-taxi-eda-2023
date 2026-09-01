# Data Folder

## Official Dataset Source

This project uses the **2023 Yellow Taxi Trip Records** provided by the New York City Taxi & Limousine Commission (TLC).

### Download Full Dataset
- Official Page: [https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- Required files:  
  `yellow_tripdata_2023-01.parquet`  
  `yellow_tripdata_2023-02.parquet`  
  ...  
  `yellow_tripdata_2023-12.parquet`

Place all 12 monthly Parquet files in this `data/` folder (or update the paths in the notebook accordingly).

---

## Taxi Zones Shapefile (Required for Geospatial Analysis)

Download the official Taxi Zone shapefile from the TLC website or NYC Open Data.

You need the complete set of files:
- `taxi_zones.shp`
- `taxi_zones.shx`
- `taxi_zones.dbf`
- `taxi_zones.prj`
- (and other related files)

Create a folder named `taxi_zones` inside this directory and place all shapefile components inside it:

```
data/
└── taxi_zones/
    ├── taxi_zones.shp
    ├── taxi_zones.shx
    ├── taxi_zones.dbf
    └── ...
```

---

## Sample Data Included

A small cleaned sample is provided for quick testing and demonstration purposes:

- **`sample_yellow_taxi_2023.csv`** → Approximately 5,000 rows of cleaned 2023 Yellow Taxi data.

This sample allows anyone to run parts of the analysis without downloading the full multi-GB dataset.

> **Note**: The sample is for demonstration only. For complete and accurate results, please use the full official dataset.

---

## Recommended Folder Structure After Downloading Data

```
data/
├── README.md
├── sample_yellow_taxi_2023.csv
├── yellow_tripdata_2023-01.parquet
├── yellow_tripdata_2023-02.parquet
├── ... (other months)
└── taxi_zones/
    ├── taxi_zones.shp
    ├── taxi_zones.shx
    └── ...
```
