# ERA5 Wind Data Visualization

This project demonstrates how to download and visualize ERA5 wind data (u10 & v10) using Python.

## Features

* Download ERA5 data via CDS API
* Load GRIB files using xarray
* Plot wind speed and direction
* Simple and reproducible workflow

---

## Requirements

Install dependencies using conda or pip:

```bash
conda install -c conda-forge xarray cfgrib cdsapi matplotlib numpy pandas
```

or

```bash
pip install xarray cfgrib cdsapi matplotlib numpy pandas
```

---

## CDS API Setup (IMPORTANT)

To download ERA5 data, you must register and configure the CDS API.

### 1. Create an account

Register at:
https://cds.climate.copernicus.eu/

---

### 2. Get your API key

After login, go to:
https://cds.climate.copernicus.eu/api-how-to

Copy your API credentials.

---

### 3. Create `.cdsapirc` file

Create a file in your home directory:

**Windows:**

```
C:\Users\YOUR_USERNAME\.cdsapirc
```

**Linux / Mac:**

```
~/.cdsapirc
```

Paste your credentials:

```
url: YOUR_https/api
key: YOUR_API_KEY
```

---

## Project Structure

```
era5-wind-visualization/
│
├── notebook_1_era5_visualization.ipynb
├── output/
│   └── plotwind.png
├── data/ (optional)
└── README.md
```

---

## How to Use

1. Run the notebook step-by-step
2. Download ERA5 data (u10 & v10)
3. Load GRIB files
4. Visualize wind field

---

## Output Example

![Wind Plot](Output/plotwind.png)

---

## Notes

* ERA5 data is downloaded from Copernicus Climate Data Store
* Time selection can be adjusted using `TIME_INDEX`
* Visualization uses a combination of contour and vector plots

---

## Future Work

* Wind rose analysis
* Multi-year statistics
* Integration with coastal modeling tools

---

## Author

Created as part of a learning and knowledge-sharing initiative on ocean and coastal data analysis.
