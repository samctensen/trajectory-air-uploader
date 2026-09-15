# Trajectory Air Uploader

A Python pipeline that converts atmospheric NetCDF data into vector tilesets and uploads them to Mapbox.

This companion tool supplies map data for [Trajectory Air](https://github.com/samctensen/trajectory-air). It includes CMAQ and NetCDF processing scripts and a pinned Python dependency list.

## Run

Install Python 3 and Tippecanoe, then follow the [setup and upload guide](docs/setup.md). From the repository root, the existing scripts can also be run with Zsh:

```sh
zsh install.sh
zsh upload.sh
```

The installer creates a virtual environment in the repository directory. Uploads require your Mapbox account and a token with tileset read/write permissions. The upload command sends data to Mapbox.

## Project

- `UploadCMAQ.py`, `UploadNetCDFs.py` — data processing and upload pipelines.
- `install.sh`, `upload.sh` — environment setup and execution.
- `requirements.txt` — Python dependencies.
