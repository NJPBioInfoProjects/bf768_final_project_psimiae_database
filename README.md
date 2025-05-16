# Integrated Genome-Scale Metabolic Database

## Overview
This project implements a structured, searchable SQL-backed database and web interface for managing genome-scale metabolic models (GEMs), developed for **BF768: Biological Database Analysis** at Boston University in Spring 2025. The database supports gap-filling, flux balance analysis (FBA), model version control, and growth simulation data visualization—initially for *P. simiae*, with future extensibility in mind.

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

## Authors
- Vassanth Mathan
- Aravind Panicker
- Nicolas Petrunich
- Benjamin Pfeiffer
- Nicholas White
