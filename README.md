# Preprocessing Brazilian aviation data for RGraphSpace vignette 

Flávio Gabriel Carazza-Kessler, Sysbiolab Team

24 July 2026


This repository provides a reproducible R workflow for preprocessing
Brazilian flight and airport data for spatial network analysis with
RGraphSpace.

## Workflow

The workflow:

1. Downloads 2024 flight records with `flightsbr`.
2. Downloads Brazilian airport metadata.
3. Harmonizes IATA and ICAO airport codes.
4. Removes international routes.
5. Identifies active Brazilian airports.
6. Aggregates flights by origin–destination pair.
7. Converts airport and geographic data to `sf` objects.
8. Saves the processed objects for use in an RGraphSpace vignette.

If you are not familiar to *RGraphSpace*, please see the available workflows: [RGraphSpace - Get Started](https://sysbiolab.github.io/RGraphSpace/articles/get-started.html)

## Rendered vignette

[Read the complete preprocessing workflow](https://flaviogckessler.github.io/PreprocessingAviationData/)

RGraphSpace vignette: [Using RGraphSpace for spatial data analysis](https://flaviogckessler.github.io/PreprocessingAviationData/Using_RgraphSpace_SpatialData.html).

## Data sources

- Agência Nacional de Aviação Civil — ANAC
- `flightsbr`
- `rnaturalearth`

## Main outputs

- Brazilian geographic boundaries
- Active Brazilian airports
- Aggregated domestic flight routes
- Spatial objects for RGraphSpace

## Reproducibility

The repository contains the R Markdown source, rendered HTML output,
bibliographic references, and processed data objects.

# Citation

If you use *RGraphSpace*, please cite:

- Sysbiolab Team (2026). RGraphSpace: A lightweight interface between 'igraph' and 'ggplot2' graphics. R package version 1.2.4. DOI: 10.32614/CRAN.package.RGraphSpace
