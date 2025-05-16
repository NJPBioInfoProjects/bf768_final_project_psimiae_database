# Integrated Genome-Scale Metabolic Database

## Overview
This project implements a searchable, version-controlled metabolic modeling database for the organism *Pseudomonas simiae* (P. simiae), developed as part of BF768 at Boston University. The system is designed to support gap-filling, flux balance analysis (FBA), and growth data visualization across multiple experimental conditions.

The data originates from internal research at the Segrè Lab, which focuses on microbial metabolism and systems biology. *P. simiae* was grown in a 96-well plate under various media and growth conditions (e.g., glucose, sucrose, xylitol). Media compositions, biomass data, and model annotations were collected using tools like KBase, RASTtk, and Model SEED.

Simulated growth curves were generated using COMETS (Computation of Microbial Ecosystems in Time and Space), which models dynamic microbial interactions and metabolite fluxes in spatially structured environments. These simulations support insights into metabolic behavior and the effects of gap-filled reactions.

This internal-use platform provides an upload portal for metabolic model files, a search and filter interface for media-based growth conditions, downloadable datasets, and tools for visualizing metabolite charge and growth outcomes.

## Features
- **Search Interface**: Query models by growth medium and filter by growth result.
- **Upload Portal**: Upload metabolic model files (.xml) and associated growth/biomass data (.tsv).
- **Charge Visualization**: Interactive browser-based charts for metabolite charge distributions.
- **Downloadable Data**: Model data and outputs can be downloaded in XML or TSV formats.

## Repo Structure
- `templates/`: HTML templates for different pages of the web application:
  - `about.html`: Background and scope of the project
  - `functionality.html`: Interactive charge distribution visualizer for metabolites
  - `help.html`: Step-by-step usage guide
  - `index.html`: Homepage with search and upload interface
  - `intro.html`: Project overview and abstract
  - `linked_databases.html`: Tab containing links to linked databases, such as KEGG and BiGG
  - `navbar.html`: Navigation bar placed at the top of the webpage
- `app.py`: Flask server for handling file uploads, database queries, and routing.

## Access and Usage
This application is designed for **internal lab use at the Segrè Lab.** Data access is protected, and uploads are limited to authorized users. There is currently no public API.

## Credentials and DB Setup
For privacy and security, database connection strings and credentials were intentionally removed from this repo.


## Authors
- Vassanth Mathan
- Aravind Panicker
- Nicolas Petrunich
- Benjamin Pfeiffer
- Nicholas White
