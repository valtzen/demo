# ECMWF Open Data – Jupyter Notebooks

This repository contains Jupyter notebooks demonstrating how to access and visualise ECMWF Open Data using [earthkit-data](https://earthkit.readthedocs.io/), [earthkit-plots](https://earthkit-plots.readthedocs.io/), and [ecmwf-opendata](https://github.com/ecmwf/ecmwf-opendata).

## Notebooks

- **Novice Notebook** – Step-by-step introduction to retrieving and plotting ECMWF Open Data.
- **Advanced Notebook** – Covers advanced retrieval options, multiple models, and richer plotting techniques.

## Repository Structure

```
ecmwf-open-data-jupyter/
├── data/                # Downloaded GRIB/NetCDF files (ignored in Git)
├── env/                 # Environment configuration files
├── notebooks/           # Jupyter notebooks (novice & advanced)
├── README.md            # This file
└── .gitignore           # Git ignore rules
```

## Installation

We recommend using [conda](https://docs.conda.io/) with the provided environment file:

```bash
conda env create -f env/environment.yml
conda activate ecmwf-open-data-jupyter
```

## Running the Notebooks

1. Start JupyterLab:
    ```bash
    jupyter lab
    ```
2. Open the desired notebook from the `notebooks/` folder.
3. Follow the cell instructions to retrieve and plot data.

## Data Sources

The notebooks use the **ECMWF Open Data** service:
- Documentation: [https://www.ecmwf.int/en/forecasts/datasets/open-data](https://www.ecmwf.int/en/forecasts/datasets/open-data)
- Access via the `ecmwf-opendata` Python client.

## Plotting

We use:
- **earthkit-data** to read and manipulate GRIB data.
- **earthkit-plots** for map visualisation.
- **matplotlib** for custom plotting.

## License

To be clarified... CC-BY?

