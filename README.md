# ECMWF Open Data – Jupyter Notebooks

This repo contains Jupyter notebooks that retrieve and visualise **ECMWF Open Data** using:
- [earthkit-data](https://earthkit.readthedocs.io/) — load/select GRIB
- [earthkit-plots](https://earthkit-plots.readthedocs.io/) — mapping, contours, vectors
- [ecmwf-opendata](https://github.com/ecmwf/ecmwf-opendata) — download client
- [MetPy](https://unidata.github.io/MetPy/latest/) — Skew‑T, CAPE/CIN, parcel paths, shear

## What’s in here

- `notebooks/` — examples covering:
  - IFS‑single / IFS‑ENS / IFS waves and AIFS (open‑data 0.25° grid)
  - Map plots (filled fields, MSLP isolines, wave products)
  - Wind plots (barbs/quiver) with subsampling & colorbars
  - Point time‑series (single and ensemble)
  - Vertical profile (Skew‑T/Log‑P) with SFC/MU/ML parcels, CAPE/CIN, 0–6 km shear, LCL, θe
- `data/` — **ignored**; downloads land here
- `env/environment.yml` — reproducible environment

We suggest using conda or mamba for creating an enviroment and istalling required dependencies as listed in environment.yml running this.

## Notes on ECMWF Open Data

- Open‑data IFS products are **0.25°** GRIB2 (global).  
- Families included here: **IFS‑single**, **IFS‑ENS**, **IFS waves**, **AIFS (single/ENS)**.  
- Docs:  
  - Overview: https://www.ecmwf.int/en/forecasts/datasets/open-data  
  - Access & details: https://confluence.ecmwf.int/display/DAC/ECMWF+open+data%3A+real-time+forecasts+from+IFS+and+AIFS

## Dependencies

Managed via `env/environment.yml`. Key packages:
- `earthkit-data`, `earthkit-plots`, `ecmwf-opendata`, `eccodes`
- `cartopy`, `matplotlib`, `numpy`, `xarray`, `scipy`, `pandas`
- `metpy`, `pint`

## Data & licensing

ECMWF open data license: **Attribution 4.0 International (CC BY 4.0)**. If you use figures in publications, please attribute ECMWF.
