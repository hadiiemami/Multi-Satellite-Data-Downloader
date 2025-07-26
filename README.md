# Multi-Satellite Data Downloader

A Jupyter Notebook for downloading various satellite datasets from Copernicus and related sources. This tool automates querying and retrieving geospatial data based on user-defined parameters such as date, location, and dataset type.

## Supported Datasets
The script supports downloading the following datasets:
- SENTINEL3_OLCI_L1B
- SENTINEL3_SLSTR
- SENTINEL_5P_L2
- COPERNICUS_VEGETATION_PHENOLOGY_PRODUCTIVITY_10M_SEASON1
- COPERNICUS_VEGETATION_PHENOLOGY_PRODUCTIVITY_10M_SEASON2
- COPERNICUS_PLANT_PHENOLOGY_INDEX
- ESA_WORLDCOVER_10M_2020_V1
- ESA_WORLDCOVER_10M_2021_V2
- COPERNICUS_VEGETATION_INDICES
- SENTINEL2_L1C
- SENTINEL2_L2A
- SENTINEL1_GRD
- COPERNICUS_30
- LANDSAT8_L2
- SENTINEL3_SYN_L2_SYN
- SENTINEL3_SLSTR_L2_LST
- SENTINEL1_GLOBAL_MOSAICS

## Features
- Connects to APIs (e.g., Copernicus Open Access Hub) for data retrieval.
- Supports customizable search criteria (e.g., geographic coordinates, date range).
- Organizes downloaded data for geospatial analysis.
- Implemented as a Jupyter Notebook for interactive use.

## Requirements
- Python 3.x
- Libraries: `sentinelsat`, `geopandas`, `requests`, `jupyter` (install via `pip install -r requirements.txt`)
- Copernicus SciHub account (free registration at [SciHub](https://scihub.copernicus.eu/)) for Sentinel datasets
- Access credentials for other data sources (e.g., USGS for Landsat)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/multi-satellite-downloader.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure API credentials in the notebook or a separate config file.

## Usage
1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook download_satellite_data.ipynb
   ```
2. Follow the instructions in the notebook to set parameters (e.g., dataset, location, date).
3. Run the cells to query and download the desired dataset.

## Example
To download Sentinel-2 L2A images for a specific location and date:
- Set parameters in the notebook (e.g., `lat=35.7`, `lon=51.4`, `date='2023-01-01'`, `cloud_cover=20`).
- Execute the download cell to retrieve the data.

## Notes
- Ensure valid credentials for each data source (e.g., Copernicus SciHub, USGS).
- Suitable for researchers working on remote sensing, environmental monitoring, or geospatial analysis.
- Check the notebook for dataset-specific instructions and parameter options.

## License
MIT License